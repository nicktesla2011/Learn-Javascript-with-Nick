# Learn-Javascript-with-Nick
Learn the basics of Javascript through example scripts
Javascript Video button Readme

***In-line Javascript Video with play and pause button***

In this example you will write an inline script that will <br>
1. create the 2 buttons to "play" and "pause" the video.<br>
2. embed a video frame into your HTML document.<br> 
3. set the address of the source for the video.<br>
4. Create 2 code blocks "functions that will address the following…<br>

Get the video by it's elementID and assign the "Play button" to actually play the video.<br>
The second function will pause the video.

**How to do this**

Open up your barebones HTML template that can be found in this repository.

Step 1. let's create the buttons.
This is done not by javascript but by HTML5
<button onclick="playVid()" type="button">Play Video</button>
It creates a nice little basic button but when you click on it all it does is respond like a button push but nothing happens.

Much like a light switch in a house where you need to wire the switch to the light and the main power source. 
We need to do the same thing here.

Step 2. Next we need to establish where the video will be stored or where can the buttons address the video so you can control it.
You do this by using the HTML5 Video Tag <br>
```<video>```
The first use of this tag will be to establish the size of the video window by writing this…
```<video id="myVideo" width="320" height="176">```

This sets up a window that is 320 pixels wide by 176 pixels high and labels the video for our scripts purposes as "myVideo" you can change that name to any name you want.

next we will add the source or where this video is living on your computer or your server.
To do this we add the following tag
```<source src="filename.mp4" type = video/mp4>```

This basically says you want to play a particular video that has been saved in mp4 format.
We will not get into too deep on video formats in this tutorial but for your basic info there are 
mp4 and ogg formats that will cover the bulk of the mobile devices out there.
To add the .ogg file source just type this
```<source src="filename.ogg" type = video/ogg>```

And as a courtesy if your user is using an old browser you also add the line 
```Your browser does not support HTML5 video.```
Then close it all up with a closing video tag.
```</video>```

This part of your HTML page should then look like this.

```<video id="myVideo" width="320" height="176">```
  ```<source src="mov_bbb.mp4" type="video/mp4">```
  ```<source src="mov_bbb.ogg" type="video/ogg">```
  ```Your browser does not support HTML5 video.```
```</video>```

***Now for the Javascript***
Between the ```<script> ``` tags in your HTML template 
You will set up your functions or wire the buttons to the video so it will do something.

Javascript Functions have their own anatomy, and if you can remember these basics it will be easy to set them up every time.

For this simple button function you will have the following<br>
**A Constructor** ```function playvid```<br>
This sets up the function and gives it a unique name<br>
**A Call** ```()```<br>
Only functions have this property. It’s invoked via () to internally execute function body code<br>
**Code Block** ```{ anything that goes between these curly braces}```<br>
Usually an instruction.
