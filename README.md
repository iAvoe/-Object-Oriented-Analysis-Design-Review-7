# Object-Oriented-Analysis-Design-Review-7
## Defining the System Architecture

### 6-Phase SDLC index

1. Identify problem
2. Plan and monitor project
3. Analyze details
4. **Design components**
5. Build / Develop solution
6. Deploy / Implement solution

### Anatomy of Modern Information Systems

#### Computing Devices

**Server**
- Manages shared resources
- Enables users & other computers to access resources

**PC / Clients**
- Desktops, laptops, tablets, phones

**Server Farm**
- A cluster of computing, storaging servers under high use

#### Networks

**Computer network**
- hardware, software to transmit media

**Internet backbone / Internetwork**
- High-capacity with high-bandwidth trunk lines and large high-speed computers
- Owned by governments and telecom companies

**Local area network (LAN)**
- Small network for a single site

**World Wide Web (WWW)**
- All the interconnected resources accessed through the Internet

**Uniform Resource Locator (URL)**
- The identifier for the Web to locate a particular resource

**Hyperlink**
- The URL of a resource embedded within another resource
- Protocol header: `ftp://`, `http://` 
- Server hostname or address: `www.amazon.com`
- Resource path & name: `/archive/?id=100`

#### Software

**Application software**
- Programs that perform work for/from users
- Can be web based, or locally installed
- A client on PC

**APP (mobile phone)**
- A custom program usually for a laptop or smartphone
- A client on phones

**System Software**
- Behind the scene software
- Works as glue to hold everything together
- Operating System
- Web server application
- Database system

**Web-Based Application**
- Software or app accessible through web browser
- Available for all devices with internet browser

**Embedded Software**
- Apps or functions embedded within another app

#### Protocols

A set of languages & rules to ensure communication and data exchange

**Network protocols**

Virtual Private Network (VPN)
  - A private network through internet

HTML (hypertext markup language)
  - Protocol for the structure and content of a Web page

XML (extensible markup language)
  - An extensions of H T M L that enables defining semantics of tags

HTTP (hypertext transfer protocol)
  - Defines format and content for transfer of Web documents

HTTPS (hypertext transfer protocol secure)
  - Encrypted & secure http transfers

-----

### Architectural Concepts

**Software as a Service (SaaS)**
- No software is installed on the user’s device
- Application services is accessed remotely
- User data is isolated and stored on common servers

**Web service**
- Software function that is executed with Web standards
- Access via URL
- Inputs sent via the URL
- Executes remotely
- Data returned within a Web page

#### Distributed Architectures

- Technology architecture
- Computers, network computers and hardware, and system software
- Application architecture
- The software programs and their configuration

##### Client/Server architecture
- Design part of the application on a server, and part on the client
- The client requests data from server, the server responds

##### 3-layer architecture
- Client/server architecture with application divided into view layer, logic layer, and data layer
- View/Presentation layer: the user interface
- Logic/Model layer: programmed business logic to implement the functions
- Data/Database layer: the functions to access the data
- Allows easier developing, testing, upgrading, and scaling
  - Allows fault separation
- Allows for easier collaboration by allowing team to split role to work on different parts

1. The user initiates request from view layer
2. View layer passes formatted request commandline to logic/model layer
3. Logic/model layer may retrieve data from data layer
4. Logic/model layer reponds answer to view layer
5. View layer formats the response, and present to user

**Business logic layer**
- Sits between the presentation and data access layers
- Encapsulates the logic necessary to implement use cases & business processes
- The primary responsibilities include:
  - Processing user inputs from the presentation layer
  - Applying business rules, performing computations
  - Generating appropriate responses
- Does not concern with how data is stored or retrieved

-----

### Interoperability

The ability of an application to interact with other software

Important characteristic in current development projects:
  - Understand the environment
  - Reuse software existing components (purchased or in-house)
  - Build components considering interoperability
  - Combine all components into a solution system

**Location Diagrams** (in system design or architecture)
- Identify geographical placement of hardware, software, and users
  - i.e., Retail stores, warehouses and manfacturing plants across a country
- A visual representation of the physical or logical distribution of components
- Provides an overview of the various components
- Provides an overview of component interconnections across different locations or environments.

-----

### Architectural Diagrams

**Network Diagrams**
- How the application software is deployed

**Deployment Diagrams**
- How the components of a network are interconnected
- 3-layer design with user components grouped by user functions

-----

### Describing the Environment

Providing a comprehensive understanding of the context in which the system will operate. 

Includes various factors:
- Physical infrastructure
- Technological landscape
- Organizational policies
- User demographics
- Any other external influences that may impact system design / operation
- Designing Application Components

-----

### Quizzes

#### Technology Architectures

The set of computing hardware, network hardware and system software used by an organization is called the _________.​
- Technology architecture

A method of organizing software applications so that the data and core processing is in a central location and access to that core is distributed on user's computing devices is called ________.​
- Client/server architecture

Amazon.com is a good example of what kind of architecture? 
- 3-Layer Architecture

##### Distributed Architecture

Which of the following are examples of distributed architectures?
- three-layer architecture
- client/server architecture

###### Distributed Arch: 3-Layer Architecture

A software architecture that divides an application into view, business logic, and data is called a(n) ________.​
- Three-layer architecture

A three-layer architecture requires at least three computers to be implemented correctly.
- False

In a three-layer architecture, what are the three layers?
- View layer
- Business logic layer
- Data layer

In a three-layer architecture, the application server would be part of which layer? 
- Business logic layer


-----

#### Core Process 4: Design

Describing the environment is one of the detailed activities of core process 4: Design system components.​
- True
- Describe the environment
- Design the user interface
- Design application components

Which of the following is NOT one of the activities of Core Process 4: Design system components?​
- Design security and integrity controls

-----

#### Describing the Environment

The activity of Describing the Environment consists of what two key elements?​
- External systems and technology architecture

What is a computer that manages shared resources for access across a network called?​
- A server computer

The Internet can be thought of as the network of networks.​
- True

In a client/server configuration the term "server" refers to the central computer equipment that houses the core resources.​
- False

What does XML stand for?
- Extensible Markup Language

A personal computing device includes all of the following except:
- Router

##### Environment: Software

A toolbar might be considered an example of what?
- Embedded Software

An approach to implementing a software application where little or no software is installed and local computers, where the data is isolated between organizations a service computer is called _______.​
- Software as a service

System software usually refers to what kind of software?​
- Operating systems and web servers

##### Environment: Web Service

A function or service that is called from a Web application to another Web application is called a(n) ________.​
- Web service

A set of languages, rules and procedures to facilitate data exchange between among hardware and software components is called a(n):
- Protocol

What are the characteristics of a Web service?
- Does not execute on the calling applications computer
- Returns results encoded as a Web page
- Is called via a URL

Web-based application is software with the following characteristics: 
- Uses a browser and web-server

When a URL of a Web resource is embedded within a Web page, it is called a(n):
- Hyperlink

Given the following URL, what is the correct description of the portion shown in bold? http://**www.barnesandnoble.com**/u/books-best selling-books/379003057
- The server name

The Internet and the WWW are synonyms.​
- False

Which of the following is not a valid Web protocol?​
- VPN

What is the latest version of HTML?
- HTML 5

What is the difference between HTTP and HTTPS?
- Amazon uses HTTPS for credit encryption

When we use the term the Web what is the correct definition?
- The set of world wide resources that are available over the Internet

-----

#### Architectural Diagrams

A network diagram and a deployment diagram show basically the same information, just in a different format.
- False

A network diagram and a location diagram show basically the same information but in a different format.
- False

The model that best shows how software components are distributed across hardware components is the ________.​
- Deployment diagram
