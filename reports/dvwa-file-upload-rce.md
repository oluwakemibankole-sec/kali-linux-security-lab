# DVWA File Upload RCE - Low

## Target
http://192.168.56.101/dvwa

## Vulnerability
Unrestricted File Upload

## Security Level
Low

## Uploaded File
```php
<?php system('whoami'); ?>
```

## Result
The uploaded PHP file was executed successfully from the web-accessible uploads directory and returned:

```text
www-data
```

## Impact
The application allowed executable PHP content to be uploaded into the web root, enabling remote code execution via the browser.

## Risk
An attacker could deploy a persistent web shell, execute arbitrary commands, access sensitive files, and pivot deeper into the server.

## Severity
Critical
