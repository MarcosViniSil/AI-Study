
## Static and dynamic typing

The main difference between static and dynamic type is that, in one you need to tell the compiler what is the variable type, the other, you don't. I understood that the compiler will decide for me which is the variable type.

However, it seems that a language that has static typing could not require to tell the compiler which is the variable type, and with that, the dynamic typing is only checked at runtime execution, in contrast, the Static is verified at compile time. 

For summary:

 - Static: maybe is necessary to specify which is the variable type, maybe not, and its type is checked at compile time
 - Dynamic: the type is not necessary and the type check is verified at runtime

 Some examples:

````java
// java example
int variable = 10; // in here we're telling the compiler that we're creating a integer variable
var variable = "linux is good";// here we're asking the type to be infer, and will be an string
````
````javascript
// javascript example
let variable = 10; // the type here will be verified at runtime, and will be classified as number
let variable = "linux is good"; // the type here will be verified at runtime as well, and will be classified as string
````

### what is allowed in which typing?
- Static: once a type is defined, it cannot change its typing during compilation. For example:
````java
// java example
int variable = 10; 
variable =  "linux is good";// -ERROR- once define as integer, it can receive only integer
````
- Static: its type can change during execution. For example:
````javascript
// javascript example
let variable = 10; 
variable = "linux is good"; // this is allowed and will work
````

This was what I could understand about Static and dynamic typing.😁

<audio controls>
  <source src="/assets/audio/static-and-dynamic-type.mp3" type="audio/mp3">
  Your browser does not support the audio element.
</audio>

## References
<a id="1">[1]</a> 
[Static and dynamic typing](https://www.baeldung.com/cs/statically-vs-dynamically-typed-languages)