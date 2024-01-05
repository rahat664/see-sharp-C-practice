## C#
 - C# (pronounced "See Sharp") is a modern, object-oriented, and type-safe programming language.
 - It was developed by Microsoft within its .NET initiative and later approved as a standard by Ecma (ECMA-334) and ISO (ISO/IEC 23270).
 - C# is one of the programming languages designed for the Common Language Infrastructure.
 - C# is used for developing desktop applications, web applications, and games.
 - C# is an object-oriented, component-oriented programming language. C# provides language constructs to directly support these concepts, making C# a natural language in which to create and use software components.
 - C# is a simple, modern, general-purpose, object-oriented programming language developed by Microsoft within its .NET initiative led by Anders Hejlsberg.

## .Net Architecture
 - .NET is a free, cross-platform, open-source developer platform for building many different types of applications.
 - With .NET, you can use multiple languages, editors, and libraries to build for web, mobile, desktop, games, and IoT.
 - .NET has many different libraries and frameworks, which are used for building different types of applications.
 - C# programs run on .NET, a virtual execution system called the common language runtime (CLR) and a set of class libraries. 
 - The CLR is the implementation by Microsoft of the common language infrastructure (CLI), an international standard. 
 - The CLI is the basis for creating execution and development environments in which languages and libraries work together seamlessly.

## HELLO WORLD
 - The following is a simple C# program that prints "Hello, World!" to the console:
```csharp
    using System;
    class Program
    {
        static void Main()
        {
            Console.WriteLine("Hello, World!");
        }
    }
```
- The program begins with the keyword `using`, which is used to include the `System` namespace in the program. 
- The `System` namespace contains the `Console` class, which is used to read from and write to the console.
- The `Main` method is where the program starts execution.
- The `Console.WriteLine` method prints the message "Hello, World!" to the console.

## Types and Variables
 - C# is a strongly-typed language. This means that every variable must have a type, and that type cannot change after it has been declared.
 - C# has two main categories of types: value types and reference types.
 - Value types directly contain data. Some examples of value types are `int`, `char`, and `float`.
 - Reference types store references to the actual data. Some examples of reference types are `object`, `string`, and `class`.
 - Variables are used to store data, and every variable must be declared with a type. 
 - The type of a variable determines how much memory it occupies and how the bit pattern stored is interpreted.
 - The following outline provides an overview of the basic types in C#:
   - Value Types
     - Simple Types
       - Signed integral: `sbyte`, `short`, `int`, `long`
       - Unsigned integral: `byte`, `ushort`, `uint`, `ulong`
       - Unicode characters: `char`, which represents a UTF-16 code unit
       - IEEE floating point: `float`, `double`
       - High-precision decimal: `decimal`
       - Boolean: `bool`, which represents Boolean values_values that are either `true` or `false`
     - Enum Types
        - User-defined types of the form `enum E {...}`. An `enum` type is a distinct type with named constants. Every `enum` type has an underlying type, which must be one of the eight integral types. The set of values of an `enum` type is the same as the set of values of the underlying type.
     - Struct Types
       - User-defined types of the form `struct S {...}`. A `struct` type is a value type that is typically used to encapsulate small groups of related variables.
     - Nullable Value Types
       - Nullable types of the form `T?` where `T` is a value type. For example, `int?` is a type that can hold any 32-bit integer or `null`.
     - Tuple Value Types
       - Tuple types of the form `(T1, T2, ...)`. For example, `(int, int)` is a type that represents a pair of integers.
   - Reference Types
     - Class Types
       - Ultimate base class of all other types: `object`
       - Unicode strings: `string`, which represents a sequence of UTF-16 code units
       - User-defined types of the form `class C {...}`. A `class` is a reference type that typically contains fields, properties, and methods.
     - Interface Types
       - User-defined types of the form `interface I {...}`. An `interface` is a reference type that defines a set of members. A class or struct that implements an interface must implement all its members.
     - Array Types
       - Single-dimensional, multi-dimensional, and jagged arrays. The default array type is `System.Array`.
       - For example, `int[]` is a single-dimensional array of integers, and `int[,]` is a two-dimensional array of integers.
       - Array types are reference types, and the declaration of an array variable simply sets aside space for a reference to an array instance.
       - The actual array instance must be created with the `new` operator.
       - The elements of an array are accessed by indexing. Array indices are 0-based.
       - Array types are implicitly derived from the `System.Array` base class.
       - Array covariance is supported. This allows an array of a base class to be implicitly converted to an array of a derived class.
     - Delegate Types
       - User-defined types of the form `delegate int D(...)`. A `delegate` type is a reference type that can be used to encapsulate a named or an anonymous method.