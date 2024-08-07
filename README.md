# Fireworks-Show-VR

Repo Status : Under Construction.

Being a big fireworks fan, this was a fun little app I put together to celebrate 4th of July.  It was made on an earlier version of Virtuoso Engine, and was first released in [2016](https://www.youtube.com/watch?v=Vr6wFp4_UQU) and updated significantly in 2017.

![fwgif](https://github.com/user-attachments/assets/8d931ee5-a879-4dd9-9510-eb06d53e7db1)

GearVR and App for dead platform(s) so the initial code release here probably won't focus on being super polished or buildable.  But I plan to make revisions so it runs on Quest and PC VR with the modern Virtuoso engine.

Its primary platform was the GearVR, a mobile headset by Oculus and Samsung that you would plug your Samsung Galaxy Phone into.  It supported 3DOF on the headset and later had a motion controlled remote accessory, also with 3DOF that I used as the sparkler.  For performance and compatibility testing I ended up owning 3-4 GearVR headsets and Samsung Phones by the end of developing this thing.  I remember having to track down a used S6 on craigslist for debugging because my GLSL macros were failing to compile, but only on the S6.  Experiences like that make it understandable why they invented SPIR-V :). 

![10608329_10152685492468300_6560327130948865323_o](https://github.com/user-attachments/assets/5c7d41c5-9034-4bd0-95e6-15c93b3e3a7d)

The app was released for GearVR via an app code (rather than being on the storefront itself) that I distributed via the app's website, advertised on Reddit.  It was also added to the Google Play Store with a port to GoogleVR / Cardboard.

There were some cool or notable things about the app including:
- 60FPS Stereo on mobile
- really good water shader with raycasted reflections of the fireworks and HDR sky
- The actual Fireworks show was an HD video rendered from Fireworks Sim Pro, a program I used to design the show and synchronize it to the music.
- The sparkler effect is a 3D video capture of a real sparkler, made with a custom capture rig.  A friend made a wood frame for a couple of 4K Yi cameras.  We ran a background subtraction script and some other processing on the raw video to make the final asset.
- I used the OVR_Multiview OpenGL extensions which were very new at the time.
  
  ![61shB0mir5L _AC_SX679_](https://github.com/user-attachments/assets/5a9499e3-dc87-4653-a57f-a5b70981fd3a)

There were some other things I experimented with too, like doing a photogrammetry capture of a section of beach for the user to stand on (instead of the raft / canoe that made it into the final).  I have that data still but wasn't able to finish it to a usable state at the time.
