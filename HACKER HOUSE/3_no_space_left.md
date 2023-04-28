## No Space Left

Task: Once in a remote Norwegian town, a group of skilled security professionals had convened in a fancy cabin to collaborate and achieve their objectives. On their network, they found a number of challenges that required their collective expertise. Do you have what it takes to tackle these challenges too?

This time if I try `127.0.0.1|ls` I get an error:

![33c3bb6cd12e43db8f0431baea1c678b.png](../images/33c3bb6cd12e43db8f0431baea1c678b.png)

I noticed many symbols where being blocked (and spaces as well) but `<` was not. I had to use Burp though, otherwise if I supplied my input through the UI, it tampered the request. 
%0a also works. 

![4770b5a766ff436c924ba35768f75828.png](../images/4770b5a766ff436c924ba35768f75828.png)

In the end the payload was
`ip=127.0.0.1%0acat<./../../../flag.txt`

![832b8b5011614d1197cc6645873ec7c2.png](../images/832b8b5011614d1197cc6645873ec7c2.png)

