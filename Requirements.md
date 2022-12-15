Flow: capture (3D scan) -> process (Houdini) -> VR (unity) [passive interaction]                  

                                             -> VR (gravity sketch) [active creation/interactive]  -> Output (3D Model)


## Capture (physical to digital)

There are several methods that can be used to capture 3D space, including the following:

1. [[Photogrammetry]]

2. [[Laser scanning]]


3. Structured light scanning: This is a method of capturing 3D data using a pattern of light. The pattern is projected onto the object or scene, and a camera is used to capture images of the distorted pattern. Specialized software is then used to process the images and create a 3D model.

4. Depth sensors: Depth sensors are specialized sensors that can be used to capture 3D data. They work by emitting a signal and measuring the time it takes for the signal to bounce back. This allows the sensor to create a detailed 3D map of the environment.

5. Time-of-flight cameras: These are cameras that use the time it takes for a light pulse to travel to an object and back to calculate the distance to the object. This allows the camera to create a 3D map of the environment.


6. Stereoscopic cameras: These are pairs of cameras that are mounted side by side and capture images from slightly different angles. The images are then combined to create a 3D image.

  

7. Motion capture: This is a method of capturing the movement of objects or people in 3D. It typically involves attaching markers to the objects or people and using sensors or cameras to track the markers in 3D space.


- 3D scanning

    * Photogrammetry

        - [HW] Drone

        - [HW] Smartphone

        - [SW] Polycam

    * LIDAR

        - [HW + SW?] Matterport Pro3 (6k USD)

        - [SW] Polycam

- Sensing (mapping the invisible)

    * sensors

    * programming platforms

- 3D model (manually)

    * [SW] Blender

- Available 3D models

    * [SW] renderdoc (extract 3D view currently rendered on the GPU, e.g., Google Earth/Maps)

  

## Processing

  

### Pre-processing (e.g., correct format)

Everything that needs to be done before we can start the creative processing. This needs to be done ALWAYS.

  

- Mapping sensor values to 3D position/location (mapping sensor to captured 3D space (aligning coordinate system))

- Extract sensor data from various sources

    * define structure of sensor values in Houdini (auto retrieve)

- Pre-process 3D models (obj, fbx format + png/jpg texture)

    * [keep meshes] Polyreduce (to reduce the size and computational intensity) in-house Python process

    * [keep point clouds] in-house Python process

    * [Renderdoc-specific pre-processing]  in-house tool chain

        - import in Blender (with plugin)

        - Export to houdini

        - run in-house pipeline

            -> make pointcloud

            -> make mesh

  

### Visualisation/Modelling (for VR)

- Houdini

- Blender

- Unity

- Unreal

  

### Processing in VR / VR-aided processing

                Quest   PC VR   PSVR    Drawing     Modelling     Animation

Tilt Brush      ✔       ✔       ✔      ✔          ✖             ✖

Dreams          ✖       ✖       ✔      ✖          ✔             ✔

Quill           ✖       ✔       ✖      ✔          ✖             ✔

Adobe Medium    ✖       ✔       ✖      ✖          ✔             ✖

Gravity Sketch  ✔       ✔       ✖      ✖          ✔             ✖

Tvori           ✖       ✔       ✖      ✖          ✔             ✔

AnimVR          ✖       ✔       ✖      ✔          ✖             ✔

Blocks          ✖       ✔       ✖      ✖          ✔             ✖

SculptVR        ✔       ✔       ✔      ✖          ✔             ✖

Masterpiece VR  ✖       ✔       ✖      ✖          ✔             ✔

Adobe Substance ✖       ✔       ✖      ✖          ✔             ✖

3D Modeler (closed beta)

blender plugin

  

## Post-production / Output

- Animations

- 2D print from 3D model (blender render)

- 3D printing

- laser cut

![[CM3 makerspace.png]]