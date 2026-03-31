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
