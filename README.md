# IMUSimBlender
A Blender add-on for simulating and visualizing IMU data.

## Step 1: Setting Up Blender Environment

1. **Extract Blender Archive:**
   - Navigate to the `Blender_v3.0stable_WithCUDA_addSC2Fisheye_202201251123` directory.
   - Extract the `Release.7z` archive directly into the `Blender_v3.0stable_WithCUDA_addSC2Fisheye_202201251123` directory.

2. **Verify Blender Setup:**
   - Ensure that `Blender_v3.0stable_WithCUDA_addSC2Fisheye_202201251123/Release/blender.exe` can run properly.
   - Ensure that the `gnss-ins-sim` and `pandas` packages are installed.
   - ![Check Third-Party Packages](document/1.2heck_thirdpart_canrun.png)  

## Step 2: Running the Simulation

1. **Open Blender:**
   - Go to `Blender_v3.0stable_WithCUDA_addSC2Fisheye_202201251123\Release\blender.exe` and run it.

2. **Load the Blender Model:**
   - Open the Blender model located in `Blender_Scene/RenderCamImgAccordingToCameraTrajectoryAtTxtFile_fisheye.blend`.

3. **Open Toggle System Console:**
   - In Blender, open the system console by navigating to `Window > Toggle System Console`.
   - ![Open Toggle](document/2.3opentogglesystemconsole.png)  

4. **Register Instance Panel:**
   - To register the panel by navigating to `Scripting > SimIMU_Panel.py`, first run the `SimIMU_Panel.py` script.
   - After running the script, you will find the Script Runner Panel in the right sidebar of the 3D viewport.
   - ![Register Panel](document/2.3register_panel.png)  

5. **Generate IMU Data:**
   - Pressing the `home` button will navigate the document to `config.ini`.
   - Pressing `Gen Sim IMU` will generate simulation data in the `Output_S` directory.
   - ![Run GenSimIMU](document/2.4GenSimIMUStep.png)
   - Descriptions of other buttons and the fail-safe mechanism.   
   - ![Else Button](document/2.4GenSimIMU.png)

6. **Create Motion Paths:**
   - Set up the pose animation and plot the path using the generated `/Blender_Scene/Output_S/Resample_blender.csv`.
   - ![Run CreateMotionPaths](document/2.5Setanimation_with_pose.png)

7. **Interval Render Animation:**
   - Execute `Interval Render Animation` to render images from both camera into `/Blender Scene/RenderedImages`.
   - ![Run CreateMotionPaths](document/2.5Setanimation_with_pose.png)

## Additional Tools

- **Merge Video Tool:**
  - Located in the `merge_video_tool` directory, containing `ffmpeg.exe` and `merge_video.py`.
- **SISEffectDemo:**
  - Includes raw and processed video files for the SIS effect demonstration.

## Verification

- **VerifyGroundTrustIMUData:**
  - Contains data files (`Acc.csv`, `Gyro.csv`, `Mag.csv`, `Quat.csv`) and Python scripts for verification.

For further assistance, feel free to reach out.
