## The image

Task: We found this image on a website, and there seems to be something redacted. Could you help us figure out what they tried to hide?

The task provides you with a image.svg
![8c22999a63b6491ea615d3c4556b0d3a.png](../images/8c22999a63b6491ea615d3c4556b0d3a.png)

I ran xxd on the file but in the end what worked better was simply to open the image with a text editor.
I notice there is a base64 encoded image there:
![6124dd0d25314a2e9ec36f3cabc22f22.png](../images/6124dd0d25314a2e9ec36f3cabc22f22.png)

It represents the black stripe blocking the flag.
 ![982b5655e97e48e785483e4c3b1dd7b3.png](../images/982b5655e97e48e785483e4c3b1dd7b3.png)
 
I can simply remove it and save the file to see the flag:
 ![095dfd453894484aa68739715f229d45.png](../images/095dfd453894484aa68739715f229d45.png)