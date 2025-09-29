-- Create Tables
CREATE TABLE Invoices (
	InvoiceID CHAR(6) PRIMARY KEY,
	Tanggal_Invoice DATE NOT NULL,
	Jatuh_Tempo DATE NOT NULL
);
show tables;
CREATE TABLE Sales (
	SalesID CHAR(6) PRIMARY KEY,
	SalesName VARCHAR(255) NOT NULL,
	SalesAddress VARCHAR(255) NOT NULL,
	SalesPhone CHAR(14) NOT NULL,
	SalesEmail VARCHAR(255) NOT NULL
);

CREATE TABLE Customers (
	CustomerID CHAR(7) PRIMARY KEY,
	CustomerName VARCHAR(255) NOT NULL,
	CustomerAddress VARCHAR(255) NOT NULL,
	CustomerPhone CHAR(14) NOT NULL,
	CustomerEmail VARCHAR(255) NOT NULL
);

CREATE TABLE Products (
	ProductID CHAR(7) PRIMARY KEY,
	ProductName VARCHAR(255) NOT NULL,
	Price INT NOT NULL
);

CREATE TABLE Orders (
	InvoiceID CHAR(6),
	SalesID CHAR(6),
	CustomerID CHAR(7),
	ProductID CHAR(7),
	Quantity INT NOT NULL,
	FOREIGN KEY (InvoiceID) REFERENCES Invoices(InvoiceID) ON DELETE NO ACTION,
	FOREIGN KEY (SalesID) REFERENCES Sales(SalesID) ON DELETE NO ACTION,
	FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) ON DELETE NO ACTION,
	FOREIGN KEY (ProductID) REFERENCES Products(ProductID) ON DELETE NO ACTION,
	PRIMARY KEY (InvoiceID, SalesID, CustomerID, ProductID)
);

-- Sample Data
INSERT INTO Invoices (InvoiceID, Tanggal_Invoice, Jatuh_Tempo)
VALUES
('INV001', DATE('2024/11/19'), DATE('2024/12/19')),
('INV002', DATE('2024/11/20'), DATE('2024/12/20')),
('INV003', DATE('2024/11/21'), DATE('2024/12/21')),
('INV004', DATE('2024/11/22'), DATE('2024/12/22')),
('INV005', DATE('2024/11/23'), DATE('2024/12/23')),
('INV006', DATE('2024/11/24'), DATE('2024/12/24')),
('INV007', DATE('2024/11/25'), DATE('2024/12/25')),
('INV008', DATE('2024/11/26'), DATE('2024/12/26')),
('INV009', DATE('2024/11/27'), DATE('2024/12/27')),
('INV010', DATE('2024/11/28'), DATE('2024/12/28'));

INSERT INTO Sales (SalesID, SalesName, SalesAddress, SalesPhone, SalesEmail)
VALUES
('SAL001', 'PT Fauget', 'Jl. Merdeka Raya No. 10, Jakarta Pusat, DKI Jakarta', '0812-3456-7890', 'sales@fauget.co.id'),
('SAL002', 'PT Teknologi Cerdas', 'Jl. Teknologi Utama No.45, Bandung, Jawa Barat', '0821-9876-5432', 'sales@teknologicerdas.co.id'),
('SAL003', 'PT Solusi Digital', 'Jl. Digital Nusantara No. 20, Surabaya, Jawa Timur', '0838-5678-1234', 'sales@solusidigital.co.id'),
('SAL004', 'PT Inovasi Hebat', 'Jl. Inovasi Mandiri No. 88, Yogyakarta, DIY', '0813-8765-4321', 'sales@inovasihebat.co.id'),
('SAL005', 'PT Gemilang Mandiri', 'Jl. Mandiri Sejahtera No. 99, Medan, Sumatera Utara', '0852-2345-6789', 'sales@gemilangmandiri.co.id'),
('SAL006', 'PT Jaya Mandiri', 'Jl. Kemajuan Bangsa No. 77, Semarang, Jawa Tengah', '0811-2233-4455', 'sales@jayamandiri.co.id'),
('SAL007', 'PT SwiftLink Teknologi', 'Jl. Cendekia Cepat No. 21, Makassar, Sulawesi Selatan', '0851-6677-8899', 'sales@swiftlink.co.id'),
('SAL008', 'PT DigiLancer Logistik', 'Jl. Logistik Prima No. 15, Balikpapan, Kalimantan Timur', '0822-4444-6666', 'sales@digilancer.co.id'),
('SAL009', 'PT SmartCargo Solutions', 'Jl. Cargo Modern No. 30, Denpasar, Bali', '0817-5555-7777', 'sales@smartcargo.co.id'),
('SAL010', 'PT LogiTech Nusantara', 'Jl. Teknologi Logistik No. 50, Palembang, Sumatera Selatan', '0831-9999-8888', 'sales@logitech-nusantara.co.id');

INSERT INTO Customers (CustomerID, CustomerName, CustomerAddress, CustomerPhone, CustomerEmail)
VALUES
('CUST001', 'PT Nusantara Abadi', 'Jl. Kebangkitan No. 12, Jakarta Pusat, DKI Jakarta', '0812-1111-2222', 'info@nusantaraabadi.co.id'),
('CUST002', 'PT Sinar Jaya', 'Jl. Pelangi Timur No. 34, Bandung, Jawa Barat', '0821-3333-4444', 'sales@sinarjaya.co.id'),
('CUST003', 'PT Mitra Sejahtera', 'Jl. Harmoni Raya No. 21, Surabaya, Jawa Timur', '0838-5555-6666', 'contact@mitrasejahtera.co.id'),
('CUST004', 'PT Global Indotek', 'Jl. Tekno Jaya No. 7, Yogyakarta, DIY', '0813-7777-8888', 'global@indotek.co.id'),
('CUST005', 'PT Cahaya Nusantara', 'Jl. Sentosa Utama No 88, Medan, Sumatera Utara', '0852-9999-1111', 'support@cahayanusantara.co.id'),
('CUST006', 'PT Bumi Mandiri', 'Jl. Mandiri baru No. 15, Semarang, Jawa Tengah', '0811-4444-5555', 'info@bumimandiri.co.id'),
('CUST007', 'PT Surya Teknologi', 'Jl. Cerdas Cepat No. 10, Makassar, Sulawesi Selatan', '0851-8888-9999', 'surya@teknologi.co.id'),
('CUST008', 'PT Trans Kargo', 'Jl. Logistik Raya No. 44, Balikpapan, Kalimantan Timur', '0822-1111-2222', 'contact@transkargo.co.id'),
('CUST009', 'PT Bali Agung', 'Jl. Dewata Utama No. 23, Denpasar Bali', '0817-5555-6666', 'sales@baliagung.co.id'),
('CUST010', 'PT Sumatera Logistik', 'Jl. Logistik Hebat No. 29, Palembang, Sumatera Selatan', '0831-7777-8888', 'info@sumateralogistik.co.id');


INSERT INTO Products (ProductID, ProductName, Price)
VALUES
('PROD001', 'Laptop Businesss Pro', 12500000),
('PROD002', 'Smartphone Ultra', 8000000),
('PROD003', 'Printer All-in-One', 3500000),
('PROD004', 'Monitor 24-inch LED', 2500000),
('PROD005', 'Wireless Keyboard', 700000),
('PROD006', 'External Hard Drive', 1200000),
('PROD007', 'Office Chair Comfort', 2750000),
('PROD008', 'Gaming Headset', 1500000),
('PROD009', 'Smartwatch Elite', 3000000),
('PROD010', 'Power Bank 20,000mAh', 500000);

INSERT INTO Orders (InvoiceID, SalesID, CustomerID, ProductID, Quantity)
VALUES
('INV001', 'SAL001', 'CUST001', 'PROD001', 10),
('INV001', 'SAL002', 'CUST001', 'PROD001', 10),
('INV002', 'SAL002', 'CUST002', 'PROD002', 15),
('INV002', 'SAL002', 'CUST007', 'PROD002', 15),
('INV003', 'SAL003', 'CUST003', 'PROD003', 8),
('INV004', 'SAL004', 'CUST004', 'PROD004', 12),
('INV005', 'SAL005', 'CUST005', 'PROD005', 20),
('INV006', 'SAL006', 'CUST006', 'PROD006', 25),
('INV007', 'SAL007', 'CUST007', 'PROD007', 5),
('INV008', 'SAL008', 'CUST008', 'PROD008', 18),
('INV009', 'SAL009', 'CUST009', 'PROD009', 10),
('INV010', 'SAL010', 'CUST010', 'PROD010', 50);

-- Sample Selects
SELECT * FROM Orders;
SELECT * FROM Customers;
SELECT Orders.ProductID, Quantity FROM Orders
	INNER JOIN Products
	ON Products.ProductID = Orders.ProductID
	WHERE Products.Price > 10000;
