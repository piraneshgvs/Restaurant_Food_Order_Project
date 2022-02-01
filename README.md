# Restaurant_Food_Order_Project

#Database mysql query to excute the project

             Restaurant Application DDL 
Database Name: restaurant
Tables:
  1. cart
  2. food
  3. staff
  4. user

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

 1.cart DDL (Data Definition Language)
    
     CREATE TABLE `cart` (
             `tabno` int NOT NULL,
             `user_id` varchar(45) NOT NULL,
             `fid` int NOT NULL,
            `fQua` int NOT NULL,
            `fTot` int NOT NULL,
           `fgtotal` int DEFAULT NULL,
           `status` varchar(5) DEFAULT 'no',
           `date` timestamp NULL DEFAULT CURRENT_TIMESTAMP)


------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2.food DDL

     CREATE TABLE `food` (
         `food_id` int NOT NULL AUTO_INCREMENT,
        `food_name` varchar(45) NOT NULL,
        `price` int NOT NULL,
        `available` varchar(45) NOT NULL DEFAULT 'yes',
         `images` longblob NOT NULL,
          PRIMARY KEY (`food_id`)
)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3.staff DDL

       CREATE TABLE `staff` (
         `name` varchar(45) DEFAULT NULL,
       `phone` varchar(13) DEFAULT NULL,
      `password` varchar(45) DEFAULT NULL,
      `staff_role` varchar(5) DEFAULT NULL
)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

4.user DDL

  CREATE TABLE `user` (
      `user_id` varchar(45) NOT NULL,
      `phonenumber` varchar(13) NOT NULL,
      `feedback` varchar(255) DEFAULT NULL,
      `time` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
       PRIMARY KEY (`user_id`)
)


----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Happy coding
