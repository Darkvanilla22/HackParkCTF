# HackParkCTF
TryHackMe write-up for the HackPark CTF room

As per TryHackMe's description of this room, "This room will cover brute-forcing an accounts credentials, handling public exploits, using the Metasploit framework and privilege escalation on Windows".

With that out of the way, let's begin.

As usual, we start by running a scan onto the machine to discover any open ports for us to exploit:

![image](https://user-images.githubusercontent.com/53369798/112157389-8ae0cc00-8bbd-11eb-81d3-28a2a5196de2.png)

And here are the results to that scan:

![image](https://user-images.githubusercontent.com/53369798/112157655-d1362b00-8bbd-11eb-8439-72f49528158f.png)

As you can see, there are two open ports: **80** and **3389**. Out of the two ports, we can check out port 80, which is the default port for HTTP. Here's the homepage of that given website:

![image](https://user-images.githubusercontent.com/53369798/112157932-12c6d600-8bbe-11eb-893d-351681808d0d.png)

Let's see what options are open to us in terms of basic browsing:

![image](https://user-images.githubusercontent.com/53369798/112162187-37bd4800-8bc2-11eb-92b9-582c8c4154a9.png)

After visting all of the links presented to us, I've determined that the login page is the most interesting of the bunch. We could try to break into an account through this form:

![image](https://user-images.githubusercontent.com/53369798/112166027-a5b73e80-8bc5-11eb-8425-398e1d5de378.png)

