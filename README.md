## RestAPI To SOAP Convert

This is an example project to demonstrate how to connect to SOAP web services from a Spring Boot component. It calls a basic SOAP service which converts numbers to words, exposing this function through a REST controller.

Image:
![ReQuest Process](https://github.com/CodeMechanix/RestAPI-To-SOAP-In-Spring-Boot/blob/main/images/Capture.PNG)

WSDL XML File: https://www.dataaccess.com/webservicesserver/NumberConversion.wso?wsdl

Thanks to Felipe. Credit goes to Felipe. 

## What I Learn:

> SOAP XML Communication Flow 

![SOAP Flow](https://github.com/CodeMechanix/RestAPI-To-SOAP-In-Spring-Boot/blob/main/images/SOAP1.png)

> Webservices :

The webservices are created to exchange the data between the two different system . Two types of webservices created are,
1. SOAP webservices
2. REST webservices

> SOAP Basics :

1. Simple Object access Protocol .
2. The communication happen between the consumer and provider in XML .
3. In SOAP ,the consumer should know about the provider interface and that contract information will be shared as WSDL.
4. If the service provider knows about the client ,the provider will give the WSDL directly to the client.
5. IF the service provider is not know about the consumer then the provider publish his service in the online registry UDDI.
6. UDDI -Universal Description discovery and Integration

> WSDL :

1. Webservice Definition language. All the information about the SOAP service can be found in the WSDL file.
2. This WSDL file has the below structure and to understand the Service contract information ,you should have clear idea about the WSDL structure.

![WSDL File](https://github.com/CodeMechanix/RestAPI-To-SOAP-In-Spring-Boot/blob/main/images/SOAP2.png)

![WSDL Tags](https://github.com/CodeMechanix/RestAPI-To-SOAP-In-Spring-Boot/blob/main/images/SOAP3.png)

1. Types - Data type definition
2. Message - Data communication between the client and provider defined here.
3. Operation - Abstract description of actions. For Each action ,you can pass the request and get response .
4. Port Type - Set of operation and combination of request and response communication
5. Binding - Defines the protocol and format specification for the operation (like GET,POST,HTTP)
6. Service -aggregates the set of related ports.

> Steps to Consume a SOAP service :

1. Create spring boot project and Get the WSDL from the provider .
2. Convert the WSDL to Stub
3. Understand the request ,response and the types ,operations using any tool like SOAP UI
4. Form the request object by mapping data and call the soap uri with marshal the java objects as XML
5. Receive the Response object and unmarshal it 

Content Credit Goes to theprogrammerguide.
