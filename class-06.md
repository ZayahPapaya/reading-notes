# Table of Contents

[Class 01](class-01.md)
[Class 02](class-02.md)
[Class 03](class-03.md)
[Class 04](class-04.md)
[Class 05](class-05.md)
[Class 06](class-06.md)
[Class 07](class-07.md)
[Class 08](class-08.md)
[Class 09](class-09.md)
[Class 10](class-10.md)
11
12
13
14
15

## Reading 06

### Object Literals

Let testObject = {
  hands: 2,
  fingers: 10,
  knees: 2,
  toes:  10,
  isInjured: function() {
    return this.fingers;
  }
}

testObject.fingers
    ^         ^
  Object   Property/method

Objects are defined similarly to an array or variable, and the 'this' keyword is used to refer directly to the object that the function is called in. Above is the syntax for defining properties of objects, as well as the method (a special function for objects).

### Document Object Model (DOM)

The DOM / Document Object model is an organizational model for the components for a webpage as they're actually used and manipulated, which is reflected in the user's browser.

getElementById(), querySelector(), getElementsByClassName(), getElementsByTagName(), querySelectorAll(), parentNode, previousSibling, nextSibling, firstChild, lastChild

Above are many example functions that help access the DOM in some way.

Similar to an array, you can loop through a nodelist that you've selected which would act on multiple parts of a document, such as a set of list items.

Individual components of a webpage, the nodes, can be directly modified or replaced, such as elText.replace('target', 'replacement');.
