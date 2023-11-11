#### revision
the five phases of ethical hacking are 
1. information gathering
2. scanning
3. gaining access
4. maintaining access
5. cleaning track/log
penetration testing: checking for vulnerabilities.
security audit:  is a systematic evaluation of a company's information systems, networks, and physical infrastructure.
vulnerability assessment: checking a systems security against a list of vulnerabilities.
intranet:- a private network for an organization with their own website.
internal pentesting:- pentesting an intranet for an organization.
external pentesting:- pentesting a website available for the public.
ping sweep exists on the network layer.
if a system is sending a ping with byte 64 the system is Linux. if it is 32 the system is windows.
ttl:- time to leave
`nmap -Pn IP` escapes checking if the ip is up or down and checks if the ports are open.
`sudo nmap -sS IP` stealth scan in nmap.
`sudo nmap -sU IP` UDP scan in nmap.
we can use `nmap -sU -sS -sV IP` to find ip's hidden in one but found in the other.
`sudo nmap -sX IP` Xmas scan
`nmap -sC IP`