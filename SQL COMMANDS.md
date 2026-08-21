1. SELECT --> default command
2. FROM --> it fetches from the next mentioning database
3. `SELECT * FROM OrderDetails`
	+ `*  --> it includes all rows and colums
	+ OrderDetails --> database name
4. `SELECT OrderId FROM OrderDetails`
	+ OrderId --> sub column inside database
5. `SELECT OrderID , * FROM OrderDetails`
	+ it fetches both OrderID sub column details and all the contets from OrderDetails Database
6. `SELECT * FROM OrderDetails where OrderID is null`
	+ It fetches any null value present in OrderID subcolum from OrderDetails database
7. `SELECT * FROM OrderDetails where ProductID = 42`
	+ It fetches all the contents that matches with the ProductID's value of 42
8. `SELECT OrderDetailID FROM OrderDetails where ProductID = 42`
	+ It fetches only the OrderDetailID sub column values which matches with ProductID 42
9. `SELECT * FROM OrderDetails where ProductID = 42 and OrderID = 10309`
	+ It  fetches the exact row where both 42 and 10309 are matched
10. `SELECT * FROM OrderDetails where ProductID = 42 or OrderID = 10309`
	+ It fetches all the rows even if one of the value is 42 or 10309
11. `SELECT * FROM OrderDetails where OrderID in (10248, 10299)`
	+ It fetches all the values where OrderID is 10248 and 10299
12. `SELECT * FROM OrderDetails where OrderID not in (10248, 10299)`
	+ It fetches all the OrderDetails sub column values except 10248 and 10299
13. `SELECT DISTINCT OrderID FROM OrderDetails`
	+ It removes the duplicate/ repeating values and represent only one value from each sets
14. `SELECT * FROM Customers where CustomerName like 'A%'`
	+ It fetches where CustomerName starts with 'A'
	+ %--> denotes the unknown text after the mentioned first letter
15. `SELECT * FROM Customers where CustomerID in (5,6,7,8)`
	+ fetches the entire row where the CustomerID is as mentioned
16. `SELECT * FROM Customers where CustomerID between 2 and 12`
	+ fetches entire row value where the CustomerID value between 2 and 12
17. `SELECT Count(*) FROM OrderDetails where OrderID between 10248 and 10265`
	+ gives the count or no.of values from 10248 to 10265
18. `SELECT avg(ProductID) as Average FROM OrderDetails`
	+ average of ProductID is fetched and given to user defined variable (Average)
	+ so it is displayed as :`variable : avg.value
	+ Other : `sum, max, min, `
	+ This is not case sensitive ; "AVG = avg"
19. `SELECT * FROM OrderDetails Order BY ProductID`
	+ `Order BY -->` defaultly arranges in ascending order on the values based on ProductID column
	+ ProductID is user defined we can change as per our need
20. `SELECT * FROM OrderDetails Order BY ProductID DESC`
	+ `DESC-->`It orders the value in descending order
21. `SELECT TOP 5 * FROM Customers`
	+ `TOP -->`fetches Top 5 values from customers database
22. `JOIN METHODS`
		1. `Inner - joins two columns from different databases whose value matches`
		2. `Outer - Joins two columns from diff. databases even if values don't match`
		3. `Left - compares values on the right sides based on the left side column`
		4. `Right - compares values on left side based the value on the right`
23. ``SELECT * FROM Suppliers SP INNER JOIN Employees EM ON SP.SupplierID =  EM.EmployeeID``
	+ Fetches all the column matching with the required condition
24. `SELECT SupplierName FROM Suppliers SP INNER JOIN Employees EM ON SP.SupplierID =  EM.EmployeeID`
	+ fetches SupplierName Column value which matches the values of SupplierID column from Suppliers database and EmployeeID from Employees databas
25. `SELECT SP.SupplierName, EM.FirstName FROM Suppliers SP INNER JOIN Employees EM ON SP.SupplierID =  EM.EmployeeID`
	+ fetches , SupplierName column and FirstName column value which matches as per the condition
	+ SP. and EM. represents their respective object name of their databases 
26. `SELECT SP.SupplierName, EM.FirstName FROM Suppliers SP Left JOIN Employees EM ON SP.SupplierID =  EM.EmployeeID`
	+ keeps the SupplierName from Suppliers database as the base and compares the FirstName column from Employee databases
27. `SELECT SP.SupplierName, EM.FirstName FROM Suppliers SP Right JOIN Employees EM ON SP.SupplierID =  EM.EmployeeID`
	+ keeps the EmployeeID from Employee database as the base and compares the SupplierName column from Suppliers databases i.e keeps the right side table as the base