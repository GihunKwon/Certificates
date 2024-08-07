## 7.1 SQL with Python
<br/>

### Practice
<code>
import mysql.connector
from mysql.connector import Error
import pandas a pd

<br/>
'''
def create_server_connection(host_name,user_name,user_password):
    connection = None
    try:
        connection = mysql.connector.connect(
            host = host_name,
            user = user_name,
            passwd = user_password
        )
        print("MySQL Database connection successful")
    except Error as err:
        print(f"Error : '{err}'")
    return connection
'''
<br/>
'''
pw = "....."
db = "database_name"
connection = create_server_connection("localhost","root",pw)
'''
<br/>

# create mysql_python
'''
def create_database(connection,query):
    cursor = connection.cursor()
    try:
        cursor.execute(query)
        print('Database created successfully')
    except Error as err:
        print(f"Error : '{err}'")

create_database_query = "Create database mysql_python"
create_database(connection,create_database_query)
'''