
# Full Body Photogrammetry / 3D Scan Image Dataset for 3D Photo Real Avatar / Model Creation

A set of 88 images - 8MP(3280 x 2464), 478MB in total - inside images folder.

you can also directly download .zip file from here.
https://www.real-avatar.com/Full_Body_Photogrammetry_Dataset_Yukihiro_Iwayama.zip

Camera : Raspberry Pi Camera Module v2

One of Reconstruction results is here.
https://skfb.ly/6NUVq
Directly uploaded from RealityCapture. No modification in other 3D software.

**Needless to say, you can use these images in 3DF Zephyr, Metashape, Meshroom and other photogrammetry software.**

Free to download and use. Give credit to Yukihiro Iwayama .

model : Yukihiro Iwayama,  Twitter: @[HappyOcean](https://Twitter.com/HappyOcean)

## Image Data Acquisition System Overview
"Full Body 3D Scan System Kit with Raspberry Pi Zero W"
https://www.slideshare.net/EIDEN_PRO/full-body-3d-scan-system-kit-with-raspberry-pi-zero-w

## 3D Scan Studio Location 
Asakusa, Tokyo Japan
https://www.real-avatar.com in Japanese

## Paper
"Real Avatar Production - Raspberry Pi Zero W Based Low-Cost Full Body 3D Scan System Kit for VRM format"
https://www.3dbody.tech/cap/papers/2019/19101iwayama.pdf

## RealityCapture Worlflow  (overview of one example software)

Import

Alignment: Align -> Detect Markers -> Align 

---(You could skip Detect Markers)---

Marker setting : Circular, single ring, 20-bit https://www.real-avatar.com/img/Marker_Setting.png

--(You could skip Detect Markers) --

Set reconstruction region around the subject.

Reconstruction : Normal

Close Holes -> Clean Model

Simplyfy -> Smooth

-- you could skip below ---

Unwrap
  Unwrap parameters
    Maximal texture resolution: 4096 x 4096,
    Texel size: Custom,
    Custom texel size: 0.005280
    
-- you could skip above ---    

Texture


## Remark
I hope this could contribute as some sort of reference data set especially for those who are not quite familiar but are interested in 3D body scan. There is too little of this kind of full image date set of A Pose Human which is openly available. Personally, I haven’t seen it that’s why I release.
