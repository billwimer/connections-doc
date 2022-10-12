# Upgrade considerations for Component Pack 8 {#upgrade_considerations .concept}

The upgrade path described in [Steps to install or upgrade to Component Pack 8](cp_install_services_tasks.md) is based on a given set of components, versions, and goals. Consider the following information when deciding how best to upgrade based on your deployment and needs.

## Side-by-side vs. in-place {#section_jch_yrx_bvb .section}

The approach in [Steps to install or upgrade to Component Pack 8](cp_install_services_tasks.md) focuses on upgrading Connections 7 to 8 on the same set of machines. This involves an in-place upgrade of an existing Kubernetes environment by touching file shares, and Helm release and charts.

If your upgrade strategy requires a side-by-side migration on a mirrored set of both WebSphere and Kubernetes machines, you can still use the installation document. The difference between the two approaches is the transfer of data from source to destination system.

For a side-by-side migration, these would be the steps:

-   Set up a mirrored WebSphere system with the same version as the source system
-   Migrate or switch file shares and databases
-   Migrate Connections or Docs configuration between the two systems
-   In-place upgrade of the mirrored WebSphere Application Server \(set\) by touching the database, WebSphere, HTTP Server components, and Connections
-   Set up a mirrored Kubernetes system with the same version as the source system
-   Migrate or switch file shares \(PVs\) between the two systems
-   In-place upgrade of the mirrored Kubernetes environment by touching file shares, and Helm release and charts

For more information, see [Upgrade considerations for side-by-side migration of data](cp_upgrade_considerations_for_side_by_side_migration.md).

## Docker {#section_qcg_btx_bvb .section}

To deploy Component Pack, we use HCL Software’s Harbor container registry. Modify the reference according to your environment. When provisioning Component Pack 8, you can empty your local Docker repository or manually delete the Connections 7 parts before starting the upgrade to version 8.

## Switch container runtime {#section_sqh_ktx_bvb .section}

Ensure containerd is up and running on Kubernetes master and worker nodes. Follow the steps in [migrating from Docker to containerd](http://kruyt.org/migrate-docker-containerd-kubernetes).

Watch out for the --network-plugin flag. You will need to remove it from /var/lib/kubelet/kubeadm-flags.env, otherwise kublet won't start after upgrading to v1.24. For details, view the [GitHub issue](https://github.com/kubernetes/website/issues/33640).

**Note:** Since we switched the container runtime from Docker to containerd, there is a possibility that all pods will show status as 'ImagePullBackOff'.

## Kubernetes {#section_avm_v5x_bvb .section}

If your Component Pack services run on an older Kubernetes version, we strongly recommend that you upgrade to version 1.24 before moving to Connections 8. As an example, if your Kubernetes version is 1.19, step up to 1.20 via 1.21, 1.22, and so on. See [Prerequisites for Component Pack](cp_prereqs.md).

## Kubernetes-based services {#section_ay1_5vx_bvb .section}

During the installation scenario, we will upgrade our Kubernetes stack to the newest Connections Component Pack release. This will impact the cpmaster.example.com machine, which runs the containerized modules.

## Helm {#section_bqv_2vx_bvb .section}

We recommend that you upgrade Helm to version 3.7.2.

## OpenSearch {#section_wsm_gvx_bvb .section}

Connections 8 defines OpenSearch 1.3.0 as the default backend for Orient Me, search and Metrics – this is what we'll deploy and configure in our installation scenario. Previous Connections releases used an older Elasticsearch 7 version, which is no longer needed.

**Note:** In case you already have Metrics deployed and its data collected, and you do not want to start Metrics from scratch, you will have to migrate these data into the new release. [Steps to install or upgrade to Component Pack 8](cp_install_services_tasks.md) covers both scenarios.

**Parent topic:**[Installation and upgrade](../install/cp_install_upgrade_container.md)
