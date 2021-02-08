#### Week 1: XR Terminology & Applications

1. XR:

   a.  VR: Replaces Reality

   - Computer-generated, virtual environment

   - No real world view, only virtual

   - R = synthetic world

   b. AR: Enhanced Reality

   - Virtual world merged with physical world
   - Real + virtual, composite view
   - R = real world

2. Definitions of Mixed Reality

   a. Reality-Virtuality Continuum

   <img src=".\微信图片_20210102095942.jpg"/>

   b. Synonym for AR

   c. Combination of AR and VR

   d. "Stronger" version of AR

   e. Type of Collaboration

   f. Alignment of Environments

3. XR Technology Landscape

   a. Current situation of XR technology:

   - Over-promising promotional videos of new devices with minor differences.
   - Display resolution & Field of view (FOV) are key factors and many technical aspects are rapidly improving.
   - Hand, finger & eye tracking are standard and quite good now but there are still strong technical and design limitations.
   - Environmental understanding is still rather basic.

   b. Four classes of XR Technology

   - Devices

     (1) Standalone / Built-in: Quest, HoloLens, ...

     (2) Tethered / Adapter: Cardboard, Rift, Vive, ...

   - Platform

     (1) Specific: Oculus, Vive, Magic Leap, ...

     (2) Cross-platform: SteamVR, WMR, WebXR, ...

   - Applications

     (1) XR apps: Beat Saber, Snapchat, ...

     (2) Apps with XR views/ modes: IKEA, Amazon Shopping, ...

   - Tools:

     (1) Design: Tilt Brush, Quill, Aero, ...

     (2) Development: A-Frame, Unity, Unreal, ...



#### Week 2: XR Concepts & Technologies

1. VR:

   a. Key characteristics of VR:

   - Autonomy / Agency: head tracking, body input.
   - Natural Interaction: gestures & speech, head/controller input.
   - Presence: immersive, multi-sensory.
   - Virtual Environment: can explore something 3D and provides stereoscopic view.
   - Immersive Task: spatial interaction and sound.
   - Believable Experience: no need for photorealism.

   b. VR display:

   - Head-mounted (HMD)

   - Room-sized (CAVE)

     <img src=".\Intro to VR _ Coursera - Google Chrome 2021_1_2 12_05_59.png"/>

   c. Key concepts in VR:

   - Autonomy / Agency: 

     (1) The user can choose their own perspective on the scene

     (2) The user can choose to navigate the scene in many different ways

     (3) The user can choose to interact with any objects.

   - Presence & Immersion:

     (1) Place Illusion: "Am I there?"

     (2) Plausibility Illusion: "Is this happening?"

     <img src=".\微信截图_20210102162743.png" />

   - Embodiment & Avatars: How the user is represented in the VR world.

   - Cognition & Empathy: Give the user a good simulation of the real activity.

   - Proprioception & Motion Sickness: Give the user a natural experience of behavior and avoid motion sickness. 

   - Haptics & Pseudo-Haptics: The user is trained before using VR to know the position of different devices.

   - Boundary & Redirected Walking: Defining play area and find obstacles in the area.

   d. VR Technology
   
   - 360 Photos & Videos
   
   - Stereoscopic Displays: rendering a different view for each eye (Cardboard VR).
   
   - CAVEs: the user steps inside what is called a Cave Automatic Virtual Environment inside a CAVE. 
   
   - 3 DOF and 6 DOF Tracking:
   
     (1) 3 DOF: Cardboard VR, the user can only rotate the head.
   
     (2) 6 DOF: The user can move along axes as well as rotating the head.
   
     <img src=".\微信截图_20210102194604.png" />
   
   - Outside-In and Inside-Out Tracking:
   
     (1) Outside-In: There are some sensors in the environment that point toward the user and they track the user has he moves around in a certain area that is covered in these sensors.
   
     (2) Inside-Out: The cameras and sensors are built into the device. This performs better when there are occlusions.
   
   - Hand Tracking
   
   - Spatial Audio
   
2. AR:

   a. Key characteristics of AR

   - Combines real and virtual: composite view, not just visual object.
   - Interactive in real time: explicit and implicit interaction.
   - Registered in 3D: align real and virtual objects, virtual objects is rendered according to their positions in real world.
   - Blending of environments: can view virtual objects merged with real world.
   - Information task: virtual objects encode information in real world.
   - Hologram illusion: virtual objects appear as if part of real world.

   b. AR displays:

   - Head-worn
   - Spatial
   - Hand-held
   - Monitor-based: look at the screen and the scene is rendered according to the position of user, similar to a mirror.

   <img src=.\微信截图_20210102202124.png" />

   c. AR concepts:

   - Augmentation & Mediation:

     (1) Augmentation: information overlays, spatially anchored objects, spatial audio, add virtual objects to the environment.

     (2) Mediation: beautification, diminished reality, dark patterns, remove real objects from the environment.

   - Strong AR & Weak AR: 

     (1) Strong AR: highly accurate tracking, full semantic understanding, natural / instinctual interaction, head-mounted AR display.

     (2) Weak AR: no or imprecise tracking, no knowledge of the environment, no or mostly implicit interaction, hand-held AR display.

     <img src=".\微信截图_20210102203717.png" />

   - Marker-based AR & Marker-less AR:

     (1) Marker-based AR: the device will use a marker to determine the position and scale of the objects. Usually used with tabletop scale.

     (2) Marker-less AR: the device doesn't use a marker and use other technologies such as edge detection. Usually used with tabletop, room and world scale.

   - SLAM & VIO:

     (1) SLAM (Simultaneous Localization and Mapping):

     - The device figuring our both building a map of the 3D space and then finding its location within the 3D space. 

     - Tracking points over sequence of camera frame.
     - Use the tracks to estimate the points' 3D positions.
     - From estimated 3D positions, calculate camera pose which could have observed them.
     - Observe sufficient points and solve for motion and structure.

     (2) VIO (Visual Inertial Odometry): 

     - using both the camera and the inertial measurement unit of the smartphone and trying to figure our how the phone actually moves through 3D space.
     - Track pose via camera (visual system) by matching a point in real world to pixel on camera sensor each frame.
     - Also track pose via IMU by processing both accelerometer and gyroscope data.
     - Analyze measurements of both systems over time to determine the best estimate of 3D position.

   - Registration: the process of positioning virtual object with respect to real world.

   - FOV (Field of View): HoloLens has around 35 degrees of field of view. Limitation of AR devices.

   - Plane Detection & Object Recognition: 

     (1) Plane Detection: Make the device visualize the plane. On example is to measure the size of screen with AR.

     (2) Object Recognition: Detect and understand what the object is.

   d. AR Technologies:

   - Marker Tracking: used for marker-based AR.
   - Motion Tracking: understand where the device itself is in 3D space without marker.
   - Body Tracking: track and record the movement of the body.
   - Spatial Mapping: capture and record a 3D space and place virtual objects in the space.
   - Scene Understanding: the device understanding what a real object is, getting better now.
   - Projection Mapping: project virtual objects into the environment so that the user doesn't need to wear any devices.
   - Light Estimation: estimate the light of the environment.

3. XR decisions:

   a. Factors to consider:

   - VR or AR: 

     (1) VR is better when: lots of visual elements, interaction at infinite resolution.

     (2) AR is better when: some visual elements, interaction at 1 : 1 scale or less, need connection with real world.

     (3) XR is not ideal when: many non-visual elements, lots of text to read or input, heed haptic feedback.

   - Type of display and tracking:

     Displays: VR: head-mounted vs. room-sized, tethered vs. untethered.

     ​				AR: hand-held vs. head-worn, spatial vs. monitor-based.

     Tracking: VR: 3 DOF vs. 6 DOF, outside-in vs. inside-out, head vs. eye gaze, controller vs. hands.

     ​				AR: marker-based vs. marker-less, plane detection, 3D spatial mesh, physical objects.

   - Type of platforms and devices:

     Phone-based, 3 DOF HMD, 6 DOF HMD for VR.

     Marker-based Phone, Marker-less Phone, 6 DOF HMD for AR.

   - Tools for design and development:

     360, 3D, Immersive Authoring, VR Apps for VR.

     Marker-based AR, Body-based AR, Immersive Authoring, AR Apps for AR.

   b. XR Technology tree:

   <img src=".\G-ZPELxpS3imTxC8aRt4Qg_4427051af81145c89f26f14e3bbe08f0_techtree-med.png" />



#### Week 3: Trends & Issues in XR

1. Trends in XR

   a. A technical HCI perspective: including people and their tasks as well as the technologies.

   <img src=".\微信截图_20210103102036.png" />

   b. Trends in different perspectives:

   - People: 

     (1) Single-user => Multi-user => Social

     (2) Able-bodied user => Any user

   - Tasks: 

     (1) Seated / Tabletop => Standing / Room => On the Go / World

     (2) Specific Context => Any Context

   - Technology: 

     (1) Tethered => Standalone => Built-in

     - Tethered VR/AR headsets: Rift/VIVE, Magic Leap

     - Transforming smartphones: Cardboard/GearVR/Daydream, ARCore/ARKit

     - Standalone VR/AR headsets: Go/Quest, HoloLens/Nreal

     - Integrated VR/AR capabilities: Spectacles/Focals

     (2) Hardware => Software => Cloud-based

     - Dedicated XR hardware: Glass/Tango, Kinect/MoCap suits

     - Software-based XR: ARKit/ARCore, OpenPose/PoseNet/BodyPix, Lens Studio & SnapML

     - Cloud-based XR: Kinect Azure, HoloLens Remote Rendering, 6D.ai & Niantic

     (3) AR or VR App => AR or VR Mode => Cross-reality

     - Dedicated AR or VR apps: Altspace, IKEA Place, Google Earth & Google Lens

     - Apps that offer AR or VR modes: Snapchat, Amazon Shopping, Google Maps & Google Search

     - Apps that support both AR & VR: Spatial, Ongoing research

2. Key Issues in XR

   a. Classes of Issues: 

   - Design Issues: high barrier to entry, few guidelines & best practices.
   - Technical Issues: Platform fragmentation, device limitation.
   - User Adoption: Still fairly unknown / unfamiliar, accessibility & equity.
   - Social Acceptance: Ethical & social concerns, privacy & security.

   b. Technology issues:

   <img src=".\微信截图_20210103112440.png" />

   

   c. Other issues:

   - Ethical & Social Concerns

     (1) How to promote ethical and responsible XR design?

     (2) How to increase control of users over XR apps?

     (3) What are new norms in social XR apps?

     (4) How to mitigate concerns about XR use in public?

   - Accessibility & Equity

     (1) How to make XR accessible for impaired users?

     (2) How to use XR to increase users' abilities?

     How to broaden access to XR technologies?

   - Privacy & Security

     (1) How to communicate what data is being collected?

     (2) How to prevent XR apps from seeing sensitive data?

     (3) How to know an XR app is safe and secure?

   d. Addresses: 

   - Apple lessons learned from mobile & web
   - Extend existing ecosystems
   - Make it part of existing workflows
   - Add real value for users
   - Lower the barriers to entry



#### Week 4: XR Strategy

1. Knowledge: 
   - What knowledge in the team?
   - What do you want to learn?
   - Applications, Technology, Issues, Design, Development, Management
   - Evangelist, Reading Group, Community of Practice

2. Team:
   - What role do you have?
   - What is a good composition?
   - Designer, Developer, Manager, Artist, Researcher, Entrepreneur

3. Equipment: 
   - What XR platforms & devices?
   - What XR tools and workflow?
   - Start with phone => Go broad => Combination
   - Have a dedicated space, try out the latest and never buy in bulk

4. Users:
   - Who are your target users?
   - What tasks you want to enable?
   - Seminars, Demos, Workshops



