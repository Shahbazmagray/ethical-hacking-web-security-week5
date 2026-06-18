 Ethical Hacking & Exploiting Vulnerabilities

## Objective

Learn ethical hacking techniques, perform reconnaissance, test for SQL Injection vulnerabilities, and analyze HTTP requests using Burp Suite.

---

## Tools Used

- Kali Linux
- OWASP Juice Shop
- Nmap
- SQLMap
- Burp Suite Community Edition
- Firefox Browser

---

## Tasks Completed

### 1. Reconnaissance

Performed network reconnaissance using Nmap.

Commands:

```bash
nmap localhost

nmap -sV -p 1-1000 localhost
```

Findings:

- Host reachable
- Port 3000 open
- Web application detected

---

### 2. SQL Injection Testing

Performed SQL Injection testing using SQLMap.

Command:

```bash
sqlmap -u "http://localhost:3000/login?email=test"
```

Result:

- Parameter detected
- Parameter not injectable
- No SQL Injection vulnerability found

---

### 3. CSRF Analysis

Used Burp Suite to:

- Intercept requests
- Modify requests
- Replay requests using Repeater

This demonstrated how attackers may manipulate web traffic and why CSRF protections are important.

---

## Security Recommendations

- Use prepared statements
- Validate user inputs
- Implement CSRF tokens
- Use secure session management
- Apply HTTPS

---

## Screenshots

- Nmap Scan
- SQLMap Results
- Burp Suite Intercept
- Modified Request
- Repeater Response

---

## Author

Shahbaz Iftikhar
