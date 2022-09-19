# C# Fundamentals


**1.** What is the purpose of a `namespace`?
<!-- enter you answer in the space below -->
```
declares a scope that contains a set of related objects
```
**2.** What is the difference between a `class` and a `struct`?
<!-- enter you answer in the space below -->
```
Structs are light versions of classes
```
**3.** What is the method that returns an instance of a class, yet it has no return type?
<!-- enter you answer in the space below -->
```
void
```
## Example 1
```c#
abstract class Car
{
  ...
  public virtual string Start()
  {
    return "Vroooom";
  }
}
```
**5.** In the example what is the access modifier of the `Start()` method?
<!-- enter you answer in the space below -->
```
public
```
**6.** In the example what is `string` an indication of?
<!-- enter you answer in the space below -->
```
the datatype
```
**7.** In the example what is `abstract` preventing?
<!-- enter you answer in the space below -->
```
prevents the inheritance of a class or certain class members that were previously marked virtual
```
**8.** In the example what is the purpose of `virtual`?
<!-- enter you answer in the space below -->
```
used to modify a method and allow for it to be overridden in a derived class
```
**9.** Name four access modifiers:
<!-- enter you answer in the space below -->
```
public, private, protected, internal
```
**10.** If you set a class or method to private, what can access it?
<!-- enter you answer in the space below -->
```
Only functions of the same class can access its private members
```