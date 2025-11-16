# Reverse Engineering

For advanced modders who want to dig deeper into how KSA works internally.

## Using ILSpy

[ILSpy](https://github.com/icsharpcode/ILSpy) is a free .NET decompiler. You can use it to browse KSA's code:

1. Download ILSpy
2. Open `KSA.dll` from `C:\Users\[YourName]\AppData\Local\Programs\Kitten Space Agency\`
3. Browse the code to see how things work

This lets you find:

- What XML attributes are actually supported
- Internal class structures
- How vehicles and parts are loaded
- Available properties and methods

**Other tools:** dnSpy (debugger + decompiler), dotPeek, Process Monitor
