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
[Class 11](class-11.md)
[Class 12](class-12.md)
[Class 13](class-13.md)
[Class 14](class-14.md)
[Class 15](class-15.md)

## Reading 13

### Local Storage

The use of local storage is rocky at best at higher levels, higher levels that we will not be touching in the near future just yet. For now we get to work with limited and simple cookies that store small amounts of information for each user that will be easily recovered between sessions to allow for persistent data. The data is stored as a string inside of, what appears to be, a native JS object called localStorage. Values retrieved from the object must be un-stringified to be used properly in most cases.
