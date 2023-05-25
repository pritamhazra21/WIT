HTML:
Introduction, Editors, Elements, Attributes, Heading,
Paragraph. Formatting, Link, Head, Table, List, Block,
Layout, 

CSS. Form, Iframe, Colors, Colorname,
Colorvalue.

Image Maps (1L):
map, area, attributes of image area.

Extensible Markup Language (XML) (4L):
Introduction, Tree, Syntax, Elements, Attributes,
Validation, Viewing. XHTML in brief.

CGI Scripts (1L):
Introduction, Environment Variable, GET and POST
Methods.


## CGI GET POST method

In the context of CGI (Common Gateway Interface) scripts, the terms "GET" and "POST" refer to two different methods that can be used to send data from a web browser to the server.

GET request:

When a web form or a link is submitted using the GET method, the form data or parameters are appended to the URL as a query string.
The data is visible in the URL, making it less secure for sensitive information.
The data limit for a GET request is typically limited to a few thousand characters, depending on the server configuration.
GET requests can be bookmarked and cached by browsers.

POST request:

When a web form is submitted using the POST method, the form data or parameters are sent in the body of the HTTP request.
The data is not visible in the URL, making it more secure for sensitive information.
The data limit for a POST request is much higher than that of a GET request, allowing for larger amounts of data to be transmitted.
POST requests are not bookmarkable or cached by browsers by default.
In CGI scripts, the server-side script can receive and process the data sent by the client (web browser) using either the GET or POST method. The script can access the data and perform actions accordingly, such as storing it in a database, generating dynamic content, or processing user inputs.

In most programming languages used for CGI scripting (such as Perl, Python, or PHP), the server-side script can access the data sent via GET or POST through environment variables or special libraries provided by the language. For example, in Perl, the CGI module provides methods to access GET and POST parameters.

It's important to handle user input carefully in CGI scripts to prevent security vulnerabilities, such as cross-site scripting (XSS) or SQL injection. Proper input validation, sanitization, and using prepared statements or parameterized queries can help mitigate these risks.

## XML schema

XML Schema is a specification used to define the structure, content, and data types of XML documents. It provides a way to describe the rules and constraints that XML documents should adhere to. XML Schema is written in XML itself, making it self-descriptive.

Here are some key points about XML Schema:

Structure and Validation: XML Schema defines the structure of an XML document, specifying the elements, attributes, and their hierarchical relationships. It also defines the data types that can be used for element values. XML documents can be validated against an XML Schema to ensure that they conform to the defined structure and data constraints.

Data Types: XML Schema supports various data types, including primitive types like strings, numbers, booleans, dates, and more. It also allows for the creation of complex data types, such as user-defined types and restrictions on existing types. This helps enforce data validation and consistency in XML documents.

Element Definitions: XML Schema allows the definition of elements and their characteristics, such as the element name, data type, occurrence constraints (minOccurs, maxOccurs), default values, and more. This enables the specification of the expected structure and content of XML documents.

Attribute Definitions: XML Schema can define attributes for elements, specifying their names, data types, default values, and constraints. Attributes provide additional metadata or properties for elements within an XML document.

Complex Types and Content Models: XML Schema supports the definition of complex types, which allow for the composition of multiple elements and attributes together. Content models, such as sequences, choices, and repetitions, define the order and structure of elements within complex types. These features enable the creation of more sophisticated and reusable data structures.

Namespace Support: XML Schema supports namespaces, allowing for the creation of modular and extensible schemas. Namespaces help avoid naming conflicts when multiple schemas are used together or when integrating XML data from different sources.

XML Schema provides a powerful way to define the structure, constraints, and data types for XML documents, making it a widely used technology for data validation, data exchange, and interoperability. It is commonly used in various domains, including web services, data interchange formats, configuration files, and more.

