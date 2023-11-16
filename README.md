# slashmark_project2
Task 1 : OpenAI Codex  - Saying "Hello" (Python)  -Create random names (Python)  -Create a MySQL query (Python)

print("Hello")

import random
first_names = ["John", "Alice", "Bob", "Eva"]
last_names = ["Smith", "Johnson", "Miller", "Jones"]
random_names = [random.choice(first_names) + " " + random.choice(last_names) for _ in range(10)]
print(random_names)

Task 2 : Get up and running with the OpenAI API  -Step 1 : Setup Python  -Step 2 : Setup your API key  -Step 3 : Sending your first API request

import mysql.connector
db_config = {
    "host": "DESKTOP-CJH229F",
    "user": "root",
    "password": "slash",
    "database": "slashmark1",
}
connection = mysql.connector.connect(**db_config)
cursor = connection.cursor()
query = "SELECT * FROM your_table WHERE your_condition;"
cursor.execute(query)
results = cursor.fetchall()
for row in results:
    print(row)
cursor.close()
connection.close()



