import pyodbc

server = 'servname'
database ='dbname'
username='sa'
password='password'

conn= pyodbc.connect(DRIVER={ODBC Driver 18 for SQL Server};SERVER='+server+';DATABASE='+database+';ENCRYPT=yes;UID='+username+';PWD='+ password)
cursor = cnxn.cursor()

cursor.execute("select @@version;")
row=cursor.fetchone()
while row:
    print(row[0])
    row=cursor.fetchone()
cnxn.commit()