# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket? 0 

### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior? Ticket will print with a zero balance & balance after printing ticket is always 0.
	* What happens if you insert too much money into the machine – do you receive any refund?No
	* What happens if you do not insert enough and then try to print a ticket?It still prints. 

### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine.
	* Does the printed ticket look different?Yes it show the price that you set. 

### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part.
public class Student{}

### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class? Yes the order does matter.  

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram?Won't Compile 
	* What error message do you get when you now press the compile button? identifer unexpected 
	* Do you think this message clearly explains what is wrong?No 

### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class. It is. 

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
	* Hint: There is only one constructor in the class.
	Fields:price,balance,total 
	Constructors:TicketMachine
	Methods:getPrice(),getBalance(),insertMoney(),printTicket

### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class?constructor is taking in an argument 

### Exercise 2.11
* What do you think is the type of each of the following fields?

```java
private int count; primitive int 
private Student representative; object of the student class
private Server host; object of the server class
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive; alive
private Person tutor; tutor
private Game game; game
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in? Yes
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible?
	* Check by pressing the compile button to see if there is an error message.
	* Make sure that you reinstantiate the original version after your experiments!

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration?Yes
* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.
private int status;

### Exercise 2.16
* To what class does the following constructor belong?
```
public Student(String name)
```
Student
### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
```
public Book(String title, double price)
```
2 String, double
### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be? int chapter,String title, String author,int page number,int ISBN 
* Can you assume anything about the names of its fields?They are required. 

Work all Exercises from 2.19 to 2.58 that are **NOT** marked *Challenge exercise*.
READ upto and INCLUDING section 2.15 of this chapter.
2.19
public Pet(String petName){
	 private String name = petsName; 
}
2.21 Return differnt variables 
2.22 What is the balance of the ticket machine that can be used to buy tickets. 
2.23 no
2.24 public int getTotal(){
	return total;
}
2.25 Missing return statment
2.26 Print ticket is outputting text to the screen. It is also manipulating varaibles.
2.27 No
2.28
2.29 void means it is not a constructor
2.30  public void setPrice(int ticketCost){
        price = ticketCost;
    }
2.31 public void increase(int points){
        score = score + points;
    }
2.32 public void discount(int amount){
	price = price - amount;
}
2.36 price would print as a string
2.37 Would recieve an error message
2.38 No becuase you need to print the varaiable price
2.39
2.40 mutator 
2.41 mutator
2.47 no 
2.53 you assinging the value before you set it to 0. 
2.54 you are trying to return before you assign the value. 
2.56 mutator 
