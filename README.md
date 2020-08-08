# Charge Density Wave of 1T-TaS2 using Scanning Tunneling Microscope
## I. Abstract: 
For this project, I analyzed scanning tunneling microscopy (STM) data to understand the electronic properties in the material TaS2. TaS2 is a material that hosts charge density waves (CDWs). A CDW is a modulation in an electron density within a metal and is accompanied by a periodic lattice distortion and an electronic gap. STM is a reliable tool to observe the atomic structure of a material and how charges arrange themselves. Scientists still do not understand CDW properties on an atomic scale, especially for 1T-TaS2 due to its smaller domain size around ![img](http://latex.codecogs.com/svg.latex?10%5E%7B-7%7D)mm . This means that it would be harder to observe eventhough using a micrscope to scan the service. Studying CDW states above and below their transition temperature will give us an insight into CDW formation and properties.
## II. Introduction 
**Scanning Tunneling Microscopy**

<p>STM is a technique that uses tunneling electrons to produce real-space images and deliver spectroscopic analysis of the surface material at an atomic level. With this technique, scientists can further understand the atomic structure and bonding in solids at unprecedented levels. For this research, STM has helped in 
understanding the CDW of 1T-TaS2 near the commensurate/ incommensurate phase transition </p>

**The material 1T-TaS2**
<p>TaS2, supports a CDW and has several CDW transitions slightly above room temperature, at around 355K. The transitions that I am taking a closer look would be Nearly Commensurate (NC) and Incommensurate (IC). The material’s CDW transition can be observed easily because of the accessible temperature. By studying TaS2 through the CDW transition phase, we can obtain more information about atomic scale changes in structure and properties of CDWs. </p>    

![image](https://user-images.githubusercontent.com/60806068/89607286-1e88a680-d840-11ea-8d67-97c9a4fe2ad9.png)

## III. Experiment Procedure
<p>The environment surrounding 1T-TaS2 is controlled by a thermal bath. The sample was taking at both warming and cooling point. The warming process starts at room temperature goes to 361 K; then the cooling process starts from around 360K to room temperature. At given a temperature value, the sample’s topography is scanned at different scanning rate, different pixels, range of tunneling conditions (200 to 500 pA)and range of bias voltage (-100 to -500 mV) so as to eliminate holes’ formation and noise in the topography. Afterward the information is then process using Fast Fourier Transform method that helps understanding the hexagon formation of CDW. </p>

Fast Fourier Transform Images of the 1T-TaS2 and the material corresponding phase transition 

![image](https://user-images.githubusercontent.com/60806068/89607757-40cef400-d841-11ea-8430-d8e2c00e179f.png)

<p> Depending on the scanning parameters as mention above, the resulting image might not contain any useful information. Not only that, the size of the scan is very small, ![img](http://latex.codecogs.com/svg.latex?10%5E6 times the material size. These reasons lead to a huge amount of data that needs to be processed so it is definitely to do it manually. Therefore, I develop this automate Python program that assists me in processing 50 data points at a time. The result image can either be a topography image or a FFT image. </p>

The code can be found in the files 
## IV. Analysis and Result: 
### 1) Angle between atomic lattice and CDW at temperature from 354K - 360K 
- My intial hypothesis: 
  - The angle between CDW and atomic lattice that near the transition phase (from IC to NC or vice versa) should slowly rotate from 0 deg (IC phase) to 11 – 13 deg (NC Phase)
- The result: 
  - 
### 2) 
## V. Conclusion: 

