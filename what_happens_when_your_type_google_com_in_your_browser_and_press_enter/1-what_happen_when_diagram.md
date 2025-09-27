Based on the exercise requirements and the diagrams you've shared, here's how to enhance your blog post with a visual diagram for Exercise 1:

## Enhanced Blog Post with Diagram

# Everything's Better with a Pretty Diagram: The Complete Journey of https://www.google.com

When you type "https://www.google.com" in your browser and press Enter, a complex chain of events occurs in milliseconds. Here's what happens, illustrated with a comprehensive flow diagram.

## The Complete Request Flow Diagram

```
[User Browser] 
       |
       v
   1. DNS Resolution
       |
   [Local DNS] ──→ [Recursive DNS] ──→ [Root DNS] ──→ [.com TLD] ──→ [Google's Authoritative DNS]
       |                                                                        |
       v                                                                        v
   IP: 142.250.190.46 ←──────────────────────────────────────────────────────┘
       |
       v
   2. TCP Connection (Port 443)
       |
       v
   3. HTTPS/SSL Handshake 🔒
       |
       v
   4. [Firewall] ──→ [Traffic Filter & Security Check]
       |
       v
   5. [Load Balancer] ──→ [Distributes to available servers]
       |
       v
   6. [Web Server (Nginx)] ──→ [Serves static content & routes requests]
       |
       v
   7. [Application Server] ──→ [Processes business logic]
       |
       v
   8. [Database] ──→ [Retrieves user data & search results]
       |
       v
   [Response Journey Back Through All Layers]
       |
       v
   [Browser Renders Page]
```

## Detailed Flow Analysis

### 1. DNS Resolution 🌐
Your browser doesn't understand "google.com" - it needs an IP address. The DNS system acts like the internet's phonebook:
- **Local DNS cache** is checked first
- **Recursive DNS resolver** (usually your ISP's) queries the hierarchy
- **Root nameservers** point to .com servers  
- **TLD servers** direct to Google's authoritative servers
- **Result**: www.google.com → 142.250.190.46

### 2. TCP Connection Establishment 🔗
Once the IP is known, your browser establishes a TCP connection on **port 443** (HTTPS):
- **SYN** → **SYN-ACK** → **ACK** (three-way handshake)
- Connection is now ready for secure data transmission

### 3. HTTPS/SSL Encryption 🔐
Since you typed "https://", encryption is mandatory:
- **Certificate verification** ensures you're connecting to the real Google
- **TLS handshake** establishes encryption keys
- **All subsequent traffic is encrypted**

### 4. Firewall Protection 🛡️
Multiple firewalls protect the journey:
- **Your local firewall** checks outgoing connections
- **ISP firewalls** may filter malicious traffic  
- **Google's enterprise firewalls** protect their infrastructure
- **DDoS protection** shields against attacks

### 5. Load Balancer Distribution ⚖️
Google handles billions of requests daily, so load balancers are essential:
- **Geographic routing** sends you to the nearest data center
- **Health checking** ensures requests only go to healthy servers
- **Algorithm-based distribution** (Round Robin, Least Connections, etc.)
- **Automatic failover** if servers become unavailable

### 6. Web Server Response 🌐
The web server (likely Nginx or Google's custom software) processes your request:
- **Static content serving** (HTML, CSS, JavaScript, images)
- **HTTP header processing** 
- **Reverse proxy functionality** to application servers
- **Caching** for frequently requested resources

### 7. Application Server Logic 🧠
For dynamic content, application servers handle the heavy lifting:
- **Search algorithm processing**
- **User personalization** (if logged in)
- **Real-time data processing**
- **API orchestration** for various Google services

### 8. Database Queries 🗃️
The application server queries multiple databases:
- **Search index databases** for relevant results
- **User preference databases** for personalization
- **Advertising databases** for targeted ads
- **Analytics databases** for metrics collection

## The Return Journey
The response follows the same path in reverse:
1. **Database** returns query results
2. **Application Server** processes and formats data
3. **Web Server** packages the HTTP response
4. **Load Balancer** routes response back
5. **Firewall** validates outgoing traffic
6. **HTTPS encryption** secures the response
7. **TCP connection** delivers packets reliably
8. **Your browser** receives and renders the page

## Performance Metrics
This entire process typically completes in:
- **DNS Resolution**: 20-100ms
- **TCP Connection**: 20-100ms  
- **SSL Handshake**: 100-200ms
- **Server Processing**: 50-200ms
- **Total Time**: Usually under 500ms

## Why This Matters
Understanding this flow is crucial for:
- **Debugging network issues**
- **Optimizing web performance**
- **Designing scalable architectures**
- **Implementing security best practices**
- **Technical interviews** at major tech companies

## Diagram Tools Used
For creating technical diagrams like this, popular tools include:
- **Gliffy** (recommended by the exercise)
- **Lucidchart** 
- **Draw.io (now diagrams.net)**
- **Visio** for enterprise environments

***

This comprehensive flow demonstrates why the question "What happens when you type google.com?" remains a classic technical interview question - it touches on networking, security, scalability, and system design all in one seemingly simple action.

**Diagram Image URL**: [Your diagram URL would go here when you create it using Gliffy or another tool]