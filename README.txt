Mobile Automation Testing
This type of testing is done to check whether mobile applications work well across various operating systems and mobile devices.
This testing performs various aspects of testing such as usability, security, performance, quality, and functionality. It also tests the ability of a new application to interact with other applications.

Appium
Appium is an automation testing tool that can be used to validate mobile browsers and mobile applications.
It is used in mobile automation testing because it is free and is cross-platform (can support both iOS and Android).
Automation tests in Appium can be run on mobile devices, simulators, and emulators.
An emulator is software or hardware that allows a computer system (host) to run applications designed for another system (guest).
The Appium architecture consists of three main components:
Appium Client
This contains the automation code (scripted). This code is written in a specific programming language.
The script contains the configuration details of the application and the mobile device. The scripted code and the configuration details are used to run the applications’ test cases.
Appium Server
This is an HTTP server that receives command requests (HTTP requests) from the client component (in JSON format). The commands are then executed on mobile devices.
End device
This refers to an emulator or a mobile device that is connected to the Appium server. The test cases are executed on this device.
How does Appium work?
It sets up an HTTP server that generates a REST API to enhance communication with the client.
This server collects command requests from the Appium client in JSON format. JSON Wire Protocol is a medium of communication between the server and the client. It plays the role of communicating command requests. These command requests are then executed on the end devices (either on Android, Windows, or iOS).
The Appium server uses a test automation framework to execute requests on the user interface of end devices.

How does Appium work On Android?
The Appium client connects with the HTTP server and uses the JSON Wire Protocol for communication.
The Appium server receives requests from the client component.
The server connects with the mobile automation framework for Android (UI Automator or Selendroid).
Android devices contains bootstrap.jar that receives the test commands from the Appium server. The bootstrap.jar contains executable files that enhance the connection between the server and Android devices. It plays the role of a TCP server since it enhances the secure transmission of test commands to the Android devices.
The bootstrap.jar uses the UI Automator or Selendroid to execute the command requests on the Android device.
The test results are then sent to the server, which eventually sends HTTP responses to the Appium client. The HTTP responses contain status codes indicating success or server error.

Test Steps for Post Image Feature for the given task:
1.Download and configure appiumin and Emulator(from Android studio) in your system.

2.Open the emulator.

3.Download ADB Driver and open command prompt in the adb driver folder and type adb devices on the terminal. You will get a list of devices connected and hence the device name of your emulator.

4.Fill in the desired capabilities as given in the task (fill android device value as the name of your device your recognized in the last step).

5.Now, you can start session, you will see the emulator screen loading the application while on appium window you can see the appium inspector(which is the screenshot of the emulator screen).

6.Now, sign-in with the login credentials provided, you'll observe that the application is opened.

7.Now try posting image and check for below mentioned test cases. 

Manual Test Cases for Post Image upload functionality:

1.Firstly, check Image upload path.

2.Test the Image Upload feature with image files of different extensions like PNG, BMP, JPEG etc.

3.Test with the image whose names contain space or some special characters.

4.Upload a duplicate name image.

5.To test that if user can see  the uplaoded images.

6.Check image upload with image size greater than the maximum allowed size.Proper message should be displayed.

7.Check image upload feature with file types other than images like txt, doc, exe, pdf etc.

8.Test with the images of specific width and height if specified are accepted otherwise rejected.

9.There should be a progress bar for large size images.

10.Test for the cancel button functionality is working in between while uploading the image.

11.Check the file selection dialog shows only supported files listed.

12.Check multiple images upload functionality.

13.Test for the image quality after upload.The quality of the image should not be changed after uploading the image.

 

These are the enough test cases which cover all major functionality of Image Upload feature.

 