# Web Services
Web services are client and server applications that communicate over the World Wide Web’s (WWW) HyperText Transfer Protocol (HTTP). As described by the World Wide Web Consortium (W3C), web services provide a standard means of interoperating between software applications running on a variety of platforms and frameworks. 

## Lay wo/man explanation
A web service is meant for code consumption / application consumption. Allows two different applications to talk to each other over the network. Web services can be written in any language. There are three key parts to a web service which are : 

* Machine to Machine Interaction

* Interoperable - Not platform dependent (Java to C#)

* Communication over a network

## Types of web services

* Soap (JAX-WS) Java API for XML Web Services
	- Uses a WSDL File (web service description language)

* RESTful web service  (JAX-RS)

## SOAP
Soap defines a specific xml request and response structure. It requires the creation of a soap envelope which consist of a soap Header and a Soap Body. 

 	* Header: consist of things like authorization & authentication
 	* Body: Consist the content of your request or response

### How Soap web services work?
 Transport: How the service is provided and consumed - Is it over the internet via http or is it over a Que(MQ)? 
 
 Service Definition: Often done via a wsdl

### What is a WSDL used for?
WSDL (Web service definition language) specifies an XML format for describing a service as a set of endpoints operating on messages. It defines your end point and much more.

In other words it contains the contract (XSD) to your web service that is shared with the consumers of the web service as an xml document. It contains the methods and arguments / return types that can be called. It's the way consumers of your web service know how they should structure their request.

### What is XML used for?
XML - used to exchange data between the client application and the web services. XML is mostly used in 3 ways

* Save and manipulate data

* Data exchange(has data & metadata) used for REST & SOAP 

* As a configuration file - pom.xml, web.xml, server.xml etc.

### What is an XSD (xml schema definition)?
XML Schema file is a contract between two apps. They use an xsd to define all the elements and attributes needed.



## DEMO - Spring boot project set up

Go to http://start.spring.io/
Select 2.0.0 Snapshot
Make sure Maven in selected in drop down
Enter reverse domain, choose artifact name and select Web Services ,JPA and H2 dependencies
Download the zipped file and extract it on your computer

### Download eclipse Java EE oxygen (on mac)
Accept the default workspace
Launch eclipse. 
Close the popup by clicking X at top left.
Go to File > Import and type Maven. 
Select Existing Maven Project
Browse to the spring.io project you created to select it via eclipse. Click Finish and wait...
To run it..right click and select Run as Java Application.

### Code available on Github
https://github.com/MikailaAkeredolu/java-soap-api/tree/master/src/main/java/com/mikaila/courses


