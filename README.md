
# Full Body Photogrammetry / 3D Scan Image Dataset for 3D Real Avatar / Model Creation

A set of 88 images - 8MP(3280 x 2464), 478MB in total - inside images folder.
<img src="https://www.real-avatar.com/img/dataset_sample.png" alt="Dataset Sample" title="Dataset Sample">

you can also directly download .zip file from here.

https://www.real-avatar.com/Full_Body_Photogrammetry_Dataset_Yukihiro_Iwayama.zip

Camera : Raspberry Pi Camera Module v2

One of the reconstructed and textrured resulting 3D model is here.
https://skfb.ly/6NUVq
Directly uploaded from RealityCapture. No modification in other 3D software.
<img src="https://www.real-avatar.com/img/YukihiroIwayama_Sample_Model.png" alt="Sample Model Yukihiro Iwayama" title="Sample Model Yukihiro Iwayama">

**Needless to say, you can use these images in 3DF Zephyr, Metashape, Meshroom and other photogrammetry software.**

Free to download, use, reconstruct and/or make it public. Give credit to Yukihiro Iwayama .

model : Yukihiro Iwayama,  Twitter: @[HappyOcean](https://Twitter.com/HappyOcean)

## Image Data Acquisition System Overview
"Full Body 3D Scan System Kit with Raspberry Pi Zero W"

https://www.slideshare.net/EIDEN_PRO/full-body-3d-scan-system-kit-with-raspberry-pi-zero-w


## 3D Scan Studio Where Dataset captured
The studio's 3D Model is https://skfb.ly/6OnYD
<img src="https://www.real-avatar.com/img/Asakusa_Studio.png" alt="Asakusa Studio" title="Asakusa Studio">

Asakusa, Tokyo Japan
https://www.real-avatar.com in Japanese

## Paper
"Real Avatar Production - Raspberry Pi Zero W Based Low-Cost Full Body 3D Scan System Kit for VRM format"

https://www.3dbody.tech/cap/papers/2019/19101iwayama.pdf

3DBODY.TECH 2019 - The 10th International Conference and Exhibition on 3D Body Scanning and Processing Technologies, 22-23 October 2019, in Lugano, Switzerland.

## RealityCapture Worlflow  (overview of one example software)
<img src="https://www.real-avatar.com/img/RealityCapture.png" alt="RealityCapture" title="RealityCapture">
* Import

-------
* Alignment:
  Align >
  Detect Markers >
  Align 2 times (align and wait and then align again. this reduces errors)

  Alignment Setting : https://www.real-avatar.com/img/Alignment_Setting.png
  
  You could skip Detect Markers but it clearly achieves better alignment as experimental option

  Marker Type : Circular, single ring, 20-bit https://www.real-avatar.com/img/Marker_Setting.png
  
    After last 2 times alignment, it should look like https://www.real-avatar.com/img/reprojection_error.png
--------

* Set reconstruction region around the subject.

* Reconstruction : Normal

---------
* Close Holes -> Clean Model

* Simplify to 350,000 -> Smooth https://www.real-avatar.com/img/simplify_smooth.png

  (you could skip unwrap but it produces better texture with custom settings)

* Unwrap
  Unwrap parameters:
  
  Maximal texture resolution: 4096 x 4096, Texel size: Custom, Custom texel size: around 0.005280 depends on how you set reconstruction region
  
  https://www.real-avatar.com/img/unwrap_parameters_for_texture.png
  
  You should aim for near 100% texture quality while maintaining count of textures 1

-- --- ---    

* Texture

## Retoplogy by Wrap3
https://skfb.ly/6NWU8
<img src="https://www.real-avatar.com/img/Retopology_Wrap3_Yukihiro_Iwayama.png" alt="Retopology by Wrap3 Yukihiro Iwayama" title="Retopology by Wrap3 Yukihiro Iwayama">


## Remark
I hope this could contribute as some sort of reference data set especially for those who are not quite familiar but are interested in 3D body scan. There is too little of this kind of full image date set of A Pose Human which is openly available. Personally, I haven’t seen it that’s why I release.
