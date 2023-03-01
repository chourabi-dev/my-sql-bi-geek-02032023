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

------------------------------------------------------------------------------------------------------------------------------------------------------

SELECT * FROM table WHERE conditions...



CONDICATION A  CONDITION B     AND

TRUE     FALSE   => FALSE

FALSE     TRUE    => FALSE


( TRUE  AND FALSE  ) AND TRUE => FALSE


FALSE AND FALSE => FALSE;

TRUE AND TRUE => TRUE;



CONDICATION A  CONDITION B     OR

TRUE OR TRUE => TRUE
TURE OR FALSE => TRUE
FALSE OR TRUE => TRUE
FALSE OR FALSE => FALSE
( FALSE OR TRUE ) OR TRUE => TRUE

( FALSE OR TRUE ) OR ( FALSE OR TRUE ) => TRUE

--------------------------------------------------
EXMPL AND
SELECT * FROM `products` WHERE `price` < 2000 AND `quantity` < 15

EXMPL OR
SELECT * FROM `products` WHERE `price` < 2000 OR `quantity` < 15

Exmpl NOT
SELECT * FROM `products` WHERE NOT `quantity` = 0


Exmpl ORDER BY ( ASC DESC )
SELECT * FROM `products` ORDER BY `price` ASC
SELECT * FROM `products` ORDER BY `price` DESC


Exmpl MIN
SELECT MIN(`price`) AS `min_price`,`name` FROM `products` 


Exmpl MAX
SELECT MAX(`price`) AS `max_price`,`name` FROM `products` 


Exmpl SUM
SELECT SUM(`price`) FROM `products` WHERE `quantity` = 0


Exmpl AVG
SELECT AVG(`price`) AS `moyen_price` FROM `products` 

Exmpl COUNT
SELECT COUNT(*), `name` FROM `products` WHERE `quantity` = 0



Exmpl LIKE
SELECT * FROM `products` WHERE `name` LIKE 'mac%';
SELECT * FROM `products` WHERE `name` LIKE '%mac';
SELECT * FROM `products` WHERE `name` LIKE '%mac%';
SELECT COUNT(*) AS `total` FROM `products` WHERE  `name` LIKE 'a%';


Exmpl IN
SELECT * FROM `products` WHERE  `quantity` IN ( 0, 5... )

Exmpl between
SELECT * FROM `products` WHERE `price` BETWEEN 800 AND 2500







