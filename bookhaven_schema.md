Book Haven DataBase: 

This is a simple database schema for BookHaven, meant to show the relationships between Books, Authors, Customers, and Transactions.

Below is a list of Tables, each with a list of columns by attribute and key type, with relationships listed between each table.  

Books Table: 
 - Primary Key = ISBN
 - Foreign Key = Author ID
 - Title 
 - Publication Date

Books are many to many with authors 
Books (isbn) is one to one with Transactions

Authors Table: 
 - Primary Key  = Author ID
 - Author Name  

Authors are many to many with books 

Customers Table: 
 - Primary Key = Customer ID 
 - Customer Name

Customer(customer ID) is one to many with Transactions

Transactions Table: 
 - Primary Key = Transaction ID
 - Foreign Key = Customer ID 
 - Foreign Key = Book ID
 - Due Date

Transactions are many to one with Customers(customer id). 
Transactions is one to one with Books(isbn) 