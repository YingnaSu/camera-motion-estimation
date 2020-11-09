# camera-motion-estimation
## globally optimal relative pose estimation with gravity prior
After aligning the y-axes of the views with the gravity direction,
<img src="https://github.com/YingnaSu/camera-motion-estimation/tree/main/image/align.png" width="600" height="180"/>

the essential matrix with single-axis rotation satisfies:
<img src="https://github.com/YingnaSu/camera-motion-estimation/tree/main/image/eq1.png" width="100" height="20"/>

We present a novel algorithm that gives the globally optimal solution to the relative pose estimation with known gravity direction by minimizing the algebraic error:
<img src="https://github.com/YingnaSu/camera-motion-estimation/tree/main/image/eq2.png" height="20"/>

The complete steps of the globally optimal relative pose estimation are as follows:
<img src="https://github.com/YingnaSu/camera-motion-estimation/tree/main/image/app.png" width="400" height="270"/>

## smart phone dataset for camera motion estimation
The Phone dataset contains more than 10,000 images for 6 sequences with synchronized gravity direction and ground truth motion parameters. The images were captured using an iphone 6s at the resolution of 1280x720@30Hz. The corresponding IMUs data were captured @100Hz with built-in sensor InvenSense MPU-6500. We synchronize the frames and IMUs data based on their timestamps. The motion parameters obtained from RealityCapture were used as the ground truth.
<img src="https://github.com/YingnaSu/camera-motion-estimation/tree/main/image/img.png" width="500" height="140"/>
