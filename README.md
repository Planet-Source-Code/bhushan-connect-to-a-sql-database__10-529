<div align="center">

## Connect to a SQL database


</div>

### Description

connect to a SQL database
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Bhushan\-](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/bhushan.md)
**Level**          |Beginner
**User Rating**    |3.3 (30 globes from 9 users)
**Compatibility**  |C\#
**Category**       |[Algorithims](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/algorithims__10-29.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/bhushan-connect-to-a-sql-database__10-529/archive/master.zip)





### Source Code

```
Compile with:
csc SQLConnect.cs /r:system.data.dll;system.dll
using System;
using System.Data.SQL;
public class SQLConnect
{
private String connString = "";
private SQLConnection dataConn = null;
public void OpenConnection(string connString)
{
this.connString = connString;
dataConn = new SQLConnection(connString);
dataConn.Open();
}
public static void Main(String [] args)
{
SQLConnect dbTest = new SQLConnect();
dbTest.OpenConnection("server=BEACH;uid=;pwd=;database=junk");
}
}
```

