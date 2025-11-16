# Code Documentation Guidelines

This page lays out some guidlines for creating a code documentation page.
You can see an example here:
[bool2 example](/KSAModding/advanced-internals/code-docs/Brutal/Numerics/bool2)

Make sure to always follow the [general style guid](/KSAModding/meta/style-guide/) on top of these guidlines.



## General guidline

- Pages only cover one function or datatype at a time


## Page Location

Every page should be placed in a folder structure that matches its namespace.

### bool2 Example

The page **`Brutal.Numerics.bool2`** should be located under **Code Docs** like this:

```
Code Docs
└── Brutal
    └── Numerics
        └── bool2
```


## Structure

### Page title
The title of the page should always include the full namespace and type
#### bool2 Example
**`struct Brutal.Numerics.bool2`**

### Last tested version
To keep everyone on the same page always include a version tag above the page title like this
```markdown
<sub><sup>Tested with: **KSA Version 2025.11.4.2791**</sup></sub>
# Title
``` 

### Namespace and Assembly
After the title add a box in the following style containing the namesapce and dll assembly.

---

Example for bool2:
```markdown
> **Namespace:** `Brutal.Numerics`  
> **Assembly:** `Brutal.Core.Numerics.dll`
``` 


### Short description
After the last tested version provide a short description for that specific code element.

### Function prototype
After the description add a section that lists all function protoypes for a function. In case of class or struct list the constructors instead. For a detailed example go to the [bool2 example](/KSAModding/advanced-internals/code-docs/Brutal/Numerics/bool2)

### Members (classes and structs)
When writing documentation for classes or structs, if it has public members add a section for those as well. For a detailed example go to the [bool2 example](/KSAModding/advanced-internals/code-docs/Brutal/Numerics/bool2)

### Methods (classes and structs)
When writing documentation for classes or structs, if it has public methods add a section for those as well. For a detailed example go to the [bool2 example](/KSAModding/advanced-internals/code-docs/Brutal/Numerics/bool2)

### Operators (classes and structs)
When writing documentation for classes or structs, if it has public operators add a section for those as well. For a detailed example go to the [bool2 example](/KSAModding/advanced-internals/code-docs/Brutal/Numerics/bool2)