## Order Status

The Middletown Wholesale Copper Wire Company sells spools of copper wiring for $100 each. Write a program that displays the status of an order. The program should have a function that asks for the following data:
- The number of spools ordered.
- The number of spools in stock.
- Whether there are special shipping and handling charges.
- If there are special charges, the program should ask for the special charges per spool. (Shipping and handling is normally $10 per spool.) 

The function should use 4 reference parameters for these values: number ordered, number in stock, if there's special shipping, and if so the special charges. 

The gathered data should be passed as arguments to a second function that displays:
- The number of spools ready to ship from current stock.
- The number of spools on backorder (if the number ordered is greater than what is in stock).
- Subtotal of the portion ready to ship (the number of spools ready to ship times $100).
- Total shipping and handling charges on the portion ready to ship.
- Total of the order ready to ship.

The shipping and handling parameter in the second function should be a **default parameter** equal to 10.00. When this function is called this default parameter should then be used unless there are special shipping charges. An if/else statement can be used in the main function to determine if the default parameter should be used, for example:
```
if (specialShipping == 'y')
  display(numOrdered, numStocked, specialCharges);
else
  display(numOrdered, numStocked);
```

Use good identifiers when defining variables and functions.

Optional Input Validation: Do not accept numbers less than 1 for spools ordered. Do not accept a number less than 0 for spools in stock or shipping and handling charges.