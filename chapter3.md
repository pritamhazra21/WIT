
# PERL (3L):
## Introduction,

Perl (Practical Extraction and Reporting Language) is a programming language that has been widely used in web technology for many years. It was one of the first programming languages to be adopted for web development and has played a significant role in the evolution of the web.

Perl is particularly well-suited for tasks involving text processing, data manipulation, and system administration. In the context of web development, Perl is commonly used for server-side scripting, where it runs on the web server and generates dynamic content that is then sent to the client's web browser.

Some common uses of Perl in web technology include:

CGI (Common Gateway Interface): Perl was one of the original languages used for writing CGI scripts. CGI allows web servers to execute programs or scripts and generate dynamic web content based on user input or other parameters.

Web frameworks: Perl has various web frameworks available, such as Mojolicious, Dancer, and Catalyst. These frameworks provide a structure and set of tools for building web applications in Perl, simplifying the development process.

Templating: Perl offers templating systems like Template Toolkit and Mason, which facilitate the separation of code and presentation in web applications. Templating allows developers to define reusable templates and insert dynamic data into them, making it easier to maintain and update web pages.

Web scraping: Perl has long been favored for web scraping due to its powerful regular expression support and text-processing capabilities. Developers can use Perl to extract data from websites, automate data collection, or build web spiders or crawlers.

System administration and automation: Perl's strengths in text processing and system interaction make it well-suited for tasks related to web server administration, log analysis, and automation of routine tasks.

While Perl's popularity in web development has diminished in recent years with the rise of other languages like Python, Ruby, and JavaScript, it still has a dedicated user base and continues to be used in legacy systems or specific niches where its strengths are valued.

## Variable, 


In Perl, variables are created by using the dollar sign ($) symbol followed by the variable name. Perl has three main types of variables: scalars, arrays, and hashes.

Scalars: Scalars are used to store single values. They can hold integers, floating-point numbers, strings, or boolean values. Here's an example:
```
my $name = "John";      # a scalar variable holding a string value
my $age = 30;           # a scalar variable holding an integer value
my $pi = 3.14159;       # a scalar variable holding a floating-point number
my $isStudent = 1;      # a scalar variable holding a boolean value (1 for true, 0 for false)

```
Arrays: Arrays are used to store ordered lists of values. They are represented using the @ symbol followed by the array name. Individual elements in an array can be accessed using square brackets ([]). Here's an example:
```
my @fruits = ("apple", "banana", "orange");    # an array variable holding string values
print $fruits[0];        # accessing the first element of the array (prints "apple")

```
Hashes: Hashes are used to store key-value pairs. They are represented using the % symbol followed by the hash name. Individual values in a hash can be accessed using curly braces ({}) and the corresponding key. Here's an example:
```
my %person = (
    "name" => "John",
    "age" => 30,
    "occupation" => "Engineer"
);
print $person{"name"};   # accessing the value associated with the key "name" (prints "John")

```
These are the basic variable types in Perl. Variables in Perl are dynamically typed, meaning that they can hold values of different types, and their types can change during runtime. The my keyword is used to declare variables with limited scope within a block or subroutine.


## Condition, Loop, Array,

Conditions:
In Perl, you can use conditional statements to make decisions based on certain conditions. The if, elsif, else, and unless keywords are commonly used for conditionals. Here's an example:
```
my $age = 25;

if ($age < 18) {
    print "You are underage.";
}
elsif ($age >= 18 && $age < 65) {
    print "You are an adult.";
}
else {
    print "You are a senior citizen.";
}
```
![image](https://github.com/pritamhazra21/WIT/assets/75198912/c0ba7b12-524b-4213-a52e-7296848646ec)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/82de6a6f-236f-4922-9b09-28dcee5a58d4)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/abe6552c-1c25-4b61-813f-e305cb9ccb82)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/af84a5e3-68e3-4fd2-9f29-c8a92c2d0153)



## Implementing data structure, Hash, String,
![image](https://github.com/pritamhazra21/WIT/assets/75198912/3f99825e-0ab8-4653-8029-ee9c04912c32)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/853757a6-8bbc-465a-b8a0-2f5014849997)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/86d84427-8513-4f1f-a889-f1fc44503565)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/a9fe35ed-bb28-4d8e-bcb3-f90d8c4ddd7b)




## Regular Expression, File handling, I/O handling.
![image](https://github.com/pritamhazra21/WIT/assets/75198912/b6746f43-db10-4bc3-90ad-d9ebff852881)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/1585525c-de8c-44aa-a987-a051238629fb)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/8666196d-3717-4935-95a3-bf9a794a4b78)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/d1525a40-d0fd-456e-aa73-09166eaa2f0a)

# Cookies (1L):
## Definition of cookies,

Cookies are small pieces of data that are stored on a user's computer by a website they visit. They are commonly used in web development to enable various functionalities and enhance the user experience. Cookies are created by the web server and sent to the user's browser, which then stores the cookie on the user's computer.

## Create and Store a cookie with example.
```
use CGI::Cookie;

# Create a new cookie
my $cookie = CGI::Cookie->new(
    -name    => 'username',
    -value   => 'JohnDoe',
    -expires => '+1d',  # Expires in 1 day
);

# Store the cookie in the HTTP header
print "Set-Cookie: $cookie\n";
print "Content-Type: text/html\n\n";
print "Cookie has been set!";

```
In this example, we use the CGI::Cookie module, which is a Perl module that provides functions for handling cookies. We create a new cookie object using the new() method, specifying the cookie name (username), value (JohnDoe), and expiration time (1 day from now).

Next, we send the cookie in the HTTP header using the Set-Cookie header field. The cookie is printed using the print statement with the Set-Cookie prefix. Note that this code assumes you are using Perl's CGI module for web programming.

When the user's browser receives this response, it will store the cookie on the user's computer. The cookie will be sent back to the server with subsequent requests made by the user, allowing the server to retrieve and use the stored information.

Remember to adjust the code based on your specific web framework or server configuration, as the process of setting cookies may vary depending on the environment you are working in.
