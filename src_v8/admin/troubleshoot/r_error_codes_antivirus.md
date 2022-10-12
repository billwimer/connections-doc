# Anti-virus error messages {#r_error_codes_antivirus .reference}

Use the codes included in the error messages generated by HCL Connections™ to identify problems with the Anti-Virus service plug-in and find their solutions.

## Anti-virus service plug-in errors { .section}

The following error messages are generated by the Anti-virus service plug-ins:

|Message|Cause|Solution|
|-------|-----|--------|
|CLFAQ0001E: Unable to access file \{0\}|The plug-in cannot find the file to scan.|Verify the file name and then try again.|
|CLFAQ0002E: Error raised communicating with virus scanner: \{0\}|The plug-in could not connect to the scanner. For example: my.scanner.com.|Verify that the scanner is running and the network connection is good.|
|CLFAQ0003E: Property \{0\} missing from scanner initialisation data|A required property, identified by \{0\}, is not in the <avFilter\> XML block of the configuration file.|Add the property to the to the <avFilter\> XML block in the LotusConnections-config.xml file.|
|CLFAQ0004E: ICAP error processing content: \{0\}|There was a problem processing the content of the ICAP header.|Make sure you are providing the appropriate content in the header.|
|CLFAQ0005E: Unknown Host: \{0\}|The code was unable to find the antivirus server.|First, check that the antivirus server is online and reachable by the Lotus® connections Server. Secondly, check the DNS server to ensure that the hostname/domain used for the antivirus server is pointing to the correct machine. Also ensure that the antivirus machine is running.|
|CLFAQ0006E: ICAP error null response|The antivirus server did not return any response at all.|Indicates a possible connection problem and/or anti-virus server problem. The virus scanner might have crashed, for example.|
|CLFAQ0007E: ICAP error first read timeout: \{0\}|Indicates that the anti-virus server is a bit slow or overloaded or there is some sort of network issue.|If you see this error once in a while, it is OK to ignore it. However, if the logger has a lot of timeouts and virus scanning fails, then there is a problem. In this case, check to make sure that the antivirus server is actually running and reachable by the Connections servers.|
|CLFAQ0008E: General error with connecting to a server: \{0\}|A generic error that is displayed when the code is unable to connect to the antivirus server due to some unexpected error.|First, check that the antivirus server is online and reachable by the Lotus connections Server. Secondly, check the DNS server to ensure that the hostname/domain used for the antivirus server is pointing to the correct machine. Also ensure that the antivirus machine is running.|
|CLFAQ0009E: ICAP error second read timeout: \{0\}|Indicates that the anti-virus server is a bit slow or overloaded or there is some sort of network issue.|If you see this error once in a while, it is OK to ignore it. However, if the logger has a lot of timeouts and virus scanning fails, then there is a problem. In this case, check to make sure that the antivirus server is actually running and reachable by the Connections servers.|
|CLFAQ0010E: ICAP error incomplete response: \{0\}|The antivirus server did return something, but the response was incomplete.|Check to make sure that the antivirus server is actually running and reachable by the Connections servers.|
|CLFAQ0011E: Unsupported connection type: \[tls\]|The current code does not support connecting to the antivirus scanner using TLS.|Disable TLS.|
|CLFAQ0012I: ICAP Headers: \{0\}|This informational message is provided for debugging, since the code can sometimes misinterpret the ICAP headers.|Use this message to secure a log of what the headers actually are so you can figure out what happened.|

**Parent topic:**[Error message reference](../troubleshoot/c_error_codes.md)
