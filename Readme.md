## LipSync :
# **Quick guide**
1. Create video file named input_video.mp4 - audio track removed
2. Create audio file named input_audio.wav 
3. Both files have to be exact same length
4. Target face in the input_video.mp4, must be "detectable" in ALL videoframes (So no black or blurry frames etc)
5. Make sure u use correct file extensions
6. wav2lip does not like very long and high res clips (1080p/30seconds max)

**Important Work Done**
1. Match the length of video and audio file. 
2. Use video editor tools to crop video into part.
    1. Part where the person is visible 
    2. Part where the person is not visible 
3. The apple Wav2Lip model in the visble 

**Refferences**
1. https://github.com/Rudrabha/Wav2Lip
2. https://github.com/anothermartz/Easy-Wav2Lip/tree/v4 
(better improved version )


**RUN**:
1. Select a file in which face is visible. 


**Model 1**
Every thing is explained in the nootbook .

**Model 2**
Every thing is explained in the nootbook .
It uses:  
1. https://colab.research.google.com/github/anothermartz/Easy-Wav2Lip/blob/v4/Easy_Wav2Lip_V4_fixed.ipynb
2. to know about hyperparmaeter go to link https://github.com/anothermartz/Easy-Wav2Lip/blob/v4/README.md
3. Hyper parameter used : 
    Upscaler: gfpgan
    padding : U = -10 , L=0 , R=0 , D=-10
    If using images in batch : Batch_process==True


**Ouput**
1. Append all the video clip together in sequence . (i.e with face and without faces)
2. 


