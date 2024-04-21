                                                      APPLYING FILTERS TO SQL QUERIES




Using SQL to query a database for login attempts allows for detailed analysis of login activities, including information such as country, usernames, dates, and departments. By constructing SQL queries with appropriate conditions and joins, it becomes possible to retrieve specific login data based on various criteria. For example, querying by country can help identify the geographical origin of login attempts, while querying by usernames and dates can provide insights into user behavior and patterns. Additionally, querying by departments enables organizations to track login activities associated with specific departments, facilitating targeted security measures and monitoring. Overall, leveraging SQL for database queries empowers organizations to conduct comprehensive analyses of login attempts, aiding in cybersecurity efforts and ensuring the integrity of their systems.


![IMG_8809](https://github.com/Cyberz189/SQL-Lab/assets/163569052/0575e273-a855-44ea-840e-e4a6e4c9a292)

Using "SELECT" allows me to instruct SQL to begin searching for the command that follows. The "*" symbol, known as a wildcard, is used to search for all or everything. Continuing with "FROM" instructs SQL to specify the data to be searched for in the database, in this case, "log_in_attempts". The subsequent "WHERE" command requests SQL to retrieve "login_dates" greater (>) than the date 2022-05-09. In SQL, a semicolon ";" must be used at the end of a syntax to close the commands. After successfully instructing SQL on what we are searching for, it organizes the data into tables that are easy to read and interpret. Here, we can observe the usernames, login dates, login times, country, IP addresses, and the number of successful logins.


![IMG_8820](https://github.com/Cyberz189/SQL-Lab/assets/163569052/9b554f54-9066-4b9e-87d2-b857b4a1bf0c)

Expanding on the use of filters, I'm able to utilize the logical operator "BETWEEN" to specify a date range for the information I'm seeking. This capability is crucial for a SOC analyst as it aids in pinpointing specific dates or narrowing down the timeframe of interest.



![IMG_8819](https://github.com/Cyberz189/SQL-Lab/assets/163569052/58ea4fc6-1afb-4b05-8f3c-25e5a5f1917c)

Continuing with the filters, this time I employ the comparison operator "<" to search for events occurring before 7:00 AM on any given day. This assists in identifying potential suspicious activity, as cyber attacks tend to occur more frequently during late nights or early mornings.



![IMG_8815](https://github.com/Cyberz189/SQL-Lab/assets/163569052/39a44e87-7e37-44f7-bed4-a015db08ef12)


Narrowing down the search using filters, I can utilize SQL to specifically target unsuccessful login attempts occurring after 18:00. By specifying the time and using the boolean "false", I retrieve data on unsuccessful attempts by username, country, IP address, and time. This focused approach allows for a thorough analysis of potential security threats during specific timeframes, aiding in the identification and mitigation of cybersecurity risks.


![IMG_8814](https://github.com/Cyberz189/SQL-Lab/assets/163569052/6649e1a3-4917-43eb-8846-5a6412c4561d)

Another logical operator that can be employed is "OR", which instructs SQL to combine two boolean conditions to further refine a search. In this case, we're directing SQL to retrieve information that occurred on either 2022-05-09 or 2022-05-08. This allows for a broader search scope, facilitating the retrieval of relevant data across multiple dates and enabling comprehensive analysis and reporting.


![IMG_8812](https://github.com/Cyberz189/SQL-Lab/assets/163569052/0fb3c89c-6f60-4dd3-97f0-ce685d9eda4f)

Filtering with 'NOT' instructs SQL to retrieve information that excludes what's specified. In this case, using 'LIKE' directs SQL to search for countries that don't start with 'MEX' and employing the wildcard '%' fills characters in a word. For instance, 'MEX%' could denote 'Mexican,' 'Mexico,' or any other word starting with 'MEX.' By combining all the boolean operators together, SQL can provide information where the country doesn't include Mexico


![IMG_8810](https://github.com/Cyberz189/SQL-Lab/assets/163569052/c3f40556-5759-485e-aec4-390f2ab0a11d)

Finally, SQL also enables filtering, simplifying database searches. Here, we can employ SQL to search a department for employees in Sales or Finance and retrieve their employee ID, username, and department. In security, time is of the essence, and the capability to swiftly locate and analyze information could offer a company peace of mind, cost savings, and safeguard its reputation


In conclusion using SQL for security purposes, SQL offers a powerful toolset for managing and safeguarding sensitive data within databases. Its efficient filtering and querying capabilities enable swift access to information, crucial in time-sensitive scenarios for mitigating risks and preventing breaches. Organizations can implement stringent access controls, monitor user activities, and detect anomalies to ensure data integrity and confidentiality. SQL's versatility allows integration with security protocols and encryption mechanisms, fortifying databases against unauthorized access and cyber threats. Overall, SQL plays a pivotal role in enhancing data protection, safeguarding company assets, and preserving organizational reputation in today's digital landscape.






