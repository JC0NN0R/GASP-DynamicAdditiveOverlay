# GASP_DynamicAdditiveOverlay v1.22

This Repository is not free, it is costing me money to host this and I keep running out low on bandwidth. I have had to buy 3 50gb Data Packs in less then a week 2 of those were consumed before I removed some textures which reduced the Repo by close to 60%
With that said I would appreciate any Sponsors or Donations towards Bandwidth that anyone is willing to give. $5 will sponsor 50gb's of Data for a month.

# DO NOT DOWNLOAD ZIP, THIS REPO USES LFS (LARGE FILE STORAGE) READ THIS README
**This Repository uses LFS (Large File Storage), this means if you download the Zip it will have some empty folders.
To get around this, please do not download the Zip, instead download the Desktop App and Clone this Repository.
I'm not sure if you will need LFS but here is the link in case you do. https://git-lfs.com**

The Dynamic Additive Overlay technique is most famously known in ALS. After studying ALS on and off over time I began to understand how it worked. When the Game Animation Sample Project dropped I decided to do a simple tutorial on using that technique to overlay poses naturally onto the Motion Matching. It soon started gathering publicity and rapidly evolving as I realized that my simplistic approach was a bit to simplistic and suffered from some serious limitations. 

Although a good learning intro to the technique I wanted to improve it but I wanted to do it all from scratch rather then copy/pasting code someone else wrote, so I began this project. This project was originally only really meant to demonstrate an approach to extending the Motion Matching Sample Project, it is mostly meant for Educational Purposes only, however I am aware many people will be building off of it and I am fine with that.

I didn't copy/paste ALS code although I do use a few of Calvin's Poses simply because they saved me time and worked fine for the situation given they were designed with this in mind and not much modifications would need to be made after retargeting them.
Some of the other poses I did myself, such as for the Aimoffset, an AimSweep to me personally seemed to overcomplicate the situation. I was able to use basically the same technique but using only 2 poses modified from the rifle holding pose which I had to correct for anatomy offsets.

In this project I take full advantage of the Live Retargeting and I promote the use of it for dealing with Anatomy Issues. My approach involves State Based Hand Offsets applied to the Live Retarget which gets automatically interpolated in the animation instance during live retargeting.
![image](https://github.com/user-attachments/assets/ec0c6703-5f2c-429f-8082-93d0a6348f9b)

As you can see in the image I have a line trace running, this is for correcting the Aim of each player so that they are actually pointing the gun towards the center of the screen. This means that you will never have to shoot the gun and watch the bullet come out at a 5-25 degree angle from where the gun is actually pointing.

I will develop this Readme further as we go.

**Due to Bandwidth expenses I am going to be reducing the file size of this Repository as much as possible, the Echo Character's textures consume 1.3 gbs of bandwidth and so were removed**

The Following Folders have been removed and can be added back from the original Game Animation Sample Project (GASP)

**NOTE: THESE FILES ARE STILL REFERENCED SO THAT YOU CAN EASILY ADD THEM BACK, THEY HAVE ONLY BEEN REMOVED AND IGNORED FROM THE REPOSITORY**

Folders Removed:

Content/Characters/Echo/Textures

Content/Characters/Paragon/Heroes/TwinBlast/Textures

Content/Characters/Paragon/Global

Removing these Folders has freed up well over 2gbs of Bandwidth per Clone

Developed with Unreal Engine 5
