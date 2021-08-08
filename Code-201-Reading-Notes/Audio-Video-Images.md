# HTML Video & Audio


## Video File Formats
* New browsers have evolved to support the HTML5 `<video>` tag, however old browsers require a program or player to be installed in order to play video content. These players and plugins only support certain formats
* To make sure most people can play your video the best practice is to use the `<video>` tag along with flash video, for browsers that don't support HTML5.
* To use flash we need to upload videos in at least two different formats: WebM and MP4
* There are apps and websites available online that allow you to encode videos 

## Hosted Video Services
* An easy way to add videos to a webpage is to use a hosted video service which is supported by mos browsers
* Hosted video services are websites like YouTube and Vimeo, they allow us to upload videos in a range of different formats. Then after uploading, they convert the video into the formats that are required by different browsers, and they provide features that allow us to embed the video 
* There are some disadvantages to using hosted web services such as:
    - some services have guidelines which limit what we can include in our videos
    - they usually play ads before and during the video
    - quality of the video can be limited
    - the content will not be exclusively available on our webpage since it's also available on the site of the hosted service
## Adding Audio To Webpages
* MP3 is the most popular format for adding  audio to a webpage
* There are three routes we can take to add audio to a webpage
1. Use a hosted service that lets us upload audio and provides a player that we can embed in our page.

2. Use Flash (difficult to achieve and obsolete).

3. Use the HTML5 `<audio>` tag which provides its own controls.

# HTML Images

## Adding Images To A Webpage
```
<img>- this is the element that we will use to
add a image to our page

Src- another component of the image element is src,
which tells the browser where to get the image file.


alt- This is where we can provide a text description
of the image which describes the image if someone can not
see it


title- We can also use the title attribute to the 
<img> element if we want to provide additional information
about the image. Most browsers will display this text
when the user hovers over the image
```
Here is an example of the syntax that is used to
add an image to a page in HTML:

```
<img src="your-image-url-here.jpg" alt="A text description of your image goes here" title="Your image title goes here"/>
```

Definitions in this section were derived from Chapter 5: “Images” (pp.94-125)
of the textbook *HTML & CSS Design And Build Websites* By Jon Duckett

# HTML & CSS: Practical Information