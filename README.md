# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

## Adapter Design Pattern
#### Main Concept using a Real Life Analogy
The charging plug of many foreign appliances are incompatible with Indian power sockets thus in order to use them we generally use a third device known as a Power Adapter which acts as a bridge and connects the interfaces after performing necessary adaptations without changing the functionality of the socket or appliance. 

Adapter Pattern follows the exact concept by acting as a bridge between two or more incompatible interfaces. 
#### Implementation
To implement Adapter Design we need to develop an adapter class that connects two or more incompatible interfaces without changing any content of those.
#### Advantage(s)
* Quick Integration with third party or FOSS libraries.
* Development complexity is minimal.
* Increased Re-usability.
#### Disadvantage(s)
* In an ideal world there is no place for adapters, thus although useful it's overhead.
* Chaining several adapters might become a risk for maintenance in future.

## Builder Design Pattern
#### Main Concept using a Real Life Analogy
When creating any complex object such as a car it is practical to follow a bottom-up approach where the development start with the minor components which construct the major components such as engine, chassis, transmission and finally the major components are assembled together to build the car. 

Builder Pattern follows the exact concept where developer starts with smallest components and builds-up to the final requirement. 
#### Implementation
To implement Builder Pattern we need to identify the components and traverse bottom-up developing and testing each component in the way.
#### Advantage(s)
* Very Structured development strategy, easier to maintain SRP and DRY concepts. 
* Error Contamination at the earliest.
* Ease of maintenance over time.
#### Disadvantage(s)
* Might be considered a slower method in the starting phase as decoupling and identification of unit components is crucial and time consuming.

## Composite Design Pattern
#### Main Concept using a Real Life Analogy
If we consider combos or bundles offered in stores, in spite of being a combination of several items the customer is expected to treat combos the same as any other singular item, all operations valid for a single item is also valid for combos such as checking price and buying.

Composite Pattern follows the exact concept where we need to treat a group of objects in a similar way as a single object.
#### Implementation
To implement Composite Pattern we need to create a class that can hold a list of it's own instances and the class should also expose methods of adding/removing these instances. Any operation valid for a single instance should also be considered for all the instances registered.
#### Advantage(s)
* Flexible design and extremely useful while implementing hierarchical classes.
#### Disadvantage(s)
* Not an outright disadvantage but the implementation scope is not too broad.

## Observer Design Pattern
#### Main Concept using a Real Life Analogy
When we subscribe to any YouTube channel, it is understood that the client (us) is interested in receiving notifications of any update to the subject (the channel). To fulfill the requirement subject uses one or more observers (various notifiers) and updates all whenever there is any update to it. Once notified, each observer fulfills it's task and thus we receive push notification, mails and UI notifications. 

The Observer Pattern is the behavior where a set of observers are notified at once by the subject generally to relay the information to client.  
#### Implementation
To implement Observer Pattern we need to create a Subject class that can contain a list of observers and can add/remove observers and notify all whenever there is any update. The observers classes must satisfy a mutual contract but are free to have different implementations. 

#### Advantage(s)
* Great support for open/closed principle.
#### Disadvantage(s)
* Not an outright disadvantage but the implementation scope is not too broad.



