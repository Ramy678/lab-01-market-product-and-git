## Product Choice

Telegram
<https://web.telegram.org/a/>
communication app , that is well encrypted

## Main components

![Telegram Component Diagram code]("C:\Users\amier\OneDrive\Desktop\software-engineering-toolkit\lab-01-market-product-and-git\docs\diagrams\src\telegram\component-diagram.puml")
...

Mobile App (iOS/Android)
This is the primary client interface for end-users on smartphones, enabling messaging, media sharing, and feature access. It connects to Telegram’s backend via the MTProto Protocol to ensure secure, encrypted communication.
MTProto Protocol
A custom cryptographic protocol designed for secure and efficient data transmission between clients (e.g., mobile/desktop apps) and Telegram’s servers. It handles encryption, authentication, and low-latency message delivery to maintain privacy and performance.
Auth & Session Service
Manages user authentication, session validation, and security tokens to verify user identities and maintain active logins. It ensures secure access control while preventing unauthorized sessions across devices.
State Cache (Redis)
A high-speed caching layer using Redis to store frequently accessed data (e.g., user states, session tokens) for rapid retrieval. This reduces latency and database load by serving temporary data without repeated disk reads.
Bot API Server
Provides a dedicated interface for developers to build and interact with Telegram bots via HTTPS/Webhooks. It processes bot commands, messages, and updates, enabling automated interactions with users and integration into external workflows.

Mobile App (iOS/Android) MobileDeveloper

MTProto Protocol
Cryptographer

Auth & Session Service
Backend Engineer

State Cache (Redis)
DevOps Engineer

Bot API Server
API Developer

Mobile Developer:
Designs and implements native iOS/Android interfaces; integrates MTProto for secure messaging; optimizes performance for battery/network efficiency; handles media processing and offline storage; ensures smooth UX across device types.

Cryptographer:
Designs and audits encryption schemes (e.g., AES, RSA); implements secure key exchange and message authentication; analyzes protocol vulnerabilities; ensures forward secrecy and resistance to MITM attacks; maintains cryptographic standards compliance.

Backend Engineer
Builds secure login flows (phone/SMS verification); manages session lifecycle and token validation; implements rate limiting and brute-force protection; scales authentication across millions of concurrent users; integrates with user databases.

DevOps Engineer:
Configures and maintains Redis clusters for low-latency data access; sets cache eviction policies and TTLs; monitors performance/metrics; ensures high availability and failover; optimizes memory usage to reduce database load.

API Developer:
Designs RESTful/Webhook interfaces for bot interactions; processes incoming/outgoing bot messages and commands; handles webhook delivery and retry logic; enforces rate limits and authentication for third-party bots; documents endpoints for developers.

tech skills:
Python/Go/Java
HTTP/REST APIs
Git & CI/CD
Security Fundamentals

skill i will develope:
Python/Go/Java
