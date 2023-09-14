# LipSync :

**Drive Link:**
https://drive.google.com/drive/folders/1nqK8s94LkA7oe5KgOYIQfCcKTFXaU7ny?usp=sharing
<br>
Video Results:
1. Result   https://drive.google.com/file/d/1dsfUPvzRU676HJ5Ha0QkdjIXRMeytxAb/view?usp=sharing
2. Result   https://drive.google.com/file/d/1fJl3ReoWfy_X9OOsId8p50Yz_7GqnYB7/view?usp=sharing
3. Result   https://drive.google.com/file/d/1SPBmYjDCTgdtJUOnQiFmer2ZUrL6YZIG/view?usp=sharing

<hr>

## **Quick guide**
1. Create video file named input_video.mp4 - audio track removed
2. Create audio file named input_audio.wav 
3. Both files have to be exact same length
4. Target face in the input_video.mp4, must be "detectable" in ALL videoframes (So no black or blurry frames etc)
5. Make sure u use correct file extensions
6. wav2lip does not like very long and high res clips (1080p/30seconds max)

<hr>

### **Important Work Done**
1. Match the length of video and audio file. 
2. Use video editor tools to crop video into part.
    1. Part where the person is visible 
    2. Part where the person is not visible 
3. The apple Wav2Lip model in which the person is visble. 

<hr>

### **References:**
1. https://github.com/Rudrabha/Wav2Lip
2. https://github.com/anothermartz/Easy-Wav2Lip/tree/v4 
(better improved version )

<hr>

## **RUN**:

Select a file in which face is visible. 


1. ### **Model 1**
Every thing is explained in the nootbook .

Colab link: 
https://colab.research.google.com/drive/1ZrtU9cu9Oq2E8lKRE6VPabgPOWLr-iri

Video Result:
https://drive.google.com/file/d/1dsfUPvzRU676HJ5Ha0QkdjIXRMeytxAb/view?usp=sharing

<br>

2. ### **Model 2**
Every thing is explained in the nootbook .
It uses:  
1. https://colab.research.google.com/github/anothermartz/Easy-Wav2Lip/blob/v4/Easy_Wav2Lip_V4_fixed.ipynb
2. to know about hyperparmaeter go to link https://github.com/anothermartz/Easy-Wav2Lip/blob/v4/README.md
3. Hyper parameter used : 
    1. Upscaler: gfpgan
    2. padding : U = -10 , L=0 , R=0 , D=-10
    3. If using images in batch : Batch_process==True



Video Link: 
https://drive.google.com/file/d/1fJl3ReoWfy_X9OOsId8p50Yz_7GqnYB7/view?usp=sharing

<hr>

### **Output**
1. Append all the video clip together in sequence . (i.e with face and without faces)
2. Edit video frames if needed.

<hr>

### **Special Operation**

**to improve the quality used Gan on the output video**

https://github.com/GeeveGeorge/GFPGAN-for-Video-SR
<br>
using the above model convert frames and the reconstruct using GAN.

**Disadvantage:**
1.  looks not real
2.  Lip sometimes out of Sync

**Advantages:**
1. improved quality of lip movement:

Video Result :
https://drive.google.com/file/d/1SPBmYjDCTgdtJUOnQiFmer2ZUrL6YZIG/view?usp=sharing




