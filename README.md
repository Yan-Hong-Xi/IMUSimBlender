# IMUSimBlender
A Blender add-on for simulating and visualizing IMU data.

## Step 1: Setting Up Blender Environment

1. **Extract Blender Archive:**
   - Navigate to the `Blender_v3.0stable_WithCUDA_addSC2Fisheye_202201251123` directory.
   - Extract the `Release.7z` archive to a suitable directory.

2. **Verify Blender Setup:**
   - Ensure that the extracted Blender can run properly.
   - Confirm that it supports custom CUDA and fisheye properties.

## Step 2: Running the Simulation

1. **Open Blender:**
   - Launch the Blender application from the extracted directory.

2. **Load the Blender Model:**
   - Open the Blender model located in `Blender_Scene/RenderCamImgAccordingToCameraTrajectoryAtTxtFile_fisheye.blend`.

3. **Check Configuration:**
   - Ensure that `config.ini` and other necessary configuration files are correctly set up.

4. **Adjust Scene and Parameters:**
   - Make any necessary adjustments to the scene and simulation parameters as required.

## Additional Tools

- **Merge Video Tool:**
  - Located in the `merge_video_tool` directory, containing `ffmpeg.exe` and `merge_video.py`.
- **SISEffectDemo:**
  - Includes raw and processed video files for the SIS effect demonstration.

## Verification

- **VerifyGroundTrustIMUData:**
  - Contains data files (`Acc.csv`, `Gyro.csv`, `Mag.csv`, `Quat.csv`) and Python scripts for verification.

For further assistance, feel free to reach out.
