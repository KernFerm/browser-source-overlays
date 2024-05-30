# Browser Source Overlay for OBS/Streamlabs OBS 🎥

This guide provides step-by-step instructions on how to set up a browser source as a background for your webcam feed in OBS or Streamlabs OBS.

## Prerequisites
- OBS Studio or Streamlabs OBS installed on your computer.
- A webcam connected and configured.
- The `example.html` file (containing the Example code).
> Note: There is no `example.html` provided. This is just to illustrate the setup process.

## Step 1: Download the Example HTML File 📥
1. Save the HTML code for the Example effect with alien text as `example.html`.

## Step 2: Add the Example effect in OBS/Streamlabs OBS 🛠️
1. **Open OBS or Streamlabs OBS**.
2. **Add a Browser Source**:
   - Click the `+` button in the `Sources` box.
   - Select `Browser`.
   - Name it (e.g., `example.html`) and click `OK`.
   - Check `Local File` and browse to the location of your saved `example.html` file.

   > **Tip**: To find the location, **right-click** on the file in your file explorer and select `"Copy path"` or `"Properties"` to get the file's location. and paste that location in your `"Browser URL"`. Make sure you `KEEP` the `Web Browser Open` while it is running in obs other wise it will `NOT` work.
   
   - Set the width and height to match your stream resolution (e.g., 1920x1080).
   - Click `OK`.

## Step 3: Add and Configure Your Webcam Feed 📹
1. **Add a Video Capture Device**:
   - Click the `+` button in the `Sources` box.
   - Select `"Video Capture Device"`.
   - Name it (e.g., `"webcam"`) and click `OK`.
   - Select your camera from the device list.
   - Adjust the settings as needed (resolution, frame rate, etc.).
   - Click `OK`.

2. **Ensure Proper Source Order**:
   - In the `Sources` box, ensure the Video Capture Device (camera feed) is listed above the Browser source (Matrix effect).
   - You can drag and drop the sources to reorder them if necessary.

## Step 4: Adjust the Browser Source to Fit Your Camera Size 🖼️
1. **Add Crop/Pad Filter to Browser Source**:
   - Right-click on the Browser source.
   - Select `Filters`.
   - In the `Effect Filters` section, click the `+` button and select `"Crop/Pad"`.
   - Name it (e.g., "Adjust Browser Size") and click `OK`.

2. **Configure Crop/Pad Filter**:
   - Adjust the `values` for `Left`, `Top`, `Right`, and `Bottom` to **fit the Browser source to your camera size.**
   - `You can fine-tune the cropping to match the dimensions of your webcam feed.`
   - `Close the filters window once done.`

## Step 5: Adjust Camera Feed Opacity (If Needed) 🌟
If the Example effect is not visible behind your webcam feed, you may need to adjust the opacity of your camera feed.

1. **Add Color Correction Filter**:
   - `Right-click` on the Video Capture Device source.
   - Select `"Filters"`.
   - In the `"Effect Filters"` section, click the `+` button and select `"Color Correction"`.
   - Name it (e.g., `"Camera Opacity"`) and click `OK`.

2. **Configure Opacity**:
   - Adjust the `"Opacity"` slider to make the camera feed partially transparent.
   - Start with an opacity of around 70-80% and adjust to your preference.
   - Close the filters window once done.

## Step 6: Final Adjustments 🎉
1. **Re-enable All Sources**:
    Ensure **both** the Browser source (**Example effect**) and the Video Capture Device  
   (**camera feed**) are visible (**eye icons are not crossed out**).

2. **Check Preview**:
   - Verify in the preview window that the Example effect ( **which ever `.html file` you downloaded**) is visible in the background of your camera feed.
   - Adjust the opacity or other filter settings as needed to achieve the desired effect.

## Troubleshooting ⚠️
- **Example effect Not Visible**: Ensure the Browser source is at the bottom of the source list and the Video Capture Device is above it.
- **Webcam Feed Too Opaque**: Adjust the opacity of the webcam feed using the Color Correction filter.
- **Performance Issues**: Ensure your system can handle the additional processing load of the overlay.

By following these steps, you should be able to create a dynamic and unique **Example-themed** background for your webcam feed in OBS or Streamlabs OBS. Enjoy streaming with your new setup! 🙂
