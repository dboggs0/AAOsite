# The Automatic Apparel Outliner Project
 |[ Overview ](#Overview)|[ Installation ](#Installation)|[ Accessing The App ](#Accessing\ The\ App)|[ Using The App ](#Using\ The\ App)|[ AAO GitHub ](https://github.com/sloanlipman/automatic-apparel-outliner)|[ AAO Dev Team ](#AAO\ Dev\ Team)|


## Overview
Automatic Apparel Outliner (AAO) web app is designed to draw outlines around the section of images
containing articles of clothing in photographs. 

This site provides information regarding the AAO project.

![DemoImage1](Capture1.PNG "demoImage1")
<br>
<br>
![DemoImage2](Capture2.PNG "demoImage2")

## Installation
1. Install Docker
    * Go to https://docs.docker.com/get-docker/ and download Docker for Mac/Windows/Linux 
    * Run the installer exe/bin to install Docker on the machine that will be the server
    * Run Docker app on the 
1. Install [Git](https://git-scm.com/downloads)
1. Clone the AAO repository:
    > $ git clone https://github.com/sloanlipman/automatic-apparel-outliner.git
1. Navigate to the directory containing the file called Dockerfile
1. Run the following command:
    > $ docker build .
1. The above comand will provide a docker image ID.  Use that image ID with the following command:
    > $ docker run \<imageID>

## Accessing The App
Once the docker image is running the app can be accessed through a web browser at the following address:

> http://\<Server IP Address>:12345/home

## Using The App

1. Click the “SELECT A FILE” button and select an image from your device to upload. The supported image file types are JPEG, PNG or BMP.

![SelectImage](SelectImage.PNG "SelectImage")
![SelectImagew](SelectImage2.PNG "SelectImage")

2. Once image is uploaded to AAO, it will show uploaded image on the left side and
segmented image on the right side. Segmented images have mutiple sections in different
colors detected by image classification algorithm. It allows AAO to distiguish between apparel section(s).

![ImageDemo1](ImageDemo1.PNG "Image Demo 1")

3. AAO allows users to customize the outline color and thickness. You can select any outline
color for the apparel by clicking the box next to “Select an outline color” under the Segmented
Image section. The default outline color is white.
Click on the box below the Segmented Image area to bring up the color selector.

![ImageDemo2](ImageDemo2.PNG "Image Demo 2")

4. To selecte the outline thickness click on the box below the outline color selector.  Availabile line thicknesses are small (one pixel wide), medium (3 pixels wide), and Large (5 pixels wide).

![ImageDemo3](ImageDemo3.PNG "Image Demo 3")

5. Select the region that corresponds to the to the desired type of apparel on the Segmented Image.  Once clicked the selected color will show in the box bellow the outline thickness selector.

![ImageDemo4](ImageDemo4.PNG "Image Demo 4")

6. Click on the "Outline Selected Segment" button at the bottom of the screen to generate the outlines.

![ImageDemo5](ImageDemo5.PNG "Image Demo 5")

7. The outlines can be removed in order to select a different outine color or thickness.  To do this click the "Clear Outlines" button.

8. The images can be downloaded by clicking the "Download Images" button.  Once done one or all of the following can be selected:
    * The original image
    * The original image with an outline
    * The segmented image
    * The segmented image with an outline

![ImageDemo7](ImageDemo7.PNG "Image Demo 7")

9. The selected images are downloaded as a zip archive.

![ImageDemo8](ImageDemo8.PNG "Image Demo 8")

## AAO Dev Team

### Sloan Lipman
* [LinkedIn](https://www.linkedin.com/in/sloan-lipman-b21b1626)
* [GitHub](https://github.com/sloanlipman)
* [Gmail](sloan.lipman@gmail.com)

### Akshata Marathe
* [LinkedIn](https://www.linkedin.com/in/akshata-marathe)

### Dave Boggs
* [LinkedIn](https://www.linkedin.com/in/daveboggs)
* [GitHub](https://github.com/dboggs0)

### Francisco Ozuna Diaz
* [LinkedIn](https://www.linkedin.com/in/francisco-ozuna)
* [GitHub](https://github.com/ciscojvr)
* [Gmail](cisco.ozuna@gmail.com)
