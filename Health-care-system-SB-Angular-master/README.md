# Health Care System

- Used Spring-boot for server handling, All API written in spring boot.
- Used Spring security and JWT authentication for security and Login purpose.
- Annotation applied only in spring-boo, NO XML code

- In Angular we developed Frontend pages i.e. Login, Home, Differnet functionalites
- User and Admin, Two type of roles are present.
- User is like an employee in organization, and Admin is Administrator.
- Search functionality are given by the use of Pipe


#### Angular-Client should be on http://localhost:4200
#### Spring-boot-server should run on http://localhost:8080


### MYSQL
- Data Will be store in Mysql-Database
- Database name is **HMSSpring2**
- Give your username and password in application.properties file in spring boot
- Make sure your mysql is running on 3306 else you have to change the port in application.properties file in spring boot

### Mandatory Commands you have to run
#### Manual
- Open your Mysql-workbench or Mysql 8.0 Command line client
- if Database exists **Use HMSSpring2;** else create database and run Spring-boot server application and then come to this point
- Insert Some Data into tables.

#### Existed Commands
- Goto Spring boot -> hms.sql And run this file in workbench.

#### Commands

insert into roles values(1, 'ROLE_USER');<br>
insert into roles values(2, 'ROLE_ADMIN');<br>

insert into users values(1, '$2a$10$nuyV4m3SpBYuqzdRvQK4iO1PI9O0SkLyHQP2YB8CFksVJirzGrDT2', 'admin'); **Password : admin123** <br>
insert into users values(2, '$2a$10$ef4yjYkFjmAjnQk/GPecK.VxaNmpe6yPfBoZh9dcW1.uzf1zFYemu', 'user');' **Password : user123** <br>
**This is Encrypted Password**
<br>
<br>
insert into user_roles values(2, 1);<br>
insert into user_roles values(1, 2);<br>

**There is no signup option in Angular-clinet when it is running on chrome but you can go to signup page by writting this URL**
http://localhost:4200/signup
it will create only **User role** profile for you

### Access
Admin has all accesses <br>
User has all access except Specialization, Department, Employee pages If you try using url then it will show **you are not authorised**


## Images
### Login Page
![Image of Login](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%201.png)


### ADMIN Home Page
![Image of Admin home paage](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%203.png)


### Admin Panel
![Image of Admin Panel-Options](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%204%20-%20Admin%20Panel.png)


### Patinet List
![Image of patient list](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%205%20-%20Patient%20page.jpg)

### Medicos Form
![Image of Medicos Form](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%206%20-%20Medicos%20Form.png)

### Bill List
![Image of Bill list](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%207%20-%20Bill%20List.png)

### Invoice Pr.1
![Image of Invoice](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%208%20-%20Invoice%20part%201.jpg)

### Invoice Pr.2
![Image of Invoice](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%209%20-%20Invoice%20part%202.png)

### Invoice PDF View
![Image of Invoice PDF](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%2010%20-%20Invoice%20PDF.jpg)

### Contact Us
![Image of Contact Us](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%2011%20-%20Contact%20Us.png)


### About Us
![Image of about Us](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%2012%20-%20About%20us.png)


### User-role Options-panel
![User Options](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%2013%20-%20User%20Panel.png)


### When user is not authorised
![User not authorised](https://github.com/akg07/Health-care-system-SB-Angular/blob/master/image%2013%20-%20User-Does-Not-Has-Access.png)
