# GASP_DynamicAdditiveOverlay v1.28

# Setup
Due to Bandwidth Cost over the past month ($65), and the fact we capped that out on the last day....I have entirely removed everything from the project that isn't part of the changes I made. The Project is now roughly ~50mb download, this should dramatically decrease the cost to almost nothing. However there will now be additional setup. I will make a video in the morning and post it here alongside the new steps to cloning this.

# WATCH THIS VIDEO OR YOU ARE WASTING YOUR TIME.
For the video walkthrough: https://youtu.be/lBOvJg22PuY

Initial Setup
1. Clone the Repo
2. Create a GASP Project
3. Copy the Gasp Files over to the Repo Folder

Project Setup
1. Set my Character BP as the Default Pawn Class
2. Create Virtual Bones on the Character

This repository is now free, as long as I keep the project size under 100mbs I shouldn't need LFS Storage.
I'm not sure if you will need LFS but here is the link in case you do. https://git-lfs.com

# ABOUT THIS PROJECT

The Dynamic Additive Overlay technique is most famously known in ALS. After studying ALS on and off over time I began to understand how it worked. When the Game Animation Sample Project dropped I decided to do a simple tutorial on using that technique to overlay poses naturally onto the Motion Matching. It soon started gathering publicity and rapidly evolving as I realized that my simplistic approach was a bit to simplistic and suffered from some serious limitations. 

Although a good learning intro to the technique I wanted to improve it but I wanted to do it all from scratch rather then copy/pasting code someone else wrote, so I began this project. This project was originally only really meant to demonstrate an approach to extending the Motion Matching Sample Project, it is mostly meant for Educational Purposes only, however I am aware many people will be building off of it and I am fine with that.

I didn't copy/paste ALS code although I do use a few of Calvin's Poses simply because they saved me time and worked fine for the situation given they were designed with this in mind and not much modifications would need to be made after retargeting them.
Some of the other poses I did myself, such as for the Aimoffset, an AimSweep to me personally seemed to overcomplicate the situation. I was able to use basically the same technique but using only 2 poses modified from the rifle holding pose which I had to correct for anatomy offsets.

In this project I take full advantage of the Live Retargeting and I promote the use of it for dealing with Anatomy Issues. My approach involves State Based Hand Offsets applied to the Live Retarget which gets automatically interpolated in the animation instance during live retargeting.
![image](https://github.com/user-attachments/assets/ec0c6703-5f2c-429f-8082-93d0a6348f9b)

As you can see in the image I have a line trace running, this is for correcting the Aim of each player so that they are actually pointing the gun towards the center of the screen. This means that you will never have to shoot the gun and watch the bullet come out at a 5-25 degree angle from where the gun is actually pointing.

I will develop this Readme further as we go.

**Due to Bandwidth expenses I am going to be reducing the file size of this Repository as much as possible, everything was removed but the changes I made in order to keep this project Free so that it wouldn't cost me anything to share it openly on GitHub**

The Following Folders have been removed and can be added back from the original Game Animation Sample Project (GASP)

**NOTE: THESE FILES ARE STILL REFERENCED SO THAT YOU CAN EASILY ADD THEM BACK, THEY HAVE ONLY BEEN REMOVED AND IGNORED FROM THE REPOSITORY**

Folders Removed:

Everything but Content/DAO Folder
