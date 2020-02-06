# MotionScents(NWHacks2020)
> Gestures to control essential oil diffusers

## Roles:
Ali- interfacing raspberry pi and the web app using python.

Ritvik- Developing and training a gesture recognition model using Google's autovision api as well as setting up communications with the web app and GCP.

Edwin - Responsible for developing a node js web app from scratch.

Adam - Responsible for configuring the raspberrypi and the diffuser.

## Inspiration

Gestures are powerful and easy! We decided to try utilizing the power of our gestures to control essential oil diffusers! Different gestures are captured using a node js web app, which interface with the google cloud autovision ml engine to train a model using the new gestures.

## What it does

Using the raspberry pi 4 and ultrasonic distance sensors, the raspberry pi tracks our motion and triggers the essential oil diffuser to turn on (ultrasonic transducer), releasing the scent you want into the air!

## How we built it

We used python and raspberry pi to control the different sensors. We used the data from the ultrasonic distance sensor to determine whether or not the diffuser should be turned on and for how long. The code is set up to scale so that it will be possible to control multiple diffusers. This way the user can choose specific scents to be released instead of only one SCENT. We utilized google cloud's vision api in order classify gestures and train a model that has a high success rate. In order to train the model, we used multiple datasets and classified certain gestures to default actions, which would serve as a starting point.

## Challenges I ran into

We initially aimed at using a camera module to capture the motions, but didn't have the right hardware to make it interface properly. We utilized the google cloud platforms Machine Learning API to train some data sets. After hacking it together we found the camera module didn't produce clear enough photos for the Machine Learning algorithm. We also did not have a monitor to display the raspberry pi desktop and as a result, had to develop everything using SSH into the Linux terminal...As a result, development was slower than anticipated.

## Accomplishments that I'm proud of

We successfully captured data from the distance sensor and triggered the diffuser to power on. We were also successful in capturing photos using the camera module but we decided not to pursue this route.

## What I learned

We learned how to use the google cloud machine learning API as well as how to program the raspberry pi through the terminal (none of us had used the Pi before). We also learned how to capture images through the web.

* Electronics
* Coding for Adriano
* Headless RaspberryPi
* Machine learning with Google cloud

## What's next for MotionScents

We'd like to try with a camera module again. We'd also like to try setting up multiple diffuser modules at the same time!
