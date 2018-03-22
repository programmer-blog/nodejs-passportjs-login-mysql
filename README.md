# nodejs-passportjs-login-mysql
Programmer Blog: https://programmerblog.net/

Source code for article on NodeJS PassportJS login with MySQL.

You can read detailed tutorial on our blog: http://programmerblog.net/nodejs-passport-login-mysql/
     
        Install MySQL and PHPMyAdmin 
      
          1. Create a database db_users.

          2. Create a database table for tbl_users and insert sample data into the table.
   
       Install NodeJS, Express Generator
       
          1. Generate a NodeJS, Express Application using Express Generator.

          2. Install required modules using NPM.
          
            ``` 
                npm install connect-flash

                npm install passport

                npm install passport-local

                npm install express-session

                npm install memory

                npm install crypto

                npm install mysql
            
            ```

        Create a NodeJS passportJS login script with MySQL.
        
 Read More at: http://programmerblog.net/nodejs-passport-login-mysql/
        
 MySQL Script for Creating Database and Users table with sample data
        
        
             create database db_users;

              -- --------------------------------------------------------
              use db_users;


              --
              -- Database: `db_users`
              --

              -- --------------------------------------------------------

              --
              -- Table structure for table `tbl_users`
              --

              CREATE TABLE `tbl_users` (
                `id` int(11) NOT NULL,
                `username` varchar(16) NOT NULL,
                `password` varchar(60) NOT NULL,
                `full_name` varchar(100) NOT NULL
              ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=latin1;

              --
              -- Dumping data for table `tbl_users`
              --

              INSERT INTO `tbl_users` (`id`, `username`, `password`, `full_name`) VALUES
              (1, 'john', '6607a999607711cd339dce1de6d64425a0985cfd', 'John Doe');

              --
              -- Indexes for dumped tables
              --

              --
              -- Indexes for table `tbl_users`
              --
              ALTER TABLE `tbl_users`
                ADD PRIMARY KEY (`id`);

              --
              -- AUTO_INCREMENT for dumped tables
              --

              --
              -- AUTO_INCREMENT for table `tbl_users`
              --
              ALTER TABLE `tbl_users`
                MODIFY `id` int(11) NOT NULL AUTO_INCREMENT,AUTO_INCREMENT=2;
        
         
        
     
