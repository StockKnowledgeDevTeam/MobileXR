# MobileXR
Main Repository for the SK-XR mobile application.

Uniuty Version : 2019.4.20f1

This github repository contains the ff:
  - AR
  - VR
  - 3D assets
  - UI assets
  - Google VR SDK
  - Vuforia SDK



How to install Unity.

Go to the Unity Archive Download Page "https://unity3d.com/get-unity/download/archive", look for the 2019.x tab and select the version 2019.4.20 dated 10 February, 2021, and click “Download Unitry Installer”. A UnityDownloadAssistant-x.x.exe file should be downloaded to your “Downloads” folder (where x.x is the current Unity version).
Open the downloaded installer
Accept the license and terms and click Next.
Select the components you would like to be installed with Unity and click “Next”. Note: If you ever want to change the components, you can re-run the installer.
  *Recomended Components:
        - Unity Editor
        - Visual Studio
        - Android Mobile Support
You can change where you want Unity installed, or leave the default option and click “Next”.
Depending on the components you selected, you may see additional prompts before installing. Follow the prompts and click “Install”. Installing Unity may take some time. After the installation is finished, Unity will be installed on your computer.
Enabling VR 2019.31.

Launching the Package Manager Window To develop VR experiences, you’ll need to install the VR SDK for your target OS and VR platform. The VR SDKs are installed via the Package Manager.(You can access the Package Manager Console from Visual Studio by going to Tools --> Library Package Manager --> PackageManager Console)a.Select the Package Manager from the “Window” drop down (Figure 01).Figure 01b.Once you click the “Package Manager” all packages will appear and you need to select “Open VR Desktop”. Click to install. Figure 02 below. Figure 02Other supported platforms includes:Android (Google VR Android, Oculus Android)Desktop (Oculus Desktop, OpenVr (Desktop))iOS (Google VR iOS)
Enabling VR support in project settingsUpon installing the VR SDK we are now ready to enable VR.a.Select “Project Settings” from the “Edit” drop down. See Figure 03Figure 03 b.Once “Project Settings” open click “Player”. See Figure 04Figure 04c.At the bottom part of the “Player Window” click the XR Settings to expand the section. You will see a box, then marked the “Virtual Reality Supported”. See on the Figure 05.Figure 05Note: Enabling Virtual Reality Support is the same across all currently supported platforms. d.Once “Virtual Reality Supported” is enabled you will need to add at least one VR SDK. Click the “+” sign and select “Open VR” if it is notalready added. But if once clicked and the “Open VR” is already there, no need to click the “+” sign. See Figure 06. Figure 06e.Close the “Player Settings” window. 3.ConclusionYour Unity Project is now configured for VR development.


How to install vuforia in your unity file:

The Vuforia Engine will be visible in the GameObject Menu.
If this menu is not shown, this means that you did not install Vuforia with Unity (Unity versions before 2019.2) or did not add the Vuforia Engine package to your project (Unity 2019.2 and later).

Start by adding an ARCamera. This is a Unity camera game object that includes the VuforiaBehaviour to add support for augmented reality apps for both handheld devices and digital eyewear.
Add an ARCamera GameObject from the Vuforia Engine menu. Select the ARCamera and Open Vuforia Configuration from the Inspector Add a Vuforia Development License Key in the App License Key field. For a guide on getting a license key, see Vuforia License Manager

Note: Delete the default Main Camera after adding an ARCamera. The ARCamera contains its own Camera component. The Main Camera is not needed unless you are using it to render a specific camera overlay, e.g. user interface.

Vuforia: How to add image tracking feature.

After activating Vuforia Engine in Unity, you can add features from the Vuforia Engine menu to your project from the Unity GameObject Menu.
Navigate to the Vuforia Engine Menu and select Image Target. or any of the other targets you wish to use. (VuMark, Ground Plane, and Mid Air are also trackable targets). For configurations for using other targets, please consult the Features Overview linked just above. It presents Unity guides for each Vuforia target.
Each Vuforia Engine GameObject can be configured in the Inspector. When a target is added, it will appear in the Hierarchy.

Select the Image Target GameObject from the Hierarchy and choose from the Type dropdown either From database – Image Target databases can be made in the Vuforia Target Manager. Targets to the project. Vuforia will therefore ask you if you wish to Import Default Image Target Database in a pop-up window.

Press Import. Note: Maintain an accurate scale between the Vuforia targets and physical prints or objects. Using targets that deviate in size from the real-life object you wish to track might impact the quality.

# COPYRIGHTED CONTENTS
Images, videos, and text contents that are unique to Stock Knowledge are copyrighted. Please ask permission if you wish to use them.
