# **Cipher**
#### Brendan Grubb, 4/21/2017


&nbsp;
## Description
**Cipher** is an application that demonstrates my ability to build custom modules in Drupal. The user of this website is able to encrypt a phrase using a customizable Caesar cipher. The user can choose a word or phrase, a shift value and a shift direction. Every letter in the user's phrase is replaced with another letter from the alphabet. The shift value determines how many letters away the replacement letter is from the original letter. The shift direction determines which way in the alphabet the shift occurs.

&nbsp;
## Setup/Installation Requirements
##### _To view and use this application:_
* It is necessary to download and install a few programs to use this application
    * Go to [getcomposer.org](https://getcomposer.org/) to download Composer (a dependency manager) for free.
    * If you plan on using this app on a mac, go to [mamp.info](https://www.mamp.info/en/downloads/) to download MAMP for free. If you're not using a mac, make sure you have software installed that allows you to host a web server via Apache and manage a database via MySQL (WAMP, LAMP, etc)
* Go to the [Github repository](https://github.com/Brendangrubb/cipher)
* Download the zip file via the green button
* Unzip the file and open the **_cipher-master_** folder
* Inside of the **_cipher-master/sites/db-backup_** folder, grab the **_cipher.sql.zip_** file
* Open MAMP (or equivalent) and click on preferences.
    * In the Web Server tab, set the Document Root to the project folder, **_cipher-master_**.
    * In the Ports tab, make sure that the Apache port number is set to 8888 and the MySQL port number is set to 8889
    * Click start servers.
* Type **_localhost:8888/phpmyadmin_** into your web browser
    * Click the _Import_ tab on the nav bar
    * Click _Choose File_ and navigate to **cipher.sql.zip_**
    * Click _GO_
    * Click the _User Accounts_ tab on the nav bar
    * Click _Add user account_
    * Enter cipher_ as username, _local_ as hostname and cipher_ as password
    * Check all _Global privilages_ and click _Go_
* Type **_localhost:8888_** into your web browser
* The application will load and be ready to use!

&nbsp;
## Specifications
|Behavior|Input|Output|
|--------|-----|------|
| Program will convert input to all lowercase  | _value - 0_ // _direction - right_ // _phrase - "HeLlO"_| _"hello"_ |
| Program will shift letters based on value  | _value - 1_ // _direction - right_ // _phrase - "HeLlO"_| _"ifmmp"_ |
| Program will change letter shift path based on direction  | _value - 1_ // _direction - left // _phrase - "HeLlO"_ | _"gdkkn"_ |
| Program will ignore punctuation and spaces  | _value - 1_ // _direction - left // _phrase - "HeLlO McFly!"_ | _"gdkkn lbekx!"_ |
| Program will treat alphabet cyclically  | _value - 1_ // _direction - right // _phrase - "Pizza Party!"_ | _"qjaab qbsuz!"_ |


&nbsp;
## Known Bugs
* No known bugs

&nbsp;
## Technologies Used
* Drupal
* PHP
* MAMP
* HTML

&nbsp;
_If you have any questions or comments about this program, you can contact me at [brendangrubb@gmail.com](mailto:brendangrubb@gmail.com)._

Copyright (c) 2017 Brendan Grubb

This software is licensed under the GPL license
