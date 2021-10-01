# Research_doc
  
- [x] Blink Detection Research -> Method 2
- [x] Posture Detection Research -> Method 1
- [x] Face Mapping Research -> Use Dlib library
- [x] Changing Brightness Research -> screen-brightness-control
- [ ] Room Brightness Detection + Suitable Brightness for Eyes Research
- [ ] Let app run in background Research + Figma landing page
- [ ] Optimization for Computer Vision Programs Research + Figma application interface
- [ ] Average Blinking Rate Research + AI for Counting Blinking Rate Research
- [ ] Tech-stack for Project
  
Complete Documentation: [Docs](https://docs.google.com/document/d/1TrskTl7OxPtWn8PP7vaKnlWTEtmCDBYORCT_bzEswEM/edit)
  
## Blink Detection Research
Language: Python  
Library: OpenCV (for camera access) + Dlib (for face detection)  
Methods:  
    
**1st Method: Detect face, Get position of eyes using trained data, Count blinks**
> Steps:  
> 
> > Capture/Load Video  
> Convert to grayscale  
> Get landmarks for the eyes  
> Calculate the blink ratio  
> > Detect Blinks  
> 
> URL: [Here](https://medium.com/algoasylum/blink-detection-using-python-737a88893825)  
  
**2nd Method: EAR (Eye Aspect Ratio)**
> Steps:  
> 
> > Detect desired 6 position of the eyes (P1-P6)  
> > Calculate EAR using the formula  
> 
> URL: [Here](https://www.pyimagesearch.com/2017/04/24/eye-blink-detection-opencv-python-dlib/)  
> ALternative URL: [Here](https://github.com/nWhovian/blink-detection)  

Conclusion: Both methods are roughly the same, we can test both and find which one performs better (Accuray and Loading Time)  

## Posture Detection Research
Language: Javascript and Python
Library: OpenPose (Python)
Methods:

**1st Method: Use front face for posture detection (JS)**
> Steps:
>
> > Uses a camera to detect the distance between the screen and the head rotation in 3D
> > Uses the tracking data to determine if the user is having the correct posture or not
> > There will be an alarm sound if the user is having incorrect posture
>
> URL: [Here](https://sit-straight.glitch.me)  
> Source code: [Here](https://github.com/abhilash26/sit-straight)  

**2nd Method: Use OpenPose Library**
> Steps:
>
> > Count proximity to the screen
> > Detect slump
> > Detect forward tilt
> > Detect head tilt
> > Detect shoulder tilt
> > Count shoulder width
>
> URL: [Here](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
  
Relevant Links:  
[Raspberry pi X Open CV](https://www.element14.com/community/community/project14/photography/blog/2021/08/28/posture-detection-using-opencv-and-raspberry-pi-hq-camera-kit)  
[Build your own posture corrector](https://betterprogramming.pub/build-your-own-posture-corrector-with-pose-estimation-97009943e484)  
[Youtube Link](https://www.youtube.com/watch?v=bdTSzvUE1QQ)  

## Face Mapping Research
Language: Python  
Library: MediaPipe, Dlib and OpenCV  
Methods:

**1st Method: Combine libraries function to map face**
> Steps:  
> 
> > Use webcam/camera as video input  
> > Convert to gray scale  
> > Detect the faces  
> > Find landmark for each face  
> > Show the face  
>  
> URL: [Here](https://towardsdatascience.com/facial-mapping-landmarks-with-dlib-python-160abcf7d672)  
> Extra Information: [Here](https://google.github.io/mediapipe/solutions/face_mesh.html)  

## Changing Brightness Research
Language: Python  
Library: screen_brigthness_control
Methods:

**1st Method: Get and change current laptop's brightness**
> Steps:  
>   
> > Directly use built-in function from the library  
> > set_brightness(), fade_brightness(), get_brightness()  
>   
> URL: [Here](https://www.geeksforgeeks.org/how-to-control-laptop-screen-brightness-using-python/)  
> Extra Information: [Here](https://pypi.org/project/screen-brightness-control/)  
> Demo video: [Here](https://drive.google.com/file/d/19nZ9jqwWBncfsFb14kqpV2G3FHmB0dkk/view?usp=sharing)  

## Tech-stack Research
For the building of this project, we plan to create one product and one landing page in order to showcase the product.  
Landing page:  
- Frontend -> ReactJS, HTML, CSS, JS
- Backend (Optional) -> NodeJS, Express
- UI/UX -> Figma
  
Product:
- ML/DL/CV Mode -> Python
- App development -> (?)
