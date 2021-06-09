# Changing State and This
* The context of the this keyword in JavaScript is determined by how and where the function/method is called not by where the function/method sits
* You would probably assume the context of the this keyword in one of the methods in the App class points to the React component instance and we would therefore be able to access this.state like in the template
* But by default when we call a method like this in reaction to a DOM event in the browser window like a click event the context of the this keyword is lost inside the method and it's set to undefined
* This is the normal behavior of JavaScript
* Old versions of React bound the context of the this keyword to the component instance in our method
* In the newer version we have to manually bind the this keyword to our methods
* But in the render method we can access this.state because render is a built-in React method that automatically binds the context of the this keyword
* But in our own custom methods when we call them in reaction to DOM events we have to bind the context of the this keyword ourselves
* There are different ways to bind the this keyword 
* The easiest way is to use arrow functions
  * Why do arrow functions work?
  * They have a special behavior with the this keyword
  * They bind the value of this to be whatever this is outside of the method
  * And the value of this inside the class component and outside of the method is the component instance, so it takes the value and binds it to the this keyword in the arrow function