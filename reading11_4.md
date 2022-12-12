# Event Driven Applications

1. What native Node.js module allows us to get started with Event Driven Programming?

  - Node. js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away.

2. What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

  - The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other. This is where we can make use of Event-driven programming. By registering event listeners we can actually reverse the flow of communication between our objects. Rather than on object needing to reach inside another object to trigger a function, our objects can just emit events and whichever objects are listening to those event will process it in the way they have been told to. The source of an objects behavior is now entirely contained within itself, rather than needing to be accessed by external objects.

3. Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

  - Event-driven programming is used to synchronize the occurrence of multiple events and to make the program as simple as possible.