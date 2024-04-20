                                                      APPLYING FILTERS TO SQL QUERIES




Using SQL to query a database for login attempts allows for detailed analysis of login activities, including information such as country, usernames, dates, and departments. By constructing SQL queries with appropriate conditions and joins, it becomes possible to retrieve specific login data based on various criteria. For example, querying by country can help identify the geographical origin of login attempts, while querying by usernames and dates can provide insights into user behavior and patterns. Additionally, querying by departments enables organizations to track login activities associated with specific departments, facilitating targeted security measures and monitoring. Overall, leveraging SQL for database queries empowers organizations to conduct comprehensive analyses of login attempts, aiding in cybersecurity efforts and ensuring the integrity of their systems.


![IMG_8809](https://github.com/Cyberz189/SQL-Lab/assets/163569052/0575e273-a855-44ea-840e-e4a6e4c9a292)

Using "SELECT" allows me to instruct SQL to begin searching for the command that follows. The "*" symbol, known as a wildcard, is used to search for all or everything. Continuing with "FROM" instructs SQL to specify the data to be searched for in the database, in this case, "log_in_attempts". The subsequent "WHERE" command requests SQL to retrieve "login_dates" greater (>) than the date 2022-05-09. In SQL, a semicolon ";" must be used at the end of a syntax to close the commands. After successfully instructing SQL on what we are searching for, it organizes the data into tables that are easy to read and interpret. Here, we can observe the usernames, login dates, login times, country, IP addresses, and the number of successful logins.


![IMG_8820](https://github.com/Cyberz189/SQL-Lab/assets/163569052/9b554f54-9066-4b9e-87d2-b857b4a1bf0c)

Expanding on the use of filters, I'm able to utilize the "BETWEEN" command to specify a date range for the information I'm seeking. This capability is crucial for a SOC analyst as it aids in pinpointing specific dates or narrowing down the timeframe of interest.



![IMG_8819](https://github.com/Cyberz189/SQL-Lab/assets/163569052/58ea4fc6-1afb-4b05-8f3c-25e5a5f1917c)

Continuing with the filters, this time I employ the boolean operator "<" to search for events occurring before 7:00 AM on any given day. This assists in identifying potential suspicious activity, as cyber attacks tend to occur more frequently during late nights or early mornings.



![IMG_8815](https://github.com/Cyberz189/SQL-Lab/assets/163569052/39a44e87-7e37-44f7-bed4-a015db08ef12)


Narrowing down the search using filters, I can utilize SQL to specifically target unsuccessful login attempts occurring after 18:00. By specifying the time and using the command "success = false", I retrieve data on unsuccessful attempts by username, country, IP address, and time. This focused approach allows for a thorough analysis of potential security threats during specific timeframes, aiding in the identification and mitigation of cybersecurity risks.










