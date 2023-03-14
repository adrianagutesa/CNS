# Lab Title: Man-in-the-middle attacks (ARP spoofing)

## Challenge Answers

- **Challenge 1:** [Insert answer here, i.e., a Chuck Norris fact]
- **Challenge 2:** [Insert answer here, i.e., a `password` to unlock the next lab]

## Other Relevant Information

[Insert here, if applicable]

## Lab Prep Questions and Answers
1. What is the *Address Resolution Protocol (ARP)*, and what is its role in a network?
    - Address Resolution Protocol (ARP) is a communication protocol used to find the MAC (Media Access Control) address of a device from its IP address and vice versa. This protocol is used when a device wants to communicate with another device on a Local Area Network or Ethernet.
2. What is a *Man-in-the-Middle (MitM)* attack, and how does ARP spoofing enable it?
    - A man in the middle (MITM) attack is a general term for when a perpetrator positions himself in a conversation between a user and an application, either to eavesdrop or to impersonate one of the parties, making it appear as if a normal exchange of information is underway. ARP spoofing enables the attacker to find out the MAC address of the user.
3. How does an attacker use ARP spoofing to intercept network traffic?
    - In ARP spoofing the attacker sends forged ARP Messages which allows him to pretend as a legitimate user as it links the attacker machine’s MAC Address to the legitimate IP Address. The whole communication is redirected over an attacker and he can supervise it.
4. How is the *cookie* used to derive the encryption/decryption key?
    - The *cookie* is used to generate a secret key. This secret key is then used for encryption and decryption of the messages.
5. What REST API request do you need to send to the *crypto oracle* the secret cookie?
    - GET /arp/cookie
6. How do you obtain the authentication token?
    - The authentication token is obtained by sending a POST request to **************crypto oracle************** server. The request should include the username and password in the body of the request.
7. How do you use the authentication token to obtain the cookie?
    - To use the authentication token to obtain the cookie, we need to send a REST API request with the authentication token included in the headers of the request. Only then can we obtain the cookie.
8. What encryption mode is used to encrypt the challenge in this lab?
    - AES-CBC (AES cipher and CBC encryption)
9. What tool can you use to capture network traffic on a local network interface?
    - tcpdump
