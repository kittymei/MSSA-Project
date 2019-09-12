-- Project Step 5

---------------------------------------------------------------------------------------------------------------
-- Submit sql script(s) to 
-- 1. create your database,
-- 2. create your tables (including primary keys and relations consistent with your ERD)
-- 3. populate preliminary data for implementation and test.

---------------------------------------------------------------------------------------------------------------

-- 1. Create your database
CREATE DATABASE budget_app;

---------------------------------------------------------------------------------------------------------------

-- 2. Create your tables

USE budget_app
CREATE TABLE Customer
(
	CustomerID		int				NOT NULL,
	UserName		varchar(20)		NOT NULL,
	Password		varchar(20)		NOT NULL,
	FirstName		varchar(20)		NOT NULL,
	LastName		varchar(20)		NOT NULL,
	Gender			varchar(6)		NOT NULL,
	DOB				date			NOT NULL,
	Email			varchar(30)		NOT NULL,
	Address			varchar(30)		NOT NULL,
	City			varchar(30)		NOT NULL,
	Country			varchar(30)		NOT NULL,
	PostalCode		int				NOT NULL,
	Phone			varchar(30)		NOT NULL
);

USE budget_app
CREATE TABLE Debt
(
	CreditCardLast4			int			NOT NULL,
	CreditCardExpiration	varchar(8)	NOT NULL,
	CreditCardBank			varchar(30)	NOT NULL,
	OweAmoutOnCreditCard	varchar(30)	NOT NULL,

	MonthlyCarPayment		varchar(30)	NOT NULL,
	OweAmountForCar			varchar(30)	NOT NULL,

);

USE budget_app
CREATE TABLE Income
(
	MonthlyIncome	varchar(7)		NOT NULL,
	JobDescription	varchar(30)		NOT NULL,
	CompanyName		varchar(30)		NOT NULL,
	Address			varchar(30)		NOT NULL,
	City			varchar(30)		NOT NULL,
	Country			varchar(30)		NOT NULL,
	PostalCode		int				NOT NULL
);


USE budget_app
CREATE TABLE Savings
(
	AmountInSavings		varchar(15)	NOT NULL,
	AmoutIn401k			varchar(15)	NOT NULL,
	AmountForVacation	varchar(30)	NOT NULL,
	Country				varchar(30)	NOT NULL
	
);

USE budget_app
CREATE TABLE Spending
(
	CustomerID		int				NOT NULL,
	CompanyName		varchar(20)		NOT NULL,
	City			varchar (20)	NOT NULL,
	Country			varchar (20)	NOT NULL,
	ServiceNumber	varchar (20)	NOT NULL,
	AmountSpent		varchar (20)	NOT NULL,
	PurchaseType	varchar(20)		NOT NULL,
	DateOfPurchase	int				NOT NULL

);

---------------------------------------------------------------------------------------------------------------

-- 3. populate preliminary data for implementation and test.

INSERT INTO Customer (CustomerID, UserName, Password, FirstName,LastName, Gender, DOB, Email,
			Address, City, Country, PostalCode, Phone) 
VALUES('123456', 'Tommy123', '987654', 'Tommy', 'Smith', 'Male', '19900316', 'tommysmith@email.com', 
	   '123 Street Ave', 'Topeka', 'USA', '74185', '963-357-1234');

INSERT INTO Debt (CreditCardLast4, CreditCardExpiration, CreditCardBank, OweAmoutOnCreditCard, MonthlyCarPayment,OweAmountForCar)
VALUES('6635', 'Nov 2022', 'Navy Federal Credit Union', '1568.30', '340.00', '15200.00');

INSERT INTO Income (MonthlyIncome, JobDescription,CompanyName,Address,City,Country,PostalCode)
VALUES ('7682.00','Software Developer', 'Microsoft', '987 Add St', 'San Diego', 'USA', '92123' );

INSERT INTO Savings (AmountInSavings, AmoutIn401k, AmountForVacation, Country)
VALUES ('10,600.30', '6,000.20', '600.00', 'Asia');

INSERT INTO Spending (CustomerID, CompanyName, City,Country, ServiceNumber,AmountSpent,PurchaseType,DateOfPurchase)
VALUES ('123456','In & Out', 'San Diego', 'USA', '760-852-951', '29.33', 'Food', '20190320');

