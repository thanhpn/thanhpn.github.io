---
layout: post
title:  "Guide submit app to Apple Appstore  "
date:   2016-12-5
desc: "Guide submit app to Apple Appstore"
keywords: "Guide,submit app,Apple,Appstore"
categories: [Life]
tags: [blog]
icon: fa-bookmark-o
---

App submission is often an afterthought. But ensuring you submit your app to the App Store properly (a service included in our end-to-end development) is an important first step to ensure exposure and entice users to download.


That’s why we made this step-by-step guide to App Store submission. This guide contains all the steps required to properly submit an iOS app to the App Store.

**Prerequisites

Project that is ready for submission and passes Apple’s App Store Guidelines 
Valid Apple developer program account (not the Apple Developer Enterprise Program)
Computer that runs Mac OS X
The following programs installed:
Xcode
Keychain Access


Step Overview

Below you will find a list of guides, each describing how to do one of the steps required for submitting an app.

Assemble App Store Information
Create a Bundle Identifier
Create a Certificate Signing Request
Create an App Store Production Certificate
Create a Production Provisioning Profile
Create an App Store Listing
Create a Release Build
Fill in the Version Information
Submit Version for Review
Release


1. Assemble App Information

It is very important to collect all of the information you need to submit before you start the process.  More Information Here

Requirements	Notes
Screenshots	You need at least one for every supported device screen size.  The screenshots cannot contain transparency
Name	Name of the app as seen by users
Description	A description of your app, detailing features and functionality
Keywords	Separate keywords with a comma
Support URL	A URL with support information for your app
Marketing URL	A URL with marketing information about your app, optional
Privacy Policy URL	A URL containing your app’s privacy policy, optional
App Icon	This icon will be used on the App Store and must be in the JPG or PNG format, with a minimum resolution of at least 72 DPI, and in the RGB color space. It must not contain layers or rounded corners.
Categories	Secondary category is optional
Rating	Generate your rating based on the questionnaire  More Information Here
Copyright	Use the format: YYYY Company Name
Trade Representative Contact Information	Only appears on the Korean App Store, optional
Demo Account	“The username and password for a full-access account for your app. Include details for additional accounts in the Notes field.”


2. Create a Bundle Identifier

The bundle identifier is the name of your app, as seen by both the App Store and iOS devices.

In your browser, navigate to Apple’s Developer Portal
Log in
Click Identifiers
Click the “+” in the top right of the screen
Name the App ID the same as your app
Make sure the Bundle ID follows the standard naming convention: com.yourcompanyname.yourappname
Check any App Services the app needs, click Continue
Verify the services are correct, then click Submit


3. Create a Certificate Signing Request

Certificate Signing Requests are used to link your computer to your Apple developer account.

Open a program called KeyChain Access
In the top left menu, click Certificate Assistant
Click Request a Certificate From a Certificate Authority…
User email: Enter your email address
Common Name: We recommend using the name of the app
CA email is not actually required
Check Saved to Disk, click Continue
Save the Certificate Signing Request for later


4. Create an App Store Production Certificate

Code Signing Certificates are used to link iOS apps to your Apple developer account.

In your browser, navigate to Apple’s Developer Portal
Click Certificates
Click the “+” in the top right of the screen
Click the App Store Production
Currently named “App Store and Ad Hoc” under Production
Click Continue
Upload the Certificate Signing Request created earlier
Download the Certificate
Install the certificate on your computer by double clicking
Keep this file somewhere safe


5. Create a Production Provisioning Profile

Provisioning Profiles are packaged with iOS apps so users devices can install them.

In your browser, navigate to Apple’s Developer Portal
Log in
Click Provisioning Profiles
Click the “+” in the top right of the screen
Click the App Store Distribution option, click Continue
Select the Bundle ID created earlier, click Continue
Select the Certificate created earlier, click Continue
Make sure the Profile Name follows the standard naming convention: App Name App Store Distribution
Click Generate
Download it
Install the provision profile on your computer by double clicking
Keep this file somewhere safe


6. Create App Store Listing

Reserve a slot in the App Store for your app for users to see.

Start in your browser, navigate to iTunes Connect
Log in
Click My Apps
Click the “+” in the top left of the screen
Click “New iOS App”
Bundle ID: choose the one created on Developer Portal
For convenience, make the SKU match the Bundle ID created earlier
Click Create to create the first version listing


7. Make the release build

Package the actual binary that users will be uploading to the store.

Start Xcode
Open the project or workspace
Update the version and build numbers
Open Build Settings
Make sure All settings is selected
Scroll to Code Signing
Use the provisioning profile created earlier
Use the code signing identity created earlier
In the top menu, select Generic iOS Device as the build destination if no actual device is connected
Menu, Project, Archive
Click Distribute
Sign in as your apple developer account
Submit to app store
Wait for the confirmation


8. Fill In Version Information

Users will decide whether or not to install your app based on your store listing.

Enter all of the information assembled in step 1
Select the build you wish to tie to the version (Note: This usually appears 10-15 minutes after sending from Xcode)
Fill in pricing information
Click Save
Fit any errors based on the messages that appear and save changes


9. Submit Version for Review

Every app that is submitted to the store has to be reviewed by the Apple team before release.

Select the release type
Manual release – after the app is accepted, a Release button will appear
Automatic release – as soon as the app is accepted, it will be released
Wait for approval
This process usually takes 2-3 weeks for a new submission
If your app was not approved, review the notes in the Resolution Center and make any necessary changes to the app or version information then resubmit


10. Release

Enjoy the final, most satisfying step.

If you selected Manual release, click Release your app when ready
Wait for the green “Ready for Sale” version status (This might take from 1 hour to 1 day after release)
Search for your app on the App Store
Celebrate!
When submitting a new version of your app, you will only have to repeat steps 7 through 10.