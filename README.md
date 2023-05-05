Download Link: https://assignmentchef.com/product/solved-ece-210b-homework-7
<br>



In this assignment, you will reinforce what we did in lecture today regarding MATLAB’s filter toolbox.

For each of the following questions, you will create a filter, create magnitude-phase plots for the filter and apply the filter to a signal. Follow these steps:

<ul>

 <li>Generate MATLAB code for filters using the filter design toolbox in the signal processing toolbox (<em>filterDesigner</em>).</li>

 <li>Create a filter object by calling the generated code.</li>

 <li>Use the DSP toolbox’s version of <em>freqz </em>on the filter object. Make sure to include the sampling frequency in the function call as this is hardly mentioned in the documentation. For example, if <em>filter </em>is a filter object, <em>n </em>is the number of points (you can use 1024) and <em>fs </em>is the sampling frequency, run [<em>H,f</em>] = <em>freqz</em>(<em>filter,n,fs</em>). Note I use <em>f </em>instead of <em>w </em>since by including the sampling frequency, MATLAB scales the frequencies from [0<em>,π</em>] to [0<em>,fs/</em>2]. Hence these frequencies have units of Hertz. Keep that in mind when including units in your plots and setting the axis limits.</li>

 <li>Create magnitude-phase plots akin to homework 6 except for the difference mentioned above regarding <em>f</em>.</li>

 <li>Apply the filter to the signal using <em>filter</em>.</li>

 <li>Lastly, plot the Fourier Transform of the final result using <em>fft </em>and <em>plot</em>. Refer to the notes for the proper way to use <em>fft </em>and obtain the proper scaling.</li>

</ul>

This may seem daunting, but with properly defined functions, you may only have to do most of the work once. However, I still want unique titles for plots (maybe pass in a string?).

<ol>

 <li>Generate a signal that consists of a sum of sine waves of frequencies 1 to 50 kHz. Set <em>t </em>to be from 0 to 2 seconds, using an interval of 0.001s.</li>

 <li>Create a Butterworth lowpass filter with a sampling frequency of Fs = 100 kHz, a passband frequency of Fpass = 10 kHz, a stopband frequency of Fstop = 20 kHz, a passband attenuation of Apass = 5dB, and a stopband attenuation of Astop = 50dB.</li>

</ol>

1

ECE-210B Homework 7

<ol start="3">

 <li>Create a Chebychev I highpass filter with a sampling frequency of Fs = 100 kHz, a passband frequency of Fpass = 35 kHz, a stopband frequency of Fstop = 15 kHz, a passband attenuation of Apass = 2dB, and a stopband attenuation of Astop = 40dB.</li>

 <li>Create a Chebychev II bandstop filter with a sampling frequency of Fs = 100 kHz, a passband frequency of below the frequency Fpass1 = 5 kHz and above Fpass2 = 45 kHz, a stopband frequency of between Fstop1 = 15 kHz Fstop2 = 35kHz, a passband attenuation of Apass = 5dB, and a stopband attenuation of Astop = 50dB.</li>

 <li>Create a Elliptic bandpass filter with a sampling frequency of Fs = 100 kHz, astopband frequency of below the frequency Fstop1 = 15 kHz and above Fstop2 = 35 kHz, a passband frequency of between Fpass1 = 20 kHz Fpass2 = 30 kHz, a passband attenuation of Apass = 5dB, and a stopband attenuation of Astop = 50dB.</li>

</ol>


