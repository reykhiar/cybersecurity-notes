# Web Fundamentals for Cybersecurity
## Overview
Web technologies are at the core of modern cybersecurity. Understanding how websites work, how browsers communicate with servers, and how web applications process user input is essential before learning topics such as Web Security, Burp Suite, OWASP Top 10, and Web Penetration Testing.

This note covers the fundamental concepts required to understand web applications and the technologies that support them.

---

## How Websites Work
When a user visits a website, several processes take place behind the scenes:
1. The browser sends a request to access a website.
2. DNS resolves the domain name into an IP address.
3. The browser communicates with the web server using HTTP or HTTPS.
4. The server responds with content such as HTML, CSS, JavaScript, and images.
5. The browser renders the content and displays it to the user.

Understanding this process helps security professionals identify how data flows between users and web applications.

---

## Domain Name System (DNS)
The Domain Name System (DNS) translates human-readable domain names into IP addresses.
Example:
```text
google.com → 142.250.x.x
```

### Common DNS Records

| Record | Purpose                                                |
| ------ | ------------------------------------------------------ |
| A      | Maps a domain to an IPv4 address                       |
| AAAA   | Maps a domain to an IPv6 address                       |
| CNAME  | Creates an alias for another domain                    |
| MX     | Specifies a mail server                                |
| TXT    | Stores text-based information and verification records |

DNS plays a critical role in web browsing, email delivery, and network reconnaissance.

---

## HTTP and HTTPS
HTTP (HyperText Transfer Protocol) is the protocol used for communication between web browsers and web servers.
HTTPS is the secure version of HTTP and uses TLS encryption to protect transmitted data.
### HTTP
Characteristics:
* Unencrypted communication
* Data can potentially be intercepted by attackers
### HTTPS
Characteristics:
* Encrypted communication
* Protects data confidentiality
* Helps ensure data integrity
* Standard for modern websites

Using HTTPS significantly improves the security of web communications.

---

## HTTP Methods
HTTP methods define the action a client wants to perform on a resource.
### GET
Retrieves data from a server.
Example:
```http
GET /index.html
```
### POST
Sends data to a server.
Example:
```http
POST /login
```
### PUT
Updates an existing resource.
### DELETE
Removes a resource.

Understanding HTTP methods is important when analyzing web traffic and testing web applications.

---

## HTTP Status Codes
Web servers return status codes to indicate the result of a request.
| Code | Meaning               |
| ---- | --------------------- |
| 200  | OK                    |
| 201  | Created               |
| 301  | Moved Permanently     |
| 401  | Unauthorized          |
| 403  | Forbidden             |
| 404  | Not Found             |
| 500  | Internal Server Error |
| 503  | Service Unavailable   |

Status codes provide valuable information during troubleshooting and security assessments.

---

## HTTP Headers
HTTP headers provide additional information during client-server communication.
Common headers include:
```http
Host:
User-Agent:
Cookie:
Content-Type:
Authorization:
```

Headers are frequently examined during web application testing and traffic analysis.

---

## Cookies
Cookies are small pieces of data stored in a user's browser.
Common uses include:
* Authentication
* Session management
* User preferences
Example:
```http
Cookie: sessionid=abc123
```

Cookies are a key component of modern authentication systems and web sessions.

---

## Frontend vs Backend
### Frontend
The frontend is the part of a website that users interact with directly.
Common technologies:
* HTML
* CSS
* JavaScript
### Backend
The backend handles requests, processes data, and generates responses.
Common technologies:
* PHP
* Python
* Node.js
* Ruby

Backend systems often communicate with databases, APIs, and other services.
Understanding the distinction between frontend and backend components helps identify potential attack surfaces.

---

## HTML Basics
HTML (HyperText Markup Language) defines the structure of a web page.
Common HTML tags:
```html
<html>
<head>
<body>
<h1>
<p>
<a>
<img>
```

HTML provides the foundation for displaying content in a web browser.

---

## JavaScript Basics
JavaScript adds interactivity and dynamic behavior to websites.
Common uses include:
* Modifying page content
* Handling user events
* Validating forms
* Creating dynamic web applications

JavaScript is widely used in modern web development and is frequently encountered during security testing.

---

## Sensitive Data Exposure
Sensitive Data Exposure occurs when confidential information becomes accessible to unauthorized users.
Examples include:
* Hardcoded passwords
* Exposed API keys
* Embedded credentials
* Internal URLs and system information

Example:
```html
<!-- admin:test123 -->
```

Reviewing page source code and application responses can sometimes reveal sensitive information that should not be publicly accessible.

---

## HTML Injection
HTML Injection occurs when user input is rendered as HTML without proper validation or sanitization.
Example:
```html
<h1>Injected Content</h1>
```

Potential impacts include:
* Website defacement
* Displaying misleading content
* Serving as a stepping stone toward more advanced attacks

### Prevention
* Input validation
* Output encoding
* Proper sanitization

Secure input handling is essential for preventing web-based attacks.

---

## Load Balancers
A Load Balancer distributes incoming traffic across multiple servers.
Benefits include:
* Improved availability
* Better performance
* Fault tolerance and failover support

Common load-balancing methods:
* Round Robin
* Weighted Distribution

Load balancers help ensure web applications remain accessible under varying traffic conditions.

---

## Content Delivery Networks (CDNs)
A Content Delivery Network (CDN) stores and serves content from geographically distributed servers.
Common cached content:
* Images
* CSS files
* JavaScript files
* Videos

Benefits include:
* Faster content delivery
* Reduced server load
* Improved user experience

CDNs are widely used to improve both performance and availability.

---

## Web Application Firewalls (WAFs)
A Web Application Firewall (WAF) sits between users and web applications.
Primary functions:
* Blocking malicious requests
* Detecting common attack patterns
* Rate limiting
* Protecting web applications

Common threats mitigated:
* SQL Injection
* Cross-Site Scripting (XSS)
* Certain Denial-of-Service attacks

WAFs are an important layer of defense for modern web applications.

---

## Web Servers
Web servers are responsible for delivering web content to users.
Common web servers:
* Apache
* Nginx
* IIS
* Node.js-based servers

Responsibilities:
* Processing HTTP requests
* Serving website content
* Hosting web applications

Web servers form the foundation of web application infrastructure.

---

## Static and Dynamic Content
### Static Content
Content that remains unchanged regardless of user interaction.
Examples:
* Images
* CSS files
* JavaScript files

### Dynamic Content
Content generated based on user requests or backend processing.
Examples:
* User dashboards
* Search results
* Blog feeds

Most modern web applications rely heavily on dynamic content.

---

## Virtual Hosts
Virtual Hosts allow multiple websites to run on a single web server.
Example:
```text
example1.com
example2.com
example3.com
```

Each website can have its own configuration while sharing the same physical server.

---

## Cybersecurity Relevance
Understanding web fundamentals is essential because:
* HTTP is used in nearly all web communications.
* DNS is important for reconnaissance and network investigations.
* Cookies are critical for authentication and session security.
* Sensitive Data Exposure is a common web vulnerability.
* HTML Injection introduces important web exploitation concepts.
* HTTP headers are frequently analyzed during security assessments.
* Load Balancers, CDNs, and WAFs are commonly encountered in enterprise environments.
* Understanding frontend and backend architecture helps identify potential attack surfaces.

---

## Key Takeaway
Web fundamentals provide the foundation for understanding how modern web applications operate and how attackers interact with them. These concepts are essential for future topics such as Burp Suite, OWASP Top 10, Web Security, Web Application Testing, and Penetration Testing.
