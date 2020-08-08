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

<p> Depending on the scanning parameters as mention above, the resulting image might not contain any useful information. Not only that, the size of the scan is very small, ![img](http://latex.codecogs.com/svg.latex?10%5E%7B-5%7D) times smaller the material size. These reasons lead to a huge amount of data that needs to be processed so it is definitely to do it manually. Therefore, I develop this automate Python program that assists me in processing 50 data points at a time. The result image can either be a topography image or a FFT image. </p>

## IV. Analysis and Result: 
### 1) Angle between atomic lattice and CDW at temperature from 354K - 360K 
- My intial hypothesis: 
  - The angle between CDW and atomic lattice that near the transition phase (from IC to NC or vice versa) might slowly rotate from 0 deg (IC phase) to 11 – 13 deg (NC Phase)
- Method: 
  - Out of around 7000 data set, I obtain 28 data that match with what we need: having both atomic lattice peaks and CDW peaks
  - Choosing the 2 line pairs that are closest to each other to find the difference. Because of the intrinsic nature of the hexagonal structure, I just need to measure one angle value, instead of 3, for each FFT data image
  - Graphing out the angle values, the angle difference behaves in a no clear trends manner
  
![image](https://user-images.githubusercontent.com/60806068/89712611-090a9e00-d960-11ea-8983-a5552781281f.png)

- Result: 
  - This concludes that the angle between CDW and atomic lattice is unbiased with temperature. Pretty close to the value proposed in table 1 for NC phase, the value for the angle between CDW and lattice is 11.60° ±1.31

### 2) Angle between domain + CDW and domain +  lattice from 354K to 360K
- My initial hypothesis: As the temperature changes, we suspect that the domain might also slowly change its rotation. Because domains form as the material transits from I phase to NC phase, there might be a relationship between them. There might be some sort of relationship in the difference between CDWs and domain. 
- Method: 
  - Obtaining the data is pretty similar to the method in finding the angle between atomic lattice and CDW.  

![image](https://user-images.githubusercontent.com/60806068/89712834-6c490000-d961-11ea-87c7-896977999f93.png) 

- Result: 
  - The angle difference is unbiased with the temperature. This result might happen because of the following reasons: its size - very small and somewhat difficult to detecthere and temperature preference - the domain’s formation is preferred at some temperatures

### 3) Domains formation and satellite peaks
- The method: 
  - I will use 1 data point that have 2nd and 3rd order satellite peaks at room temperature. The image of that data: 

![image](https://user-images.githubusercontent.com/60806068/89713665-40c91400-d967-11ea-94ec-4084af2a46ec.png)  

  - Filtering the lattice + CDW, lattice + satellite peaks, and lattice and low-wavevector (domain) peaks

![image](https://user-images.githubusercontent.com/60806068/89714001-8be42680-d969-11ea-84b8-c8931699a6fa.png)

![image](https://user-images.githubusercontent.com/60806068/89713989-81299180-d969-11ea-979d-f91c05a3da75.png)
  
- Result: 
  - In inside (or center) the domain, the CDW stays fully commensurate with the lattice underneath. When transitioning from I phase to C phase, the CDW might interact with the underneath lattice in a way that all the CDWs share similar period but different wave phases
  - The CDWs wave interference causes the formation of satellite peaks
## V. Conclusion: 
- As the CDW undergoes transition from IC phase to NC phase, the angle between CDW and the atomic lattice is not temperature dependent
- The CDW’s wavelength in both phases is roughly about 11.8A ̇±0.4 A
- The angle between the domain and the underneath lattice is temperature dependent and has a value roughly 5.96 ±0.436°. 
- “False” domains might be formed from the low-wavevector peaks. The true domain can only form when there are satellite peaks. The low – wavevector peaks signifies that the domain in topography might not be actual domain
## VI. Poster

![image](https://user-images.githubusercontent.com/60806068/89713613-cd270700-d966-11ea-91c6-92bd62a729c6.png)
