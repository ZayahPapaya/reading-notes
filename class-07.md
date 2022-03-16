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

## Reading 07

### Domain Modeling

I was looking for this concept previously, on Monday or Tuesday, and am excited to finally note down how it actually works. A model is essentially the same concept as a function with parameters and arguments. You define an object with a set of properties, but the properties are empty placeholders to fill in information later. You can then create new objects based off of that template by filling in the arguments.

let exampleModel = function(property1, property2) {
  this.property1 = propertyVal1;
  this.property2 = propertyVal2;
}
var subModel1 = new exampleModel(true, 'value');
var subModel2 = new exampleModel(false, 'null');

This creates new objects with the information filled in.

### Tables

They're tables lmao. Writing them is:

`<table>`
  `<tr>`
    `<th scope="col">First</th>`
    `<th scope="col">Second</th>`
   `<th scope="row">Numbers</th> <td>1</td> <td>2</td> <td>3</td>`
  `</tr>`
  `<tr>`
    `<th scope="row">Letters</th> <td>a</td> <td>b</td> <td>c</td>`
  `</tr>`
`</table>`
         First Second
Numbers  1 2 3
Letters  a b c

Other goodies:
`<td colspan="3">info</td>` will make an item span across 3 columns. rowspan does the same but for multiple rows.
`<thead>, <tbody>, <tfoot>` will all act like normal HTML definitions. They're the head, body, and foot for a table that help organize and style it.
