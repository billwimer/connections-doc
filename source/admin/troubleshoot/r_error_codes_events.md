# Events service error messages {#r_error_codes_events .reference}

Use the codes included in the error messages generated by HCL Connections™ to identify problems related to the events service of the Home page application and find solutions to those problems.

## Events error messages { .section}

The following events service error messages are generated by Connections:

|Message|Cause|Solution|
|-------|-----|--------|
|CLFWY0001E: The Source field was null or empty when creating a new event record. The Source field must contain a valid value.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0005E: An attempt was made to register a null event consumer for the Source \{0\}|This is an internal error.|Contact HCL Support.|
|CLFWY0006E: The Event Name field was null or empty when creating a new event record. The Event Name field must contain a value.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0007E: An invalid JSON string was provided|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0008E: The Source field value \{0\} is not a known, valid source. The event record cannot be created.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0009E: The ACL Feed URL field was null or empty when creating a new event record. The ACL Feed URL field must contain a value.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0011E: The Event Name field was null or empty when sending an event record for source \{0\}. The Event Name field must be supplied before the event is sent!|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0014E: The Container ID field was null or empty when creating a new event record. The Container ID field must contain a value.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0015E: The input set to add to was provided as null.. A valid set must be provided.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0017E: The Source field was null or empty when registering a new event record consumer. Events will not be sent to the consumer.|This is an internal error.|Contact HCL Support.|
|CLFWY0019E: The following class could not be instantiated as an event transport: \{0\} but was specified as the default transport. Events cannot be propagated to the News Repository.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0020E: The following class is not a valid event transport: \{0\} but was specified as the default transport. Events cannot be propagated to the News Repository.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0022E: A JMS Exception occurred when consuming an event record. The event record will be retried and eventually be placed on the system exception queue if unsuccessful.|An event could not be consumed from the JMS queue used by the event infrastructure. This will result in news stories not displaying in Home Page in some circumstances.|Check the configuration of JMS resources in WebSphere®. Also check that the Service Integration Bus is configured to allow access to the user defined in the connectionsAdmin authentication alias. The nested exception provides more details.|
|CLFWY0024E: JMS QueueConnectionFactory for sending the ACL event record with ID \{0\} from source \{1\} were not available. QueueConnectionFactory may not be defined.|JMS resources required by the event infrastructure could not be looked up. This will result in news stories not displaying in Home Page in some circumstances.|Check the HCL Connections installer log for any errors during install. Also check the WebSphere Application Server JMS Resources to check if any QueueConnectionFactory objects are defined. If not, the installer failed to create them. Attempt a reinstall or contact HCL Support.|
|CLFWY0025E: JMS QueueConnectionFactory for sending the event record with ID \{0\} from source \{1\} were not available. QueueConnectionFactory may not be defined.|JMS resources required by the event infrastructure could not be looked up. This will result in news stories not displaying in Home Page in some circumstances.|Check the HCL Connections installer log for any errors during install. Also check the WebSphere Application Server JMS Resources to check if any QueueConnectionFactory objects are defined. If not, the installer failed to create them. Attempt a reinstall or contact HCL Support.|
|CLFWY0026E: A JMS exception occurred when attempting to sent the event record ID \{0\} from source \{1\}. Check the nested exception for more details.|An event could not be propagated onto the JMS queue used by the event infrastructure. This will result in news stories not displaying in Home Page in some circumstances.|Check the configuration of JMS resources in WebSphere Application Server. Also check that the Service Integration Bus is configured to allow access to the user defined in the connectionsAdmin authentication alias. The nested exception provides more details.|
|CLFWY0027E: A JMS exception occurred when attempting to sent the ACL event record ID \{0\} from source \{1\}. Check the nested exception for more details.|An event could not be propagated onto the JMS queue used by the event infrastructure. This will result in news stories not displaying in Home Page in some circumstances.|Check the configuration of JMS resources in WebSphere Application Server. Also check that the Service Integration Bus is configured to allow access to the user defined in the connectionsAdmin authentication alias. The nested exception provides more details.|
|CLFWY0028E: An EJB instance for the Event Record Transport implementation could not be created. Check nested exception for more details.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Check the nested exception for any details, and resolve any obvious configuration issue. Contact HCL Support.|
|CLFWY0029E: The EJB Home for the Event Record Transport implementation could not be looked up. Check nested exception for more details.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Check the nested exception for any details, and resolve any obvious configuration issue. Contact HCL Support.|
|CLFWY0030E: An error occurred when creating a JMS message due to an invalid session. The event will not be sent. Restarting the application may resolve this issue.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|This error may happen due to temporary configuration of infrastructure reasons. Restart the application. If this error persists or requires regular restarts, contact HCL support.|
|CLFWY0031E: An unexpected implementation class for an ACL event record was received. The event will not be sent. The class was \{0\}|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0032E: A JMS message could not be created for the event record ID \{0\} from source \{1\}. The event will not be sent. Check the nested exception for more details.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0033E: An unexpected implementation class for an event record was received. The event will not be sent. The class was \{0\}|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0037E: An error occurred while fetching the News Repository EJB. Check the logs for more details.|The News Repository EJB could not be looked up. This will result in news stories not displaying on the Home Page Updates page.|The nested exception will contain exact details of the error. Refer to the error message for the nested exception.|
|CLFWY0038E: Impossible to get the bootstrap and port information for the remote EJB from LotusConnections-Config.xml|The LotusConnections-config.xml file could not be read to obtain the bootstrapHost and bootstrapPort values for the News service.|Validate that LotusConnections-config.xml is correct and that the bootstrapHost defined for the News service points to the application server running News, and that the bootstrapPort points to the correct Bootstrap Port for that server. Fix the file and restart the application.|
|CLFWY0039E: The JMS QueueConnectionFactory or Queue could not be looked up. Check the QCF and Queue is defined in WebSphere and bound to the application. Check the nested exception for more details.|JMS resources required by the event infrastructure could not be looked up. This will result in news stories not displaying in Home Page in some circumstances.|Check the HCL Connections installer log for any errors during install. Also check the WebSphere Application Server JMS Resources to check if any QueueConnectionFactory and Queue objects are defined. If not, the installer failed to create them. Attempt a reinstall or contact HCL Support.|
|LFWY0056E: The scheduled task service mbean needed to run tasks is not registered for application ''\{0\}''. Verify that the component is running. If it is there is an internal error. Call HCL Customer Support in this case.| | |
|CLFWY0057E: The task named ''\{0\}'' is not one of the configured tasks. Possibly a task name accidently was changed in the component configuration file. If not, Call HCL Customer Support.|The task you specified cannot be found.|Determine whether a task name was changed in the application's configuration file. If that is not the cause, contact HCL support.|
|LFWY0058E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar period is invalid. Call HCL Customer Support.|The calendar period is invalid.|Determine whether a calendar period is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0059E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: The scheduler is not available. Call HCL Customer Support.|The scheduler is not available.|Try restarting Websphere Application Server. If this fails, contact HCL support.|
|CLFWY0060E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: The notification sink is invalid. Call HCL Customer Support.| | |
|CLFWY0061E: Local task ''\{0\}'' failed to start on the cluster servers for reason previously given.| | |
|CLFWY0062E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: A notification exception occurred. Call HCL Customer Support.| | |
|CLFWY0063E: Remove task for task ''\{0\}'' failed to complete successfully. Internal error: A JNDI naming exception occurred. Call HCL Customer Support.| | |
|CLFWY0064E: Remove task for task ''\{0\}'' failed to complete successfully. Internal error: The scheduler is not available. Call HCL Customer Support.|The scheduler is not available.|Try restarting Websphere Application Server. If this fails, contact HCL support.|
|CLFWY0065E: Task ''\{0\}'' failed to start or complete normally. Possibly the task class is incorrect. Inspect the task configuration settings.| | |
|CLFWY0066E: Remove task for task ''\{0\}'' failed to complete successfully. Internal error: the created task is not valid. Call HCL Customer Support.| | |
|CLFWY0067E: An error occurred while calling remote method for task \{0\}. Internal error. Call HCL Customer Support.| | |
|CLFWY0068E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: the created task is not valid. Verify the task configuration settings, and then call HCL Customer Support.| |Verify the task configuration settings, and then contact HCL support.|
|CLFWY0069E: Internal error: The default user calendar is not valid. Call HCL Customer Support.| |Contact HCL support.|
|CLFWY0070E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar specifier is invalid. Call HCL Customer Support.|The calendar specifier is invalid.|Determine whether a calendar specifier is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0071E: The task \{0\} is not valid and cannot be accessed. Internal error. Call HCL Customer Support.| | |
|CLFWY0072E: The local scheduled task ''\{0\}'' failed to start due to failure to get the connectionsAdmin alias or password. Check the Connections Admin alias''s. If they are ok this is an internal error; call HCL Customer Support.| | |
|CLFWY0073E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: The notification sink is invalid. Call HCL Customer Support.| | |
|CLFWY0075E: Error loading scheduler settings for component with config id \{0\}. Call HCL Customer Support. Please check the validity of your HCL Connections installation configuration files. Then call HCL Customer Support.| | |
|CLFWY0076E: Task configuration is not available for task ''\{0\}''. The application may not have started properly. Try restarting the application. If this fails, call HCL Customer Support.| | |
|CLFWY0077E: The local scheduled task ''\{0\}'' failed to start due to failure to get the deployment manager admin client. Verify that the dmgr is started.| | |
|CLFWY0078E: The local scheduled task ''\{0\}'' failed to start due to failure to get the deployment manager node name. Internal error. Call HCL Customer Support.| | |
|CLFWY0079E: Internal error: A JNDI naming exception was caught. \{0\} Call HCL Customer Support.| | |
|CLFWY0080E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: A JNDI naming exception occurred. Call HCL Customer Support.| |Contact HCL support.|
|CLFWY0081E: Internal error: The calendar specifier is not valid. Call HCL Customer Support.|The calendar specifier is invalid.|Determine whether a calendar specifier is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0082E: Update task for task ''\{0\}'' failed to complete successfully. The task is pending. Try again later.|The task is pending.|Try again later.|
|CLFWY0083E: The local scheduled task ''\{0\}'' failed to start due to failure to get the deployment manager host name or SOAP port. Internal error. Call HCL Customer Support.| | |
|CLFWY0084E: Internal error: The Notification Sink object failed to fire. Call HCL Customer Support.| |Contact HCL support.|
|CLFWY0085E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: A notification exception occurred. Call HCL Customer Support.| | |
|CLFWY0086E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar is invalid. Call HCL Customer Support.|The calendar is invalid.|Determine whether a calendar is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0087E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: A JNDI naming exception occurred. Call HCL Customer Support.| |Contact HCL support.|
|CLFWY0088E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: A remote exception occurred. Call HCL Customer Support.| | |
|CLFWY0089E: The local scheduled task ''\{0\}'' failed to start due to failure to get the connectionsAdmin alias or password, or the deployment manager host name or SOAP port. Internal error. Call HCL Customer Support.| | |
|CLFWY0091E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar specifier is invalid. Call HCL Customer Support.|The calendar specifier is invalid.|Determine whether a calendar specifier is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0092E: For task \{0\}, the specified ''interval='' attribute is not a valid ''cron'' schedule. Correct the cron string.|An invalid value is being used as the cron string for the interval attribute.|Correct the syntax of the cron string.|
|CLFWY0093E: The HCL Connections component for task ''\{0\}'' scheduler is not available. The component appears to be stopped.|The application is not available.|Make sure the application is started. If not, start it. If that is not the cause, contact HCL support.|
|CLFWY0094E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: the created TaskInfo object is not valid. Verify the task configuration settings, and then call HCL Customer Support.|The TaskInfo object is invalid.|Verify the task configuration settings, and then contact HCL support.|
|CLFWY0095E: The task named ''\{0\}'' with an unknown type of ''\{1\}'' has fired, and is being ignored. Inspect the task configuration settings.|You might have inadvertently changes the task type in the configuration file.|Correct the configuration settings.|
|CLFWY0096E: Internal error: The scheduled tasks will not fire. Call HCL Customer Support.| | |
|CLFWY0097E: Remove task for task ''\{0\}'' failed to complete successfully. The task is pending. Try again later.|The task is pending.|Try again later.|
|CLFWY0098E: The task \{0\} is already pending.|The task you are trying to schedule is already scheduled.|No further action is required.|
|CLFWY0099E: The local scheduled task ''\{0\}'' failed to start, could not invoke mbean on remote server in cluster. Internal error. Call HCL Customer Support.| | |
|CLFWY0101E: Internal error: This is probably due to a deployment error. Call HCL Customer Support.| | |
|CLFWY0102E: Remove task for task ''\{0\}'' failed to complete successfully. Internal error: A notification exception occurred. Call HCL Customer Support.| | |
|CLFWY0103E: The local scheduled task ''\{0\}'' failed to start due to failure to get the list of remote servers. Internal error. Call HCL Customer Support.| | |
|CLFWY0104E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: A remote exception occurred. Call HCL Customer Support.| | |
|CLFWY0105E: Update task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar is invalid. Call HCL Customer Support.|The calendar is invalid.|Determine whether a calendar is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0106E: Update task for task ''\{0\}'' failed to complete successfully. The created task is not valid. Verify the task configuration settings, and then call HCL Customer Support.|The created task is not valid.|Verify the task configuration settings, and then contact HCL support.|
|CLFWY0107E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: The calendar period is invalid. Call HCL Customer Support.|The calendar period is invalid.|Determine whether a calendar period is defined correctly in the application's configuration file. If that is not the cause, contact HCL support.|
|CLFWY0108E: Create task for task ''\{0\}'' failed to complete successfully. Internal error: The scheduler is not available. Call HCL Customer Support.|The scheduler is not available.|Try restarting Websphere Application Server. If this fails, contact HCL support.|
|CLFWY0109E: Task ''\{0\}'' failed to start. The Mbean name is ''\{1\}''. Possibly the task mbean or method name \(''\{2\}''\) argument is incorrect.| | |
|CLFWY0110E: Internal error: The scheduler is not available. Try restarting Websphere. If this fails, call HCL Customer Support.|The scheduler is not available.|Try restarting Websphere Application Server. If this fails, contact HCL support.|
|CLFWY0112E: Internal Error: The specified notification sink class is not valid. Call HCL Customer Support.| | |
|CLFWY0113E: Internal error: JNDI naming exception caught. Connections component has been incorrectly deployed. Call HCL Customer Support|The application was incorrectly deployed.|Contact HCL support.|
|CLFWY0135E: The default event enable implementation class \{0\} does not implement the EventEnable interface|Internal error. Events may not be generated and the HCL Connections Home Page Updates page may be empty as a result.|Contact HCL support.|
|CLFWY0136E: Could not instantiate an instance of the default event enable class \{0\}|Internal error. Events may not be generated and the HCL Connections Home Page Updates page may be empty as a result.|Contact HCL support.|
|CLFWY0138E: The source, type, scope and name of an event must always be set.|This is an internal error. This will result in news stories not displaying in Home Page in some circumstances.|Contact HCL Support.|
|CLFWY0140E: The following class is not a valid async event invoker: \{0\} but was specified as the default invoker. Events cannot be propagated asynchronously.|Internal error. Events may not be generated and the HCL Connections Home Page Updates page may be empty as a result.|Contact HCL support.|
|CLFWY0141E: The following class could not be instantiated as an async event invoker: \{0\} but was specified as the default transport. Events cannot be propagated asynchronously.|Internal error. Events may not be generated and the HCL Connections Home Page Updates page may be empty as a result.|Contact HCL support.|
|CLFWY0143E: An exception occurred when trying to send the event \{0\} with ID \{1\} asynchronously. No asynchronous event consumers will receive this event. Check nested exception for more details.|An asynchronous event could not be sent. This will result in data not appearing in the HCL Connections Home Page Updates page, or being available to third party event consumers.|Check the nested exception for more details. Check that a CLFWX0186I message is generated when the News application starts up. Contact HCL support.|
|CLFWY0144E: An invalid JSON string was provided: \{0\}|Internal error. As a result of this error, an event cannot be sent.|Contact HCL support.|
|CLFWY0145E: The input set to add to was provided as null.. A valid set must be provided.|Internal error. As a result of this error, an event cannot be sent.|Contact HCL support.|
|CLFWY0146E: An EJB instance for the event implementation could not be created. Check nested exception for more details.|Internal error. Events may not be sent.|Restart the application. If the problem persists, contact HCL support.|
|CLFWY0147E: The EJB Home for the event implementation could not be looked up. Check nested exception for more details.|Internal error. Events may not be sent.|Restart the application. If the problem persists, contact HCL support.|
|CLFWY0148E: Could not obtain an event connection|Internal error. Events may not be sent.|Restart the application. If the problem persists, contact HCL support.|
|CLFWY0149E: An outgoing event due to be consumed by News could not be augmented. It will not be consumed by News.|An event could not be augmented for delivery to the News application.|This is an internal error. Contact HCL support.|
|CLFWY0150E: Could not obtain the event topic connection factory|Internal error. Events may not be sent.|Check the HCL Connections install log for any errors. Check the nested exception for any errors, then contact HCL support.|
|CLFWY0151E: A JMS Exception occurred when publishing an event with ID \{0\} to topic \{1\}|Internal error. Events may not be sent.|If the exception only happens once, it could be a temporary connectivity issue. Otherwise restart the application. If the problem persists, contact HCL support.|
|CLFWY0152E: An outgoing event due to be consumed by Communities could not be augmented. It will not be consumed by Communities.|An event could not be augmented for delivery to the Communities application.|This is an internal error. Contact HCL support.|
|CLFWY0153E: Could not create a JMS MapMessage|Internal error. Events may not be sent.|Contact HCL support.|
|CLFWY0154E: The Map object does not contain all mandatory event data: ID, Timestamp, Source, Type, Scope, Name|Internal error. As a result of this error, an event cannot be sent.|Contact HCL support.|
|CLFWY0155E: The Map object provided is not an event map, or is not the correct version.|Internal error. As a result of this error, an event cannot be sent.|Contact HCL support.|
|CLFWY0156E: The events-config.xml configuration appears not to be an XML configuration file.|The events-config.xml configuration file is not a valid XML file. This means that registered event handlers will not be invoked.|Examine the events-config.xml file and fix any errors.|
|CLFWY0159E: events-config.xml failed validation. Check the file and correct any XML errors.|The events-config.xml file contains invalid XML that does not match the schema in events-config.xsd. This means that registered event handlers will not be invoked.|Examine the events-config.xml file and fix any errors.|
|CLFWY0161E: An exception occurred when trying to load events-config.xml. Event handlers will not be run.|The events-config.xml configuration file could not be loaded. This means that registered event handlers will not be invoked.|Examine any nested exception for the cause. Ensure the events-config.xml file exists in the LotusConnections-config directory and fix any errors.|
|CLFWY0170E: An exception occurred when invoking the event handler named: \{0\} with the event: \{1\}|The named event handler could not be invoked for the named event.|Check the nested exception for more details and resolve any errors.|
|CLFWY0171E: Could not load event handler configuration. Registered event handlers will not run. Check nested exception for more details.|The event handler configuration could not be loaded. This means that registered event handlers will not be invoked.|Examine the nested exception for the cause and resolve any problems.|
|CLFWY0172E: The event handler named \{0\} could not be created because the handler class \{1\} could not be instantiated. The handler will not run.|The class for the named event handler could not be instantiated. This handler will not be run.|Examine any nested exception for more details. Ensure the handler class provides a default public constructor.|
|CLFWY0173E: Could not set the property named \{1\} on handler \{0\}. The property value may not be mappable to the property type. This handler may not initialize correctly.|The named property of the named event handler could not be set. This may cause the handler to fail to initialize.|Check the handler definition in events-config.xml and check that the defined properties match the properties of the handler class exactly.|
|CLFWY0174E: The event handler named \{0\} could not be created because the handler class \{1\} could not be loaded. The handler will not run.|The class for the named event handler could not be loaded. This handler will not be run.|Ensure the event handler Jar is defined in a shared library, and that the shared library is referenced by all HCL Connections applications in the WebSphere Application Server administrative console.|
|CLFWY0175E: The event handler named \{0\} could not be created because the handler class \{1\} could not be accessed. The handler will not run.|The class for the named event handler could not be accessed. This handler will not be run.|Examine any nested exception for more details and resolve any problems.|
|CLFWY0176E: The event handler named \{0\} did not initialize correctly. Check the handler configuration in events-config.xml. The handler will not run.|The named event handler failed to initialize correctly. This handler will not be run.|Examine any nested exception for more details. Check that all required properties of the handler are defined in events-config.xml.|
|CLFWY0177E: The event handler named \{0\} is not a valid event handler class: \{1\} The handler will not run.|The named event handler is implemented by a class which is not a valid event handler class. This handler will not be run.|Examine the configuration of the event handler in events-config.xml and inspect the source of the event handler class to ensure it correctly implements the Event SPI.|
|CLFWY0178E: An outgoing command due to be consumed by other applications could not be augmented. It may not be consumed by other applications.|A platform command event could not be augmented for delivery to command consumers.|This is an internal error. Contact HCL support.|
|CLFWY0179E: Could not load the set of event names to be consumed by river of news. Events may not display in the river of news.|The set of events that need to be consumed by the News application could not be loaded. This will result in no events being sent to News, and the HCL Connections Home Page Updates page will be empty as a result.|If you have made any customization changes to the JAR file lc.events.internal.jar then revert these changes, otherwise contact HCL support.|
|CLFWY0183E: The invocation of the asynchronous event point for the event named \{0\} with ID \{1\} failed. The event was not sent.|An asynchronous event could not be sent. This will result in data not appearing in the HCL Connections Home Page Updates page, or being available to third-party event consumers.|Check the nested exception for more details. Check that a CLFWX0186I message is generated when the News application starts up. Contact HCL support.|
|CLFWY0185E: A null internal event subscriber object was supplied.|Internal error.|Contact HCL support.|
|CLFWY0187E: The invocation of the synchronous post-commit event point for the event named \{0\} with ID \{1\} failed. The event was not sent.|A synchronous event could not be sent.|Check the nested exception for more details. Contact HCL support.|
|CLFWY0188E: The invocation of the synchronous pre-commit event point for the event named \{0\} with ID \{1\} failed. The event was not sent.|A synchronous event could not be sent.|Check the nested exception for more details. Contact HCL support.|
|CLFWY0190E: A JMS exception occurred when consuming an event in an internal consumer. Check nested exception for more details.|Internal error. An event cannot be consumed.|If the exception only happens once, it could be a temporary connectivity issue. Otherwise restart the application. If the problem persists, contact HCL support.|
|CLFWY0192E: task config error, task name is the empty string. Task is skipped. Inspect the task config.| | |
|CLFWY0193E: task config error, for task name ''\{0\}'' mbean method name cannot be empty due to type. Task is skipped. Inspect the task config.| | |
|CLFWY0194E: task config error, for task name ''\{0\}'' task type not valid. Task is skipped. Inspect the task config.| | |
|CLFWY0195E: task config error, task name \(\{0\}\) enabled not true or false. Task is skipped. Inspect the task config.| | |
|CLFWY0196E: task config error, for task name ''\{0\}'' startby cannot contain punctuation characters. Task is skipped. Inspect the task config.| | |
|CLFWY0197E: task config error, task name \(\{0\}\) defined more than once. Duplicates skipped. Task is skipped. Inspect the task config.| | |
|CLFWY0198E: task config error, for task name ''\{0\}'' scope value not valid. Task is skipped. Inspect the task config.| | |
|CLFWY0199E: task config error, for task name ''\{0\}'' interval cannot contain punctuation characters. Task is skipped. Inspect the task config.| | |
|CLFWY0200E: task config error, task config is out of date. Task is skipped. Inspect the task config.| | |
|CLFWY0201E: task config error, task name \(\{0\}\) cannot contain punctuation characters. Task is skipped. Inspect the task config.| | |
|CLFWY0202E: The event handler named \{0\} threw an exception when handling an event. Check nested exception for more details.|The named event handler threw an exception when handling an event.|Examine any nested exception for more details. Check any logs that the event handler keeps.|
|CLFWY0203E: The event handler named \{0\} encountered an initialization exception and will not receive events. It may be mis-configured. Check nested exception for more details.|The named event handler failed to initialize correctly. This handler will not be run.|Examine any nested exception for more details. Check that all required properties of the handler are defined in events-config.xml.|
|CLFWY0204E: Error when lookup with asynchronous event handler work manager. Check nested exception for more details.|Could not look up the asynchronous event handler work manager in the News application. Asynchronous event handlers may not work.|Check the nested exception for more details and check the HCL Connections install log for any errors when installing the News application.|
|CLFWY0205E: Error creating asynchronous subscriber for event handler named \{0\} and subscription \{1\}. This handler will not receive events.|Could not register a subscription for the named asynchronous event handler. This handler may not receive all events it expects to.|Check the subscription defined for the handler in events-config.xml and correct any issue.|
|CLFWY0206E: Error when reading event handler configuration in events-config.xml whilst creating asynchronous event handlers. Check nested exception for more information.|Could not configure an asynchronous event handler due to a configuration issue in events-config.xml.|Check the nested exception for more details. Check events-config.xml and correct any issues.|
|CLFWY0222E: An outgoing news cleanup event could not be augmented.|A deletion event could not be augmented for delivery. Any existing updates for the item the event represents will not be removed from the HCL Connections Home Page Updates page.|This is an internal error. Contact HCL support.|
|CLFWY0233E: The event handler named \{0\} encountered an unexpected exception when handling an event. Check nested exception for more details.|The named event handler threw an unexpected exception when handling an event.|Examine any nested exception for more details. Check any logs that the event handler keeps.|
|CLFWY0234E: Cannot build a path to the filesystem using a base location: \{0\} and relative path: \{1\}|Internal error. A path location in an event cannot be resolved to an absolute path. Event consumers may not work correctly if they depend on this.|Check the base location in the error message and then check the value of the corresponding WebSphere Application Server variable.|
|CLFWY0235E: A deferred event with ID \{0\} could not be retrieved. This event will not be sent.|Internal error. Events may not be sent.|Contact HCL support.|
|CLFWY0236E: A deferred event is not of type MapMessage.|Internal error. Events may not be sent.|Contact HCL support.|
|CLFWY0237E: A JMS exception occurred when processing deferred event with ID \{0\}. This event will not be sent. Check nested exception for more details.|Internal error. Events may not be sent.|If the exception only happens once, it could be a temporary connectivity issue. Otherwise restart the application. If the problem persists, contact HCL support.|
|CLFWY0238E: A JMS Exception occurred when publishing a deferred event with ID \{0\} to temporary topic \{1\}|Internal error. Events may not be sent.|If the exception only happens once, it could be a temporary connectivity issue. Otherwise restart the application. If the problem persists, contact HCL support.|
|CLFWY0267E: An outgoing notification event could not be augmented. The notification may not be successful.|A notification event could not be augmented for delivery. This notification will not be processed and recipients will not get emails.|This is an internal error. Contact HCL support.|
|CLFWY\#\#\#\#E: Could not load event content store location for feature \{0\}. Check events-config.xml for errors.|Internal error. Could not retrieve the base file system location of the content store for the named application.|Check the definition of the base location variable in events-config.xml and then check that the corresponding WebSphere Application Server variable has a valid value.|

**Parent topic:**[Error message reference](../troubleshoot/c_error_codes.md)
