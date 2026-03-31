# DVWA SQL Injection - Low Security

## Target
http://192.168.56.101/dvwa

## Vulnerability
SQL Injection

## Security Level
Low

## Payload Used
```sql
1' OR '1'='1
```

## Result
The payload bypassed normal query logic and returned user records from the database.

## Risk
An attacker can retrieve unauthorized database information and potentially dump sensitive credentials.

## Severity
High


# DVWA SQL Injection - Low

## Target
http://192.168.56.101/dvwa

## Vulnerability
SQL Injection

## Security Level
Low

## Payload Used
```sql
1' OR '1'='1
```

## Result
The payload forced the SQL query to always evaluate as true and returned multiple user records from the backend database.

Returned users included:
- admin
- Gordon Brown
- Hack Me
- Pablo Picasso
- Bob Smith

## Risk
An attacker can enumerate database contents, extract sensitive records, and potentially dump authentication credentials.

## Severity
High
