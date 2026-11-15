# Mission 7 — How computers communicate

## 1. Task / objective
Explain basic network types and concepts, observe network lookup and connectivity information, and describe what happens when a website opens.

## 2. Work completed

### Task 7.1: Network concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN | A network covering a small area like a home, lab or office | Wi-Fi at home connecting my phone and laptop |
| MAN | A network covering a city or a large campus | A college campus network linking all its buildings |
| WAN | A network covering a very large geographical area | The internet connecting countries |
| DNS | Translates a domain name into an IP address | Turning example.com into a number the computer can use |
| Router | Connects networks and forwards data between them | The Wi-Fi router at home |
| Protocol | A set of rules devices follow to communicate | HTTPS for secure web pages |
| Packet switching | Data is split into small packets that travel across the network and are put back together | A video call sent as many small packets |
| Client-server | A client requests a service and a server provides it | My browser asking a website's server for a page |

### Task 7.2: Network observations
I ran `ping -c 4 example.com` and `nslookup example.com`. My network details are redacted for privacy.

- **Connectivity test:** the ping test checks whether my computer can reach another computer on the network and how quickly it replies. [Result: 4 packets transmitted, 4 packets received, 0.0% packet loss]
- **DNS lookup:** nslookup shows the IP address linked to a domain name. For example.com it returned an IP address. [####]
- **Role of DNS:** when I type a website name, DNS converts it into the IP address of the server, because computers communicate using addresses and not names.

### Task 7.3: What happens when I open a website
1. I type a website address into my browser, which acts as the client.
2. The browser asks DNS to translate the domain name into an IP address.
3. The browser sends a request, following a protocol such as HTTPS, from my computer to my router.
4. The router forwards the request across the network and the internet to the server with that IP address.
5. The server receives the request and prepares the web page.
6. The server sends the page back as packets, which travel through the router to my computer.
7. My browser puts the packets together and displays the web page.

## 3. Commands / tools used
- `ping -c 4 example.com` – tested whether my computer can reach the website
- `nslookup example.com` – looked up the IP address of the domain
- Tools: VS Code, zsh terminal