KRISH — COMPUTER NETWORKS PROJECT — PHASE 1 EVIDENCE
==========================================================

These screenshots were extracted from CN_Lost_Packets.pdf and renamed to match
the terminology and evidence requirements in the provided CN Project document.

1. 01_Mac4_LAN_Ping_Reachability.png
   Task A — Establish the Private LAN.
   Shows ping reachability from Mac 4 to the other LAN machines.

2. 02_Mac4_WiFi_Network_Details.png
   Task A — Private LAN / network information.
   Shows the active Wi-Fi interface and network details.

3. 03_Mac4_IP_Subnet_Gateway_Interface_MAC.png
   Task A — Record machine network information.
   Shows IPv4 address, subnet mask, gateway, interface and MAC address.

4. 04_Mac4_Private_DNS_Resolution_dig.png
   Task B — Configure a Private DNS Server.
   Shows `dig @10.7.19.168 app.team1.test` resolving the private domain
   to 10.7.14.3.

5. 05_Mac4_DNS_Resolution_Troubleshooting.png
   Task B — DNS troubleshooting / resolution verification.
   Shows an initial DNS/socket issue followed by successful resolution.

6. 06_Mac4_HTTPS_TLS_Certificate_Validation_Failure.png
   Task E — HTTPS / TLS.
   Shows curl reaching the HTTPS service and the certificate trust/validation
   failure. This is useful as setup/troubleshooting evidence, NOT as the final
   successful HTTPS demonstration.

7. 07_Mac4_HTTPS_TLS_HTTP_Request_Success.png
   Task E + Task G — HTTPS/TLS and complete protocol flow.
   Shows successful TLS handshake, certificate verification, HTTP/2 request,
   response headers and backend response.

8. 08_Mac4_DNS_and_Backend_B_Startup.png
   Task B + Task C — DNS testing and backend service setup.
   Shows DNS resolution activity and Backend B being started/listening.

9. 09_Mac4_Backend_A_API_Response_X_Backend_Header.png
   Task C / backend API verification.
   Shows a direct backend API response with `X-Backend: A`.
   Note: this screenshot is not the required final load-balancing proof,
   because the project requires repeated requests through the nginx edge.

IMPORTANT:
- The CN project document says Phase 1 evidence should include DNS resolution,
  curl/browser output with headers, Wireshark DNS/TCP/TLS captures, HTTP caching,
  and failure demonstrations.
- These are only the screenshots present in CN_Lost_Packets.pdf. No screenshot
  has been invented or added.
