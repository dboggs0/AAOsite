# The Automatic Apparel Outliner Project
 |[Overview](#Overview)|[Installation](#Installation)|[Accessing The App](#Accessing\ The\ App)|[Using The App](#Using\ The\ App)|
 |:---|:---|:---|:---|

## Overview
Automatic Apparel Outliner (AAO) web app is designed to draw outlines around the section of images
containing articles of clothing in photographs. 

This site provides information regarding the AAO project.

![DemoImage1](Capture1.PNG "demoImage1")
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

