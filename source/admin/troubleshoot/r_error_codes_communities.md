# Communities error messages {#r_error_codes_communities .reference}

Use the codes included in the error messages that are generated by HCL Connections™ to identify problems with the Communities application and find solutions.

## Communities messages { .section}

The following Communities error messages are generated by Connections:

|Message|Cause|Solution|
|-------|-----|--------|
|CLFRM\#\#\#\#E: A JNDI naming exception was caught, probably the result of a deployment error.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0001E: Communities https service url is malformed: \{0\}.|The web address that is specified is in an invalid URL syntax.|Correct the URL syntax.|
|CLFRM0002W: SubjectHelper.cloneSubject was called with null subject.|There is a problem with the authenticated user that results in null information.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0003E: Communities http service url is malformed: \{0\}.|The web address that is specified is in an invalid URL syntax.|Correct the URL syntax.|
|CLFRM0004I: Executing \{0\} request.|The specified request is being executed.|Informational message, no solution is needed.|
|CLFRM0005E: Error executing update community name for \{0\}.|Could not update specified community.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0006I: Executing create community. Community name: \{0\}.|Creating the specified community.|Informational message, no solution is needed.|
|CLFRM0007E: Error registering mbean.|An exception was generated when registering the MBeans.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0008E: Error executing remove tags from \{0\}.|Could not remove tags from specified community.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0009E: Unknown role assignment in createCommunity call: role must be either OWNER or MEMBER.|Invalid role parameter used in administrative command.|Correct the syntax and retry the command.|
|CLFRM0010I: Executing add members to \{0\}.|Adding members to the specified community.|Informational message, no solution is needed.|
|CLFRM0011E: Error initializing Communities JMX support: failed to register \{0\}.|The web address that is specified is in an invalid URL syntax.|Correct the URL syntax.|
|CLFRM0012I: Executing remove tags from \{0\}.|Executing the specified command.|Informational message, no solution is needed.|
|CLFRM0013E: Error purging index.|An error occurred while purging the full text index.|Shut down and restart the server. If the error persists, report this problem to Customer Support.|
|CLFRM0014E: Error locating MBeanServer, no Community Administration MBeans registered.|An exception was generated when locating the MBean server needed to register the MBeans.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0015E: User \{0\} was not found.|The specified user was not found in the directory. The command cannot be executed.|Check the spelling of the user name and the directory configuration.|
|CLFRM0016E: Error executing \{0\}.|There was an error executing the specified request.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0017E: Error executing update community description for \{0\}.|The description of the specified community could not be updated.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0018I: Executing update community name. Changing \{0\} to \{1\}.|Updating community name as specified.|Informational message, no solution is needed.|
|CLFRM0019E: Error initiating indexing operation.|An error caused by initializing the full text index.|Shut down and restart the server. If the error persists, report this problem to Customer Support.|
|CLFRM0020E: Error executing add members to \{0\}.|Could not add members to specified community.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0021E: Error executing remove references by URI from \{0\}.|Could not remove references from specified community.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0022E: Error executing create community. Community name: \{0\}|Could not create a community with specified name.|Check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0023I: Executing start indexing request.|The index is being started.|Informational message, no solution is needed.|
|CLFRM0024I: Executing remove references by URI from \{0\}.|Removing requested references from specified community.|Informational message, no solution is needed.|
|CLFRM0025I: Executing purge index request.|The index is being purged.|Informational message, no solution is needed.|
|CLFRM0026I: Executing update community description for \{0\}.|The community description is being updated.|Informational message, no solution is needed.|
|CLFRM0027E: Community not found: \{0\}.|The community specified was not found.|Informational message, no solution is needed.|
|CLFRM0028E: Cannot create reference with duplicate URI: \{0\}.|Cannot create a reference with the specified name.|A reference with the specified name exists within this community and cannot be duplicated. Select a different name and execute the command again.|
|CLFRM0029E: Error executing update all member external ids, profiles.|The update member external IDs process encountered an error. Additional information that relates to the failure can be found in the SystemOut.log file.|If the problem persists after you restart the Communities application, contact Customer Support to report the incident.|
|CLFRM0029I: Finished writing index at: \{0\}.|The full text index task finished updating the index at the specified time.|Informational message, no solution is needed.|
|CLFRM0030E: Error: Index may be corrupted. Please re-run the indexing task to build a new index.|The full text index might be corrupted. Full text search does not function.|Use the administrative tasks to purge and reload the index.|
|CLFRM0031E: Error retrieving IndexWriter.|The server cannot update the full text index.|If the error persists, stop, and then restart the server.|
|CLFRM0032E: Error deleting community documents from the index.|The server was unable to delete the documents from the full text index.|Try again to delete the documents or use the administrative tasks to purge and reload the full text index.|
|CLFRM0033E: There is no directory profile associated with this email address <mail address\>|The wsadmin command could not be performed because the specified email address did not match any entries in the directory.|Correct the email address or use a login name to specify the user.|
|CLFRM0033I: Initializing Communities Management.|The communities management application is initializing.|Informational message, no solution is needed.|
|CLFRM0034E: Error writing last update to \{0\}.|The server encountered an error when writing the full text index last update time to the file system.|If the error persists, stop and then restart the server.|
|CLFRM0035E: Severe error executing update member id, profile in batch mode. Processing will terminate.|The update member external IDs process encountered an error. Additional information that relates to the failure can be found in the SystemOut.log file.|Investigate any additional errors that can be found in the SystemOut.log file.|
|CLFRM0035I: Full-text search was started at: \{0\}.|The full text search was started at the specified time.|Informational message, no solution is needed.|
|CLFRM0036E: Unable to find reference with id: \{0\}.|A reference with the specified identifier was not found.|Check the parameter value and try again. If the problem persists, check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0037E: User is not authorized to perform the indexing task on communities.|The indexing task is not running under an authorized user account.|Stop and then restart the server. If the error persists, report the problem to Customer Support.|
|CLFRM0038E: Error retrieving the last update from \{0\}.|The server encountered an error when retrieving the full text index last update time from the file system.|If the error persists, stop and then restart the server.|
|CLFRM0040E: The list argument passed to updateMemberIdBatch was null or empty|No IDs were passed into the updateMemberIdBatch wsadmin command.|Supply one or more IDs when using the updateMemberIdBatch command.|
|CLFRM0039E: Internal error.|An internal error has occurred.|See the SystemOut.log file for more information about the error.|
|CLFRM0040I: Starting to write the index at: \{0\}.|The full text index task started to update the index at the specified time.|Informational message, no solution is needed.|
|CLFRM0041E: Unable to find community with id: \{0\}.|The community with the specified identifier was not found.|Check the parameter value and try again. If the problem persists, check the database connection. See the SystemOut.log file for more information about the error.|
|CLFRM0042E: Schema Version Mismatch.|The database schema does not match the application version.|Upgrade the database using the specified procedure.|
|CLFRM0043E: Cannot create community with duplicate name: \{0\}.|Cannot create a community with the specified name.|A community with the specified name exists and cannot be duplicated. Please select a different name and execute the command again.|
|CLFRM0044E: Error retrieving the full-text index. Stopping scheduled full-text indexing for Communities.|The server could not initialize the full text indexing service. The indexing service is disabled.|Stop, and then restart the server. If the error persists, report the problem to Customer Support.|
|CLFRM0045E: Error parsing the search query.|The search query syntax was invalid.|Correct the syntax and enter the command again.|
|CLFRM0046I: Stopping Communities Management.|The communities management application is stopping.|Informational message, no solution is needed.|
|CLFRM0047E: User passed NULL directory member profile to getCurrentMemberProfile\(\) method.|The member profile parameter is invalid; a non-null value is required.|Specify appropriate parameters for the request.|
|CLFRM0048E: Error retrieving communities for indexing.|An error occurred searching the full text index.|Stop and then restart the server. If the error persists, report the problem to Customer Support.|
|CLFRM0049E: NOT IMPLEMENTED.|This function is not implemented.|See the SystemOut.logfile for more information about the error.|
|CLFRM0050E: Cannot find credentials for <alias name\>|The J2C Authentication alias <alias name\> could not be found.|In the WebSphere® Application Server Integrated Solutions Console, expand **Security**, select **Global security**, then expand **Java Authentication and Authorization Service** and select **J2C authentication data**, and check whether there is an entry for name. If there is no entry, create an Authentication Alias for name by completing these steps: 1.  Shut down the WebSphere Application Server.
2.  Edit the security.xml file in the following directory: APPServer\_HOME/profiles/AppSrv01/config/cells/cell
3.  Find the authDataEntries entry with an alias that includes <name\>.

For example:

    ```
<authDataEntries alias="text/name"> 3.0.1
    ```

4.  Replace "text/name" with "name".
5.  Save the security.xml file.
6.  Restart the WebSphere Application Server. If there is an entry for <name\>, verify that the user credentials are correct. If these steps do not fix the problem, then contact Customer Support.

|
|CLFRM0050E: Error sending member added or member removed mail notification|A mail notification alerting users that they have been added or removed from a community was not sent. Additional information relating to the failure can be found in the SystemOut.log file.|Ensure that the SMTP and DNS servers that are configured in the notifications-config.xml are reachable.|
|CLFRM0052E: Failed to create worker thread for the event queue.|A background process failed to create a thread to handle additional work.|If the problem persists after you restart the Communities application, contact Customer Support to report the incident.|
|CLFRM0054E: Error parsing communities-policy.xml: \{0\}|The communities-policy.xml file is not in a valid format.|Correct any minor syntax issues in the file or obtain a copy of this file from a clean install.|
|CLFRM0055E: Error fetching Member list.|Not identifiable without more information. Report this problem to Customer Support.|Not identifiable without more information. Report this problem to Customer Support.|
|CLFRM0056E: Error fetching Community Data.|Not identifiable without more information. Report this problem to Customer Support.|Not identifiable without more information. Report this problem to Customer Support.|
|CLFRM0057E: Unable to get application list.|Not identifiable without more information. Report this problem to Customer Support.|Not identifiable without more information. Report this problem to Customer Support|
|CLFRM0059E: Error fetching links and bookmarks.|A problem occurred while running CommunitiesService.fetchReference\(\)|Ensure that all passed in community uuids are valid.|
|CLFRM0066E: Error adding member, who has name: \{0\}, email: \{1\}, and member uuid: \{2\}, to community, which has name: \{3\}, and its community uuid: \{4\}.|This error message may show if adding a person as a community member when the person is already a member or owner.|Check to see whether the person is now a member. If not, try to readd the person. If problems persist, contact Customer Support.|
|CLFRM0070E: Error updating property values in a link.|Error while updating a managed application property value.|Validate the specified link is valid.|
|CLFRM0072E: Cannot find application "\{0\}" for community "\{1\}".|A managed application could not be found for the specified community.|Validate the managed application type and community uid are correct.|
|CLFRM0073E: Unknown application <managed application name\>.|The specified <managed application name\> could not be found.|Correct the specified name.|
|CLFRM0077E: Error caused by an invalid input.|An invalid number of parameters or empty string parameters were passed to a wsadmin command for managed applications.|See [Communities administrative commands](../admin/r_admin_communities_admin_props.md) for the correct parameters to pass.|
|CLFRM0078E: Error updating URI links in an application for a community.|An error occurred while attempting to update a managed application link.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0079E: Error fetching application link list.|An error occurred while attempting to fetch managed application links.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0081E: Error creating application link.|An error occurred while attempting to create a managed application link.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0082E: Error deleting application link.|An error occurred while attempting to delete a managed application link.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0083E: Error fetching application properties.|An error occurred while attempting to fetch a managed application's properties.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0084E: Error during initializing VenturaConfigurationHelper|The server could not retrieve or successfully parse a LotusConnections-config.xml configuration file from the LotusConnections-config folder hierarchy.|Correct any syntax errors in the file. If problems persist report this problem to Customer Support.|
|CLFRM0085E: There is something wrong with VenturaConfigHelper|The server could not retrieve or successfully parse a LotusConnections-config.xml configuration file from the LotusConnections-config folder hierarchy.|Correct any syntax errors in the file. If problems persist report this problem to Customer Support.|
|CLFRM0087E: The current database schema version for Communities is \{0\}, but the application expects \{1\}. Please update the schema version to match.|The database scripts to migrate the Communities database schema to the current version need to be run.|For more information, see [Updating databases](../migrate/t_update_connections_databases_for_v6.0_cr1.md).|
|CLFRM0088E: Error accessing database.|An error occurred while doing a query on a database.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0092E: There is no directory profile associated with this login name <login name\>|The wsadmin command could not be performed because the specified login name did not match any entries in the directory.|Correct the login name or use an email address to specify the user.|
|CLFRM0093E: Failed to delete bookmarks or feeds associated with deleted widget. <root cause\>|A bookmarks or feeds widget was deleted but the associated bookmarks and feed entries could not be deleted.|Report this problem to Customer Support.|
|CLFRM0095E: Error loading Communities Scheduler settings 'communities-config.xml'. Please check the validity of your HCL Connections Communities installation.|The server could not retrieve or successfully parse the communities-config.xml configuration file from the LotusConnections-config folder hierarchy.|Check the validity of the communities-config.xml file.|
|CLFRM0097E: Error running Communities LifecycleRetryQueuedEvents scheduled task|An error occurred while running the task that periodically retries failed life-cycle events.|Ensure that all HCL Connections applications are running.|
|CLFRM0106E: Communities eventLog scheduled cleanup task|The supplied task name was not recognized.|Task names of "LifecycleRetryQueuedEvents", "EventLogCleanup", "ForumPurgeTrash" must be used.|
|CLFRM0114E: JNDI naming exception caught. Connections Communities application has been incorrectly deployed.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0115E: Create task for task \{0\} failed to complete successfully.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0116E: Update task for task \{0\} failed to complete successfully.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0117E: Remove task for task \{0\} failed to complete successfully.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0119E: Create task for task \{0\} failed to complete successfully.|A scheduled task has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0120E: Task is not valid and cannot be fired.|A scheduled task has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0121E: Create task for task \{0\} failed to complete successfully.|A scheduled task has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0122E: Create task for task \{0\} failed to complete successfully.|The WebSphere Application Server scheduler was not available.|Report this problem to Customer Support.|
|CLFRM0123E: Update task for task \{0\} failed to complete successfully.|The WebSphere Application Server scheduler was not available.|Report this problem to Customer Support.|
|CLFRM0124E: Remove task for task \{0\} failed to complete successfully.|The WebSphere Application Server scheduler was not available.|Report this problem to Customer Support.|
|CLFRM0125E: Create task for task <task\> failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0126E: Update task for task \{0\} failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0127E: Create task for task \{0\} failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0128E: Update task for task \{0\} failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0129E: Create task for task \{0\} failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0130E: Update task for task \{0\} failed to complete successfully.|The interval settings for the <task\> task were not valid.|Correct the interval setting for the <task\> task in the communities-config.xml file.|
|CLFRM0131E: Create task for task \{0\} failed to complete successfully.|The notification sink for the scheduling EJB was invalid.|Report this problem to Customer Support.|
|CLFRM0132E: Update task for task \{0\} failed to complete successfully.|The notification sink for the scheduling EJB was invalid.|Report this problem to Customer Support.|
|CLFRM0133E: Create task for task \{0\} failed to complete successfully.|A notification exception occurred for the <task\> task.|Report this problem to Customer Support.|
|CLFRM0134E: Update task for task \{0\} failed to complete successfully.|A notification exception occurred for the <task\> task.|Report this problem to Customer Support.|
|CLFRM0135E: Remove task for task \{0\} failed to complete successfully.|A notification exception occurred for the <task\> task.|Report this problem to Customer Support.|
|CLFRM0137E: Create task for task <task\> failed to complete successfully.|A remote exception occurred while completing <task\> task.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0138E: Update task for task <task\> failed to complete successfully.|The task is pending and cannot be paused or resumed. See the system error log for more detail about the exception.|Report this problem to Customer Support.|
|CLFRM0139E: Remove task for task \{0\} failed to complete successfully.|A task pending exception occurred for the <task\> task.|Report this problem to Customer Support.|
|CLFRM0140E: Create task for task <task\> failed to complete successfully.|The scheduled task <task\> has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0141E: Update task for task \{0\} failed to complete successfully.|The scheduled task <task\> has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0142E: Remove task for task \{0\} failed to complete successfully.|The scheduled task <task\> has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0143E: Task named <task\> is not one of the configured tasks. Note that the task names in communities-config.xml cannot be changed.|The supplied task name <task\> was not recognized.|Task names of "LifecycleRetryQueuedEvents", "EventLogCleanup", "ForumPurgeTrash" must be used.|
|CLFRM0144E: An exception occurred updating member id \{0\}, display name: \{1\}. The external id has not been updated.|The attempt to update the member's external ID failed.|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0145E: There is a discarded login name <login name\> in the Communities member profile table for the member with display name <display name\>. This login name will be removed.|The communities database has the <login name\> for the person <display name\> but the directory no longer has that login name.|No action required. This message is informational. The Communities database is updated automatically to remove the previous login name.|
|CLFRM0146E: There is an inconsistent login name <login name\> in the Communities member profile table for the member with display name <display name\>. For this member two or more login names resolve to different profiles in the directory. The external id has not been updated.|The login name <login name\> is assigned to multiple people in the directory.|Update the directory to make login names unique, which is a prerequisite for HCL Connections.|
|CLFRM0151E: An error occurred while updating last login time-stamp for <user\>|A problem occurred while updating the last login time for the user.|Examine the additional error messages in the log.|
|CLFRM0152E: An unexpected exception has occurred. The command failed to complete successfully. See the system error log \(normally SystemErr.log\) for more detail about the exception.|An unexpected exception has occurred. The command failed to complete successfully. See the system error log \(normally SystemErr.log\) for more detail about the exception|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0153E: The specified task is not one of the known tasks. You cannot change the task name in communities-config.xml.|The communities-config.xml file contains an unrecognized task name.|Task names of "LifecycleRetryQueuedEvents", "EventLogCleanup", "ForumPurgeTrash" must be used.|
|CLFRM0154E: The specified task is not registered with the Communities scheduler.|The specified task is not registered with the Communities scheduler.|Task names of "LifecycleRetryQueuedEvents", "EventLogCleanup", "ForumPurgeTrash" must be used.|
|CLFRM0155E: JNDI naming exception caught. Connections Communities application has been incorrectly deployed. See the system error log \(normally SystemErr.log\) for more detail about the exception.|An error occurred while accessing the scheduling EJB.|Restart the Communities server. If problems persist, uninstall and reinstall the Communities application.|
|CLFRM0156E: The HCL Connections Communities scheduler is not available, probably the result of a deployment error. See the system error log \(normally SystemErr.log\) for more detail about the exception.|The HCL Connections Communities scheduler is not available, probably the result of a deployment error. See the system error log \(normally SystemErr.log\) for more detail about the exception|Examine the additional error messages in the log. If no straightforward fix can be found, contact Customer Support to report the incident.|
|CLFRM0158E: Task is not valid and status cannot be retrieved. See the system error log for more detail about the exception.|A scheduled task has task information that is not valid.|Report this problem to Customer Support.|
|CLFRM0159E: The Notification Sink object failed to fire, probably the result of a deployment error. See the system error log \(normally SystemErr.log\) for more detail about the exception.|The notification sink for the scheduling EJB was invalid.|Report this problem to Customer Support.|
|CLFRM0160E: The task is pending and cannot be paused or resumed. See the system error log for more detail about the exception.|A scheduled task is pending and cannot be paused or resumed. See the system error log for more detail about the exception.|Report this problem to Customer Support.|
|CLFRM0161E: The task is not valid and cannot be paused or resumed. See the system error log for more detail about the exception.|A scheduled task is invalid and cannot be paused or resumed. See the system error log for more detail about the exception.|Report this problem to Customer Support.|
|CLFRM0162E: Failure notifying remote widget applications of a community change: <root error message\>|The Communities app could not notify remote applications of a community change.|Report this problem to Customer Support.|
|CLFRM0163E: Failure retrieving values for a lifecycle event: <root error message\>|The Communities app could not notify remote applications of a community change.|Report this problem to Customer Support.|
|CLFRM0173E: Error inserting EventLogEntry: \{0\}|Event data could not be saved to the database.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0174E: Error updating EventLogEntry: \{0\}|Event data could not be saved to the database.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0175E: Error purging EventLogEntry: \{0\}|Old event data could not be deleted.|Not a problem in the short term - old event data will be purged when the task runs the next time. For a continual problem, report to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0176E: Error getting LogEntries: \{0\}|Event data could not be read from the database.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0177E: Failed to locate authenticated user, \{0\}, in user directory.|If WPI is enabled, the user could not be found in Profiles; the user might be missing, have an incorrect login name or be inactive in the Profiles database. If WPI is not enabled, the user could not be found in the LDAP directory.|Update Profiles or the LDAP directory to have a valid entry for the user.|
|CLFRM0178E: Cannot create community with duplicate handle: \{0\}|A non-unique value was entered for the community's web address.|Ensure the value that is entered for the community web address is unique.|
|CLFRM0179E: Cannot create community with handle that is a reserved word: \{0\}|A number of words in web addresses are reserved for potential future use by Communities.|Use a different word in the web address for the community.|
|CLFRM0180E: Cannot create community with handle that needs to be character-escaped in the URL: \{0\}|An attempt was made to update a community web address with a value that contains invalid characters.|Use only the letters A-Z, numbers 0-9, at sign \(@\), underscore \(\_\), period \(.\), and hyphen \(-\) characters.|
|CLFRM0181E: Cannot create community with handle that is in GUID format: \{0\}|Web addresses are not allowed to use a format of XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX, where X is 0 - 9 or a-f.|Use a different value for the web address of the community.|
|CLFRM0182E: The community handle is too long.|The value for the web address for the community is too long.|Use a shorter value for the web address of the community.|
|CLFRM0183E: Cannot locate the parent community from database by the community uuid: \{0\}.|A subcommunity refers to a parent community that cannot be found.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0184E: Cannot locate the community from database, by the handle hierarchy: \{0\}.|A community could not be located by the web address.|Correct the requested web address.|
|CLFRM0185E: The handle hierarchy, \{0\}, is too long.|A web address was requested that had handles for more than one parent community.|Report this problem to Customer Support. See the SystemOut.log file for more information about the error.|
|CLFRM0186E: The search service is unavailable at this time.|A search could not be performed because the search service is unavailable.|Examine the log files for errors specific to the search service and address any reported issues. Start the Search application.|
|CLFRM0192E: Cannot create the specified directory \{0\}.|An invalid directory path was passed as a parameter to a wsadmin command or Connections did not have rights to create the path.|Pass in a valid path to an existing directory.|
|CLFRM0195W: Unable to synchronize to latest group information. Will proceed with existing group information.|Communities tried to fetch the LDAP groups a user is a member of but the action failed. An LDAP server outage might cause this problem.|Try to restore the LDAP server and/or update LDAP credentials so that Connections can query the LDAP server.|
|CLFRM0196E: Cannot find widget with ID: **\{0\}**.|A request to set the community start page for a community failed because an invalid widget ID was specified.|Reissue the request with a valid widget ID.|
|CLFRM0197E: Failed to migrate community with ID: **\{0\}**.|A background task failed to update a community such that more UI elements such as Important Bookmarks are represented by widgets.|Contact support.|
|CLFRM0198E: Active Content Filter failed to process HTML field.|A request to update an HTML field, such as the community description failed, due to malformed HTML.|Reissue the request with valid HTML.|
|CLFRM0199E: Community \{0\} cannot be converted to allow visitors, it's not private.|An ATOM request failed since it tried to update a community to allow external users and be public or moderated.|Reissue the request such that the community is either private or does not allow external users.|

**Parent topic:**[Error message reference](../troubleshoot/c_error_codes.md)

**Related information**  


[Communities widget error messages](../troubleshoot/r_error_codes_widgets.md)

