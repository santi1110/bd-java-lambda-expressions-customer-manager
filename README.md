### Functional interfaces with lambda expressions Pre-work

Expected time required: 15 min

In this scenario, you are completing an application that processes users of an online store. New terms and conditions
have been released and you need to check a `List` of customers to make sure they have accepted these new terms. Write a 
lambda expression that implements the `Consumer` functional interface that consumes an user from a `List`, and calls 
a method to email that user if they have not accepted the new terms. The resource `DatabaseManager` will handle some 
functionality including emailing the specific customers. The method `checkCustomers` in the class `CustomerManager` has
some TODO methods for you to complete.

1. `CustomerManager` has a method `checkCustomers` that has TODO comments. Using the `forEach` method of `List`, use a 
lambda expression that consumes the items contained in the `List`. You'll pass the lambda expression as the input 
argument to the `forEach` method. Implement the lambda expression in-line.
2. `DatabaseManager` has a method `checkCustomer(String name)` that accepts a `String` that is the name of a customer. 
Use `Strings` from the customers `List` to send to this method. The method will return `true` if the customer has 
already accepted the terms and conditions and will return `false` if they have not accepted the terms and conditions.
3. If `checkCustomer()` returns `false`, then you must call the `DatabaseManager` method `emailCustomer(String name)`. 
Call the method `emailCustomer(String name)` with the customer name and the resource will handle the rest.


HINTS:
* [I'm confused on where to put my code](./hints/hint-01.md)
