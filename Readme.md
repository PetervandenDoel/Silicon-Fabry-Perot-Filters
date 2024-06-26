Fabry perot filters are a kind of photonic narroband filter use for constraining the lasing frequency of semiconductor lasers. The goal of this project is to fabricate and characterize the frequency response of 31 different silicon perot cavities. 


This project was fabriacated in the 2024 SIEPIC open ebl lithography run https://github.com/SiEPIC/openEBL-2024-02, files were named after my edx username. The y branches, grating couplers, waveguide tapers, and bragg gratings were imported as parameterized components from the SIEPIC EBL Klayout library  


**OSA spectra are currently being analyzed. Designs were simulated in Lumerical interconnect to ensure that transmission peaks won't be below the OSA noise floor and transmission peak shifts would be observable within the OSA frequency sweep window**<br>


The goal of this project was to observe the effect of slight bragg grating period changes on the performance of 1310nm TE fabry perot filters used in semiconductor lasers. Different bragg grating periods, reflecitvities, and cavity lengths were tested in every possible combination of these parameters.<br>

Grating period: 271nm, 272nm, 273nm<br>
Number of grating periods: 20, 50<br>
Cavity length: 518nm, 538nm, 558nm, 100μm, 3393μm <br>
Grating corrugation width: 50nm <br>

Designs with different numbers of grating periods(reflectivities) were fabaicated with agressive designs to see strong effects(50 periods), and conservative designs to still see results if cavities are too lossy(20 periods). Different cavity lengths were fabricated to see if the center frequency shift could be observed at vastly different free spectral ranges  


These are the contents of the klayout design files

**TEST SETUP**
Grating couplers are placed precisely 127μm apart from one another to allow for automated testing with fiber arrays. 1310nm light is injected into the middle grating coupler, then transmission is measured on the top and reflection is measured on the bottom.<br> This allows for transmission, reflection, and loss of the cavity to be measured with an optical spectrum analyzer.<br>
Reflections are channeled back into the reflection grating coupler by a Y branch on the input path




![image](https://github.com/PetervandenDoel/Silicon-Fabry-Perot-Filters/assets/73015873/d5230a1b-658f-497c-896f-25e0a9689b43)

**Individual designs**  


Filename: GreyPoupon.oas


There are 6 designs in this file<br>
Design parameters

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/5104ea08-d751-4376-aa18-53d6caca0bf8)
<br>
These designs are meant to profile the behivour of the FP cavities at a medium free spectral range


![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/df7e709b-65c9-4c1e-ab62-4f61fdcfabae)





**Filename: GreyPoupon2.oas**

This design was made simply to capture an SEM image of a funny drawing and because there was extra space on the die left at the last minute


Design parameters 


Cavity length 3851u	 <br>	Bragg grating period 272n <br> 	# periods 20 <br>

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/87eb197e-1ead-4209-8638-a5adbd67f348)




**Filenames: GreyPoupon3,4,5,6,7,8.oas**

Design parameters

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/e62e0e45-5ae7-46e5-afff-8d7f88cad0e3) <br>
These designs are meant to profile the behivour of the FP cavities at a very small free spectral range  

The IC layouts of these 6 designs all look like this

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/3ad2a808-9613-4206-b093-16dedf964846)











**Filenames: GreyPoupon9,10,11.oas**


there are 6 designs each of these this files. All the designs are similar in appearance

Design parameters 

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/b76fe880-b5f6-4246-98d5-ba3727079522)
![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/8ec9f830-9fb4-408c-98cd-9254f17913e1)
![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/eb08cb01-f29b-4c6d-b6b2-55c5ef303093)
<br>
These designs are meant to profile the behivour of the FP cavities at a very large free spectral range(on the order of the OSA frequency sweep window size). Because our cavity lengths are on a similar order to the wavelength, there is a significant risk of the main peak in the transmission spectrum not showing up on the optical spectrum analyzer due to uncertainties in modelling and the lithography process tolerances. Three different fraction wavelength cavity lengths were used to improve the chances of one of the designs providing a good visible frequency response. 






The IC layouts of these 3 files all look like this

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/45c6f4bb-ca50-4d9d-ba69-7122f6f5fc4e)


<br>
Closeup image of one of the 538nm cavities<br>

![image](https://github.com/PetervandenDoel/Fabry-Perot-Cavities/assets/73015873/5ce6ca0a-e799-4f39-8345-e81317139939)


end
<br>





