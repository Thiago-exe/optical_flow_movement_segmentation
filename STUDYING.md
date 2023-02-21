# Study Report
Here, we'll discuss the theory behind optical flow and the Lucas-Kanade and Horn-Schunck techniques.

## What is optical flow? What is it used for?
The technique known as Optical Flow allows certain points of a video frame to be located in a previous frame. This is the initial step, for example, to determine the displacement of a vehicle between two consecutive video frames. More objectively, optical flow is the apparent movement pattern of image objects between two consecutive frames caused by object or camera movement. It is a 2D vector field, where each vector is a displacement vector, showing the movement of points from the first frame to the second.

## How to determine it?
### The Lucas-Kanade method
Before detecting the object, the vector field around the defined point is mapped, and this happens every new frame the object moves in the video. The Lucas Kanade method assumes that the displacement of the image content between two close instants (frames or frames) is small and approximately constant taking into account the pixels neighboring a point p.

Thus, optical flow, at a higher level definition, is the movement of objects between consecutive frames of sequence, caused by relative movement between the object and the camera. We can express the optical flow as follows:

![](https://miro.medium.com/v2/resize:fit:828/format:webp/1*dhdDZiBOshg6Xwx2_40N2Q.png)

Between consecutive frames, we can express the intensity of the image (I) as a function of the point (x,y) and time (t). Thus, if we extract the first image I(x,y,t) and move its pixels represented by (dx, dy) under time (t), we will obtain a new image I(x+dx, y+dy). that an object's pixel intensities are constant between consecutive frames.

![](https://miro.medium.com/v2/resize:fit:750/format:webp/1*7bpJR8sAVGH2ZB5l3ftNpg.png)

### The Horn-Schunck method


## References
- [Rastreamento de Fluxo Óptico com OpenCV - Medium (in Portuguese)](https://estevestoni.medium.com/rastreamento-por-fluxo-óptico-com-opencv-aa6302630f7c)
- []()
- []()