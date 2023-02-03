*********************************************************************** demo QUERY ******************************************************************************

- CREATE TABLE `product` (

    `code` int(20),
    `name` VARCHAR(20),
    `price` float(20),
    `quantity` int(100)
    
);



- DROP TABLE `demo`


- ALTER TABLE `product` ADD `unit` int(5)

- ALTER TABLE `product` DROP COLUMN `unit`

- CREATE TABLE `users` (
	`fullname` VARCHAR(200) NOT NULL,
    `email` VARCHAR(200) UNIQUE
);