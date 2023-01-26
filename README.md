# Dart-Interview-question

1. What is Dart?

        - Dart is a free and open-source programming language. You don’t need to pay any money to run dart programs.
        - Optimized for crafting a beautiful user interface and high-quality experiences. IT IS Used to develop android, iOS, web, and desktop apps fast WITH SAME CODE. Google developed Dart as a programming language.
        - Dart is a platform-independent language and supports almost every operating system such as windows, mac, and Linux.
        - Dart is an object-oriented programming language and supports all oops features such as encapsulation, inheritance, polymorphism, interface, etc.
        - Dart comes with a dart2js compiler which translates dart code to javascript code that runs on all modern browsers.
        - Dart is a programming language used by flutter, the world’s most popular framework for building apps.
        - Offers modern programming features like null safety and asynchronous programming.
         - You can even use Dart for servers and backend.


2. Difference Between Dart & Flutter

        - Dart is a client optimized, object-oriented programming language. It is popular nowadays because of flutter. It is difficult to build complete apps only using Dart because you have to manage many things yourself.

        - Flutter is a framework that uses dart programming language. With the help of flutter, you can build apps for android, iOS, web, desktop, etc. The framework contains ready-made tools to make apps faster.


3.Dart History

        - Google developed Dart in 2011 as an alternative to javascript.
        - Dart 1.0 was released on November 14, 2013.
        - Dart 2.0 was released in August 2018.
        - Dart gained popularity in recent days because of flutter.
        
4. Variable Types

        - String: For storing text value. E.g. “John” [Must be in quotes]
        - int: For storing integer value. E.g. 10, -10, 8555 [Decimal is not included]
        - double: For storing floating point values. E.g. 10.0, -10.2, 85.698 [Decimal is included]
        - num: For storing any type of number. E.g. 10, 20.2, -20 [both int and double]
        - bool: For storing true or false. E.g. true, false [Only stores true or false values]
        - var: For storing any value. E.g. ‘Bimal’, 12, ‘z’, true

        SYNTAX: type variableName = value;
        
        
5. DATA TYPES IN DART


        Data Type	Keyword	                Description
        Numbers	int, double, num	It represents numeric values
        Strings	String	                It represents a sequence of characters
        Booleans	bool	                It represents Boolean values true and false
        Lists	        List	                It is an ordered group of items
        Maps	        Map	                It represents a set of values as key-value pairs
        Sets	        Set	                It is an unordered list of unique values of same types
        Runes	        runes	                It represents Unicode values of String
        Null	        null	                It represents null value
        
        
6. Types Of Comments

        Single-Line Comment: For commenting on a single line of code. E.g. // This is a single-line comment.
        Multi-Line Comment: For commenting on multiple lines of code. E.g. /* This is a multi-line comment. */
        Documentation Comment: For generating documentation or reference for a project/software package. E.g. /// This is a documentation comment
        
7. Types Of Operators

        Arithmetic Operators
        Increment and Decrement Operators
        Assignment Operators
        Logical Operators
        Type Test Operators
        
        Arithmetic Operators:
        Operator Symbol	Operator Name	Description
        +	Addition	For adding two operands
        -	Subtraction	For subtracting two operands
        -expr	Unary Minus	For reversing the sign of the expression
        *	Multiplication	For multiplying two operands
        /	Division	For dividing two operands and give output in double
        ~/	Integer Division	For dividing two operands and give output in integer
        %	Modulus	Remainder After Integer Division

        Increment and Decrement Operators
        Operator Symbol	Operator Name	Description
        ++var	Pre Increment	Increase Value By 1. var = var + 1 Expression value is var+1
        --var	Pre Decrement	Decrease Value By 1. var = var - 1 Expression value is var-1
        var++	Post Increment	Increase Value By 1. var = var + 1 Expression value is var
        var--	Post Decrement	Decrease Value By 1. var = var - 1 Expression value is var
        
        Assignment Operators:    
        Operator Type	Description
        =	Assign a value to a variable
        +=	Adds a value to a variable
        -=	Reduces a value to a variable
        *=	Multiply value to a variable
        /=	Divided value by a variable
        
        Relational Operators:
        >	Greater than	Used to check which operand is bigger and gives result as boolean
        <	Less than	Used to check which operand is smaller and gives result as boolean
        >=	Greater than or equal to	Used to check which operand is bigger or equal and gives result as boolean
        <=	Less than or equal to	Used to check which operand is smaller or equal and gives result as boolean
        ==	Equal to	Used to check operands are equal to each other and gives result as boolean
        !=	Not equal to	Used to check operand are not equal to each other and gives result as boolean
        
        Logical Operators:
        &&	This is ‘and’, return true if all conditions are true
        ||	This is ‘or’. Return true if one of the conditions is true
        !	This is ’not’. return false if the result is true and vice versa
        
        Type Test Operators:
        Operator Symbol	Operator Name	Description
        is	is	Gives boolean value true if the object has a specific type
        is!	is not	Gives boolean value false if the object has a specific type


8. USER INPUT IN DART

        import the package import 'dart:io'; for user input.

        String User Input:
        import 'dart:io';

        void main() {
          print("Enter name:");
          String? name  = stdin.readLineSync();
          print("The entered name is ${name}");
        }

        Integer User Input:
        import 'dart:io';

        void main() {
          print("Enter number:");
          int? number = int.parse(stdin.readLineSync()!);
          print("The entered number is ${number}");
        }

        Foating Point User Input:
        import 'dart:io';

        void main() {
          print("Enter a floating number:");
          double number = double.parse(stdin.readLineSync()!);
          print("The entered num is $number");
        }
        
        
9. String In Dart:
        - String Concatenation:
        print("Using +, Full Name is "+firstName + " " + lastName+".");
        print("Using interpolation, full name is $firstName $lastName.");

        - Properties Of String:
        codeUnits: Returns an unmodifiable list of the UTF-16 code units of this string. //EX. print(str.codeUnits) result:[72, 105]
        isEmpty: Returns true if this string is empty.
        isNotEmpty: Returns false if this string is empty.
        length: Returns the length of the string including space, tab, and newline characters.

        - Methods Of String:
        toLowerCase(): Converts all characters in this string to lowercase.
        toUpperCase(): Converts all characters in this string to uppercase.
        trim(): Returns the string without any leading and trailing whitespace.use trimLeft() and trimRight() methods to remove space from left and right, respectively.
        compareTo(): Compares this object to another.
        replaceAll(): Replaces all substrings that match the specified pattern with a given value. // e.g. text.replaceAll("milk", "water"); 
        split(): Splits the string at matches of the specified delimiter and returns a list of substrings. e.g List<String> listNames = allNames.split(",");
          print("Value of listName is $listNames");
        toString(): Returns a string representation of this object.
        substring(): Returns the text from any position you want. //e.g. text.substring(7)-from index 6 to the last index   text.substring(2,6)-from index 2 to the 6th index 
        codeUnitAt(): Returns the 16-bit UTF-16 code unit at the given index.

        Reverse String: input.split('').reversed.join()
        Capitalize First Letter Of String: text[0].toUpperCase()}${text.substring(1)



- 8.
