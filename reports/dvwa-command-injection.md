# DVWA Command Injection - Low

## Target
http://192.168.56.101/dvwa

## Vulnerability
Command Injection

## Security Level
Low

## Payload Used
```bash
127.0.0.1 && whoami
```

## Result
The application executed the injected operating system command and returned the server-side execution user:

```text
www-data
```

## Impact
Unsanitized input reached the server shell, allowing arbitrary OS command execution through the web application.

## Risk
An attacker could chain system commands, enumerate files, access sensitive data, and potentially escalate privileges.

## Severity
Critical
