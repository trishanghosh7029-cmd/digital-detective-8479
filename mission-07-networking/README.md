# Mission 7 — How computers communicate

## 1. Task / objective

Explain basic network concepts, observe connectivity and DNS lookup behavior, and describe what happens when a website opens.

## 2. Work completed

### Task 7.1 — Network concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN | A network covering a small area such as a home, lab or office. | Devices connected through the same local router |
| MAN | A network covering a city or a large campus area. | A university-campus network that spans several buildings |
| WAN | A network covering large geographical areas. | The Internet and networks joining distant offices |
| DNS | Translates a domain name into network address information. | Resolves `example.com` to address records |
| Router | Connects networks and forwards network traffic between them. | A home router forwards traffic toward the Internet |
| Protocol | A defined set of rules and formats for communication. | HTTP or HTTPS governs browser requests and responses |
| Packet switching | Divides data into packets that are delivered across network segments. | A website response may arrive in multiple packets |
| Client-server | A client requests a service and a server provides it. | A browser requests a page from a web server |

### Task 7.2 — Network observations

A connectivity test was run with `ping -c 1 example.com`. One test packet was sent and received, with no packet loss. This shows that the current network path could reach the public example domain at that moment. It does not prove that every service on every host is available.

A DNS lookup was run with `dig +short example.com`. It returned public address records associated with the domain. DNS lookup output is dynamic and may differ by network and provider.

- A connectivity test helps check whether a host or route can respond to network traffic.
- A DNS lookup displays network address records that correspond to a domain name.
- When a website name is entered, DNS resolves the name into an address so the browser knows where to request the content.

### Task 7.3 — What happens when a website opens

1. The browser acts as a client and reads the entered domain name and protocol.
2. The browser asks DNS to resolve the domain name into one or more network addresses.
3. Using the resolved address, the browser sends a request through a local network and router toward the server.
4. Routers and switches forward packets across networks using routing and packet-switching rules.
5. A server for the domain receives the client request through a protocol such as HTTP or HTTPS.
6. The server processes the request and sends a response containing HTML and other resources.
7. The browser receives the response packets, reassembles the data and displays the page while loading any additional resources.

## 3. Commands / tools used

- `ping -c 1 example.com` — checks whether one packet reaches the public example domain.
- `dig +short example.com` — retrieves public DNS address records.
- Text editor / Markdown — documents the concepts and observations.

## 4. My understanding

Networks provide communication paths, DNS provides name-to-address lookup, and routers forward traffic between networks. Protocols define how devices exchange data, and packet switching allows data to travel in smaller units. The browser-server model is a client-server interaction.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- Privacy-safe observations in this README
- No personal IP address or local network details were retained

## 8. Commit details

- Meaningful commit message: `Explain networking concepts and website communication`