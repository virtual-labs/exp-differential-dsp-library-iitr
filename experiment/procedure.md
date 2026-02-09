### **General Instructions:**

####  a. To simulate RLS and LMS algorithms on Simulated and real bio-signal data.
1. SPlace a list of different audio files approximately 10 in number in a folder namely “Input Audio” 
2. Select a particular audio file from the folder and carry out the process of analog to digital conversion through sampling and quantization.  
3. After obtaining the digitized version of the audio file the next process involves framing that denotes bundling together of different samples of the audio file in multiple frames. The number of frames selected that also denotes the frame size must be power of 2 in an audio file. Typical values are generally in the range of 256 to 8192. 
4. Select the sampling rate, frame length and hop length from a particular audio file and obtain multiple sets of reading by changing the above parameters associated with the audio file.
  
5. Compute the maximum amplitude values of all samples in a given frame and repeat the same process for all the different frames in an audio file.  
6. After the computation process carried out in Step 4, aggregate the results to obtain the single feature vector of the whole audio. The aggregation features can be Mean, Median, Max and Min. This single feature vector obtained basically denotes the amplitude envelope of whole duration of the audio.
7. Lastly the obtained feature vector denoting the amplitude envelope needs to be plotted for all the different aggregation features discussed in Step 6.
8. The above steps from Step 1 to Step 7 needs to be repeated for all the 10 audio files.