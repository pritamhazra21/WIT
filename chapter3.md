
## PERL (3L):
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

1. Scalars: Scalars are used to store single values. They can hold integers, floating-point numbers, strings, or boolean values. Here's an example:

```perl
my $name = "John";      # a scalar variable holding a string value
my $age = 30;           # a scalar variable holding an integer value
my $pi = 3.14159;       # a scalar variable holding a floating-point number
my $isStudent = 1;      # a scalar variable holding a boolean value (1 for true, 0 for false)
```

2. Arrays: Arrays are used to store ordered lists of values. They are represented using the `@` symbol followed by the array name. Individual elements in an array can be accessed using square brackets ([]). Here's an example:

```perl
my @fruits = ("apple", "banana", "orange");    # an array variable holding string values
print $fruits[0];        # accessing the first element of the array (prints "apple")
```

3. Hashes: Hashes are used to store key-value pairs. They are represented using the `%` symbol followed by the hash name. Individual values in a hash can be accessed using curly braces ({}) and the corresponding key. Here's an example:

```perl
my %person = (
    "name" => "John",
    "age" => 30,
    "occupation" => "Engineer"
);
print $person{"name"};   # accessing the value associated with the key "name" (prints "John")
```

These are the basic variable types in Perl. Variables in Perl are dynamically typed, meaning that they can hold values of different types, and their types can change during runtime. The `my` keyword is used to declare variables with limited scope within a block or subroutine.

## Condition, Loop, Array,



1. Conditions:
   In Perl, you can use conditional statements to make decisions based on certain conditions. The `if`, `elsif`, `else`, and `unless` keywords are commonly used for conditionals. Here's an example:

   ```perl
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

2. Loops:
   Perl provides different types of loops to repeat a block of code. The `for`, `foreach`, `while`, `do-while`, and `until` loops are commonly used in Perl. Here are a few examples:

   - `for` loop:

     ```perl
     for (my $i = 1; $i <= 10; $i++) {
         print "$i ";
     }
     ```

   - `foreach` loop (for iterating over an array):

     ```perl
     my @fruits = ("apple", "banana", "orange");

     foreach my $fruit (@fruits) {
         print "$fruit ";
     }
     ```

   - `while` loop:

     ```perl
     my $count = 1;

     while ($count <= 5) {
         print "$count ";
         $count++;
     }
     ```

3. Arrays:
   Arrays in Perl allow you to store ordered lists of values. You can access and manipulate array elements using indices. Here are a few examples:

   - Creating an array:

     ```perl
     my @numbers = (1, 2, 3, 4, 5);
     ```

   - Accessing array elements:

     ```perl
     my $first_element = $numbers[0];     # accessing the first element (1)
     my $third_element = $numbers[2];     # accessing the third element (3)
     ```

   - Modifying array elements:

     ```perl
     $numbers[1] = 10;                    # changing the second element to 10
     ```

   - Looping through an array:

     ```perl
     foreach my $number (@numbers) {
         print "$number ";
     }
     ```

   - Array functions:

     Perl provides various built-in functions to manipulate arrays, such as `push`, `pop`, `shift`, `unshift`, `splice`, `join`, and more. These functions help you add or remove elements, manipulate the array's structure, and perform common operations.

These are just the basics of conditions, loops, and arrays in Perl. Perl offers a wide range of features and functions to work with these concepts, allowing you to perform complex logic and data manipulation tasks.



## Implementing data structure, Hash, String,

1. Hashes:
   Hashes in Perl are used to store key-value pairs. They are implemented using the `%` symbol followed by the hash name. Here's an example:

   ```perl
   my %person = (
       "name" => "John",
       "age" => 30,
       "occupation" => "Engineer"
   );
   ```

   You can access and manipulate the values in a hash using the corresponding keys. Here are a few examples:

   - Accessing values:

     ```perl
     my $name = $person{"name"};
     my $age = $person{"age"};
     ```

   - Modifying values:

     ```perl
     $person{"occupation"} = "Developer";
     ```

   - Adding new key-value pairs:

     ```perl
     $person{"city"} = "New York";
     ```

   - Looping through a hash:

     ```perl
     foreach my $key (keys %person) {
         my $value = $person{$key};
         print "$key: $value\n";
     }
     ```

2. Strings:
   Perl provides powerful string manipulation capabilities. Here are some common operations you can perform on strings:

   - Concatenation:

     ```perl
     my $string1 = "Hello";
     my $string2 = "World";
     my $result = $string1 . ", " . $string2;   # Concatenating strings
     ```

   - String interpolation:

     ```perl
     my $name = "John";
     my $greeting = "Hello, $name!";            # String interpolation
     ```

   - Length of a string:

     ```perl
     my $string = "Hello";
     my $length = length($string);              # Getting the length of a string
     ```

   - Substring extraction:

     ```perl
     my $string = "Hello, World!";
     my $substring = substr($string, 7, 5);     # Extracting "World"
     ```

   - Pattern matching:

     ```perl
     my $string = "Hello, World!";
     if ($string =~ /World/) {
         print "Found 'World' in the string.";
     }
     ```

   - String manipulation functions:

     Perl provides a wide range of built-in functions for string manipulation, such as `index`, `rindex`, `split`, `join`, `uc`, `lc`, `substr`, `chomp`, `sprintf`, and many more. These functions allow you to perform tasks like searching, splitting, formatting, case conversions, and more.

These are just some examples of how you can work with hashes and strings in Perl. Perl offers a rich set of features and functions for manipulating data structures and handling string operations, making it flexible and powerful for various programming tasks.



## Regular Expression, File handling, I/O handling.

1. Regular Expressions:
   Regular expressions (regex) in Perl are powerful tools for pattern matching and text manipulation. Perl has robust support for regular expressions through built-in functions and special syntax. Here are some examples of using regular expressions in Perl:

   - Pattern matching using the `=~` operator:

     ```perl
     my $string = "Hello, World!";
     if ($string =~ /World/) {
         print "Found 'World' in the string.";
     }
     ```

   - Extracting substrings using capturing groups:

     ```perl
     my $string = "Hello, World!";
     if ($string =~ /Hello, (.*)!/) {
         my $name = $1;   # Captured substring inside parentheses
         print "Hello, $name!";
     }
     ```

   - Substituting patterns using the `s///` operator:

     ```perl
     my $string = "Hello, World!";
     $string =~ s/World/Perl/;   # Substitute "World" with "Perl"
     print $string;
     ```

   - Matching with modifiers and flags:

     ```perl
     my $string = "Hello, world!";
     if ($string =~ /world/i) {   # Ignore case using 'i' modifier
         print "Match found!";
     }
     ```

   Perl offers many more features and functions for regular expressions, including character classes, quantifiers, anchors, assertions, and more. Regular expressions are extensively used for text parsing, validation, search and replace, and data extraction tasks in Perl.

2. File Handling:
   Perl provides various functions and operators to handle files, read and write data, and perform file operations. Here are some common file handling operations in Perl:

   - Opening a file:

     ```perl
     open(my $filehandle, '<', 'filename.txt') or die "Cannot open the file: $!";
     ```

   - Reading data from a file:

     ```perl
     while (my $line = <$filehandle>) {
         chomp $line;   # Remove newline character
         print "$line\n";
     }
     ```

   - Writing data to a file:

     ```perl
     open(my $filehandle, '>', 'output.txt') or die "Cannot open the file: $!";
     print $filehandle "Hello, World!\n";
     close $filehandle;
     ```

   - Appending data to a file:

     ```perl
     open(my $filehandle, '>>', 'filename.txt') or die "Cannot open the file: $!";
     print $filehandle "New line of data\n";
     close $filehandle;
     ```

   - File operations and checks:

     ```perl
     # Checking if a file exists
     if (-e 'filename.txt') {
         print "File exists!";
     }

     # Getting file size
     my $filesize = -s 'filename.txt';
     print "File size: $filesize bytes";
     ```

   Perl provides many more functions and operators for file handling, such as `seek`, `tell`, `rename`, `unlink`, directory operations, and file permissions.

3. I/O Handling:
   Perl provides several I/O handling mechanisms, including standard input/output and file handles. Here are a few examples:

   - Standard input:

     ```perl
     my $input = <STDIN>;   # Reading input from the user
     chomp $input;
     ```

   - Standard output:

     ```perl
     print "Hello, World!\n";   # Writing output to the console
    

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


# JavaScript (4L):
## Basics,
Certainly! Here's a detailed explanation of JavaScript statements, comments, variables, comparisons, conditions, switches, loops, breaks, objects (such as strings, arrays, Booleans, and regular expressions), functions, errors, and validation, along with code samples:

1. Statements:
   - JavaScript statements are individual instructions that perform specific actions or operations.
   - Examples of statements:
     ```javascript
     var x = 5; // Variable assignment statement
     console.log("Hello, world!"); // Function call statement
     if (x > 0) { // Conditional statement
         console.log("Positive");
     } else {
         console.log("Negative");
     }
     ```

2. Comments:
   - Comments in JavaScript provide explanations and help in code documentation.
   - Single-line comments start with //, while multi-line comments are enclosed between /* and */.
   - Example:
     ```javascript
     // This is a single-line comment
     /*
        This is a
        multi-line comment
     */
     ```

3. Variables:
   - Variables in JavaScript are used to store data values.
   - They can be declared using the "var", "let", or "const" keywords.
   - Example:
     ```javascript
     var x = 5; // Declaring a variable "x" and assigning a value of 5
     let y = "Hello"; // Declaring a variable "y" and assigning a string value
     const PI = 3.14; // Declaring a constant variable "PI" with a value of 3.14
     ```

4. Comparison:
   - Comparison operators are used to compare values and return a Boolean result (true or false).
   - Example:
     ```javascript
     var x = 5;
     var y = 10;
     console.log(x > y); // false
     console.log(x === 5); // true
     ```

5. Conditions:
   - Conditional statements allow you to perform different actions based on different conditions.
   - Examples:
     ```javascript
     var age = 18;
     if (age >= 18) {
         console.log("You are an adult");
     } else {
         console.log("You are a minor");
     }
     ```

6. Switch:
   - The switch statement allows you to execute different actions based on different cases.
   - Example:
     ```javascript
     var day = "Monday";
     switch (day) {
         case "Monday":
             console.log("Today is Monday");
             break;
         case "Tuesday":
             console.log("Today is Tuesday");
             break;
         default:
             console.log("Other day");
     }
     ```

7. Loops:
   - Loops are used to repeatedly execute a block of code.
   - Examples: 
     - For loop:
       ```javascript
       for (var i = 0; i < 5; i++) {
           console.log(i);
       }
       ```
     - While loop:
       ```javascript
       var i = 0;
       while (i < 5) {
           console.log(i);
           i++;
       }
       ```

8. Break:
   - The break statement is used to exit a loop or switch statement.
   - Example:
     ```javascript
     for (var i = 0; i < 5; i++) {
         if (i === 3) {
             break;
         }
         console.log(i);
     }
     ```

9. Objects - String, Array, Boolean, RegEx:
   - JavaScript has built-in objects for strings, arrays, Booleans, and regular expressions.
   - Examples:
     - String object:
       ```javascript
       var

 str = "Hello";
       console.log(str.length); // 5
       console.log(str.toUpperCase()); // "HELLO"
       ```
     - Array object:
       ```javascript
       var arr = [1, 2, 3];
       console.log(arr.length); // 3
       console.log(arr[0]); // 1
       ```
     - Boolean object:
       ```javascript
       var bool = true;
       console.log(bool.toString()); // "true"
       ```
     - Regular Expression object:
       ```javascript
       var regex = /hello/i;
       console.log(regex.test("Hello")); // true
       ```

10. Function:
    - Functions in JavaScript are reusable blocks of code that can be invoked to perform a specific task.
    - Example:
      ```javascript
      function greet(name) {
          console.log("Hello, " + name);
      }
      greet("John"); // "Hello, John"
      ```

11. Errors:
    - JavaScript provides built-in error objects to handle and manage errors.
    - Examples:
      - Throw an error:
        ```javascript
        throw new Error("Something went wrong");
        ```
      - Try-catch block to handle errors:
        ```javascript
        try {
            // Code that may throw an error
        } catch (error) {
            // Code to handle the error
        }
        ```

12. Validation:
    - JavaScript can be used for form validation on web pages.
    - Example:
      ```javascript
      function validateForm() {
          var name = document.forms["myForm"]["name"].value;
          if (name == "") {
              alert("Name must be filled out");
              return false;
          }
      }
      ```
      




Java Applets (2L):
Container Class, Components, Applet Life Cycle,
Update method;
Parameter passing applet,
Applications.
