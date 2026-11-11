# Quality Attributes of Three Apps

| App | Attribute | Why it matters | What it trades off |
|---|---|---|---|
| WhatsApp | Performance (latency) | Businesses depend on fast messages for customer communication and deals; late messages lose business. | Fast delivery needs more servers close to users and always-open connections, which cost money and phone battery. |
| WhatsApp | Security and privacy (including consent) | Personal and business information must be protected, and sharing data with third parties needs the user's consent. | Encryption and consent steps add processing and complexity, and they limit features (if the server can't read messages, search and moderation are harder). Users see more steps. |
| WhatsApp | Availability (added) | If the app is down for an hour, businesses can't reach customers. | Spare servers in several regions cost more. During a network split (CAP), the app may show slightly old messages instead of an error. 

| YouTube | Performance (latency) | Videos should start quickly, and live streams should have little delay, because creators and companies announce things there. | Better speed means compressing video (lower quality) and paying for servers placed near viewers worldwide. |
| YouTube | Security | A hacked official channel can upload false content and damage a person's or company's reputation. User data must also be protected. | Extra checks (two-step login, upload verification) slow creators down and annoy users, and monitoring costs money. |
| YouTube | Scalability | Billions of viewers watch and many people upload at the same time. If servers are overloaded, users lose trust. | Large infrastructure costs a lot. Some data, such as view counts and comments, may lag slightly behind (eventual consistency) so the system stays fast. |

| Uber | Performance (latency and accuracy of real-time data) | If the app says the driver has arrived but they haven't, the rider is confused and loses trust. | Frequent location updates drain battery, use mobile data and put load on servers. |
| Uber | Security and privacy | Riders and drivers share location and phone numbers, and misuse of that data destroys trust. | Hiding phone numbers (calls through the app) adds cost and complexity, and identity checks make sign-up slower. |
| Uber | Scalability | Rush hour or a big event creates a spike of requests. If the system is overloaded, nobody can book a ride. | Servers that sit idle outside peak times cost money. Auto scaling reduces this but adds complexity. |
| Uber (bonus) | Usability (learnability) | Non-technical users and local-language users must be able to book a ride easily. | A very simple screen hides advanced options, and supporting many languages costs effort to build and maintain. |
