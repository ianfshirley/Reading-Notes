## Javascript Object Basics

1.How would you describe an object to a non-technical friend you grew up with?  
&ensp;&ensp;An object is a set of data, where you can list several attributes about something, and each piece of info can be looked at separately or together. You can also list the same attributes about a similar something and you can compare the things that way.  

2.What are some advantages to creating object literals?  
&ensp;&ensp;It saves times and saves space in your code by combining actions. You can create an array and a function and call the function at once.  

3.How do objects differ from arrays?  
&ensp;&ensp;I'm not really sure how to explain, but it seems like you can do more with an object than an array.   

4.Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.  
&ensp;&ensp;If a prooperty name is held in a variable.  

5.Evaluate the code below. What does the term this refer to and what is the advantage to using this?    
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}  

&ensp;&ensp; 'This' refers to the object that it is inside of; in this case: dog. The advantage is if you have other objects you can use the same function without having to change the method (or whatever it's called. too many new terms to remember)  

## Introduction to the DOM

1.What is the DOM?  
&ensp;&ensp;Document Object Model. Programming interface for web docs.  
2.Briefly describe the relationship between the DOM and JavaScript.  
&ensp;&ensp;The DOM allows JavaScript to manipulate documents, tables and other elements.  

### Sources

[JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)  
[Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

