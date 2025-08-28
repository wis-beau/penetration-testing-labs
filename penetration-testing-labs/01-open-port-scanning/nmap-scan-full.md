# Sample of Nmap Full Port + Service Scan (raw)
PORT	STATE 	SERVICE
21/tcp	ftp	open
22/tcp	ssh	open
23/tcp	telnet	open
25/tcp	smtp	open
53/tcp	domain	open
80/tcp	http	open
111/tcp	rpcbind	open
139/tcp	netbios-ssn	open
512/tcp	exec	open



>
> Example headers you should see:
> - `Host is up` line with latency
> - A list of `open` ports with service names & versions
> - `Service detection performed...` footer
