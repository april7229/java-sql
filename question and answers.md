find all customers that live in London. Returns 6 records.
This can be done with SELECT and WHERE clauses
4	Around the Horn	Thomas Hardy	120 Hanover Sq.	London	WA1 1DP	UK
11	B's Beverages	Victoria Ashworth	Fauntleroy Circus	London	EC2 5NT	UK
16	Consolidated Holdings	Elizabeth Brown	Berkeley Gardens 12 Brewery	London	WX1 6LT	UK
19	Eastern Connection	Ann Devon	35 King George	London	WX3 6FW	UK
53	North/South	Simon Crowther	South House 300 Queensbridge	London	SW7 1RZ	UK
72	Seven Seas Imports	Hari Kumar	90 Wadhurst Rd.	London	OX15 4NB	UK

find all customers with postal code 1010. Returns 3 customers.
This can be done with SELECT and WHERE clauses
12	Cactus Comidas para llevar	Patricio Simpson	Cerrito 333	Buenos Aires	1010	Argentina
54	Océano Atlántico Ltda.	Yvonne Moncada	Ing. Gustavo Moncada 8585 Piso 20-A	Buenos Aires	1010	Argentina
64	Rancho grande	Sergio Gutiérrez	Av. del Libertador 900	Buenos Aires	1010	Argentina

find the phone number for the supplier with the id 11. Should be (010) 9984510.
This can be done with SELECT and WHERE clauses
1	Heli Süßwaren GmbH & Co. KG	Petra Winkler	Tiergartenstraße 5	Berlin	10785	Germany	(010) 9984510


list orders descending by the order date. The order with date 1997-02-12 should be at the top.
This can be done with SELECT, WHERE, and ORDER BY clauses
SELECT * FROM [Orders]
order by orderdate DESC

find all suppliers who have names longer than 20 characters. You can use length(SupplierName) to get the length of the name. Returns 11 records.
This can be done with SELECT and WHERE clauses
SELECT * FROM [Suppliers]
Where length(suppliername) >20


find all customers that include the word "market" in the name. Should return 4 records.
This can be done with SELECT and a WHERE clause using the LIKE keyword

Don't forget the wildcard '%' symbols at the beginning and end of your substring to denote it can appear anywhere in the string in question
