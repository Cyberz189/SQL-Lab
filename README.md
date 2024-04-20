                                                      APPLYING FILTERS TO SQL QUERIES




Using SQL to query a database for login attempts allows for detailed analysis of login activities, including information such as country, usernames, dates, and departments. By constructing SQL queries with appropriate conditions and joins, it becomes possible to retrieve specific login data based on various criteria. For example, querying by country can help identify the geographical origin of login attempts, while querying by usernames and dates can provide insights into user behavior and patterns. Additionally, querying by departments enables organizations to track login activities associated with specific departments, facilitating targeted security measures and monitoring. Overall, leveraging SQL for database queries empowers organizations to conduct comprehensive analyses of login attempts, aiding in cybersecurity efforts and ensuring the integrity of their systems.


![IMG_8809](https://github.com/Cyberz189/SQL-Lab/assets/163569052/0575e273-a855-44ea-840e-e4a6e4c9a292)

Using "SELECT" allows me to instruct SQL to begin searching for the command that follows. The "*" symbol, known as a wildcard, is used to search for all or everything. Continuing with "FROM" instructs SQL to specify the data to be searched for in the database, in this case, "log_in_attempts". The subsequent "WHERE" command requests SQL to retrieve "login_dates" greater (>) than the date 2022-05-09. In SQL, a semicolon ";" must be used at the end of a syntax to close the commands. After successfully instructing SQL on what we are searching for, it organizes the data into tables that are easy to read and interpret. Here, we can observe the usernames, login dates, login times, country, IP addresses, and the number of successful logins.


![IMG_8820](https://github.com/Cyberz189/SQL-Lab/assets/163569052/9b554f54-9066-4b9e-87d2-b857b4a1bf0c)

Expanding on the use of filters, im able to use the "between" command to specify a range for the dates im looking to get information on. Using this information is crucial to a SOC analyst as it helps specify or even narrow down the specfic dates


![IMG_8819](https://github.com/Cyberz189/SQL-Lab/assets/163569052/58ea4fc6-1afb-4b05-8f3c-25e5a5f1917c)

Continuing on with the filters this time i use the boolean "<" to look for events that happened before 7:00am on any given day. This helps to see if there was any suspicious activity going on any given day, as cyber attacks are more prevalent during late nights or early mornings.








