# Gilbert Cell Mixer
### MIXED SIGNAL MARATHON
<img width="1313" height="547" alt="image" src="https://github.com/user-attachments/assets/08efb8b1-49c2-4801-a641-c943e0a8d504" />

  * [Abstract](#abstract)
  * [Reference Circuit Details](#reference-circuit-details)
  * [Reference Circuit Diagram](#reference-circuit-diagram)
  * [Reference Circuit Waveform](#reference-circuit-waveform)
  * [Tools and Technology](#tools-and-technology)
  * [Simulation in eSim](#simulation-in-eSim)
  * [Implementation in eSim](#implementation-in-esim)
  * [Analysis](#analysis)
  * [Conclusion](#conclusion)
  * [Author](#author)
  * [Acknowledgement](#acknowlegement)
  * [References](#references)

## Abstract

This paper presents the design and analysis of the Gilbert Cell Mixer using IHP SG13G2 technology. The proposed mixer provides **high gain performance** and **good linearity**. DC, Transient, and AC analyses were performed to evaluate key performance parameters. The mixer achieves a **conversion gain of approximately 2.5 dB** with an **operating frequency of 2 GHz**.

## Reference Circuit Details
<img width="311" height="172" alt="image" src="https://github.com/user-attachments/assets/2331889f-05f6-4ace-aec0-b78a63f3af38" />

## Reference Circuit Diagram
<img width="311" height="297" alt="circuit" src="https://github.com/user-attachments/assets/c48081f3-c060-423d-b2b3-6d5755b2e8e3" />

## Reference Circuit Waveform
<img width="376" height="255" alt="image" src="https://github.com/user-attachments/assets/5bab5f4b-6c91-4316-b58b-6a2f596536ca" />








## Tools and Technology

- **Design Tool:** eSim : eSim is an open-source Electronic Design Automation (EDA) tool developed by FOSSEE, IIT Bombay, for circuit design, simulation, and PCB design.
  It integrates multiple open-source tools (KiCad, ngspice ..) to provide a complete environment for analog, digital, and mixed-signal circuit simulation.
- **Process Technology:** IHP SG13G2 (130 nm SiGe BiCMOS)   

# Simulation in eSim

## Implementation in eSim
<img width="967" height="577" alt="image" src="https://github.com/user-attachments/assets/61d9b0aa-8309-4318-952f-bb41bce110ff" />

## Analysis 

### DC
The DC analysis determined the valid RF bias range between 0.6 V and 0.8 V, confirming proper transistor operation.

<img width="625" height="477" alt="image" src="https://github.com/user-attachments/assets/01fc4267-2167-4c55-b3d3-fdab5a218071" />


### Transient
In transient analysis, the RF signal of 0.1 GHz and LO signal of 2 GHz were applied to the Gilbert cell. The output waveform shows a modulated pattern, confirming the mixing action.

RF INPUT WAVEFORM : V(VRF+) - V(VRF-)
where, VRF​+ = 0.7 + 5 mV⋅sin(2πfRF​t)  
VRF- = 0.7 - 5 mV⋅sin(2πfRF​t)
fR = 0.1GHz

<img width="647" height="464" alt="image" src="https://github.com/user-attachments/assets/4ed6d0d3-b51f-4700-bded-ce87f67fa46c" />


LO INPUT : V(VLO+) - V(VLO-)
where, VLO​+ = 1 + 5 mV⋅sin(2πfLO​t)  
VLO- = 1 - 5 mV⋅sin(2πfLOt)
fLO = 2GHz

<img width="656" height="467" alt="image" src="https://github.com/user-attachments/assets/07373ec5-9e27-4c05-9098-52aec1e4a671" />

MODULATED OUTPUT : V(VOUT+) - V(VOUT-)

<img width="656" height="468" alt="image" src="https://github.com/user-attachments/assets/881bfe18-2614-4737-8ca4-7f9bbcdf7ea1" />



### AC
The AC analysis of the designed Gilbert cell mixer shows a maximum small-signal voltage gain of 2.5 dB with a 3 dB bandwidth of 5 GHz. The results indicate that the mixer provides stable gain performance over a wide frequency range.

<img width="1105" height="484" alt="image" src="https://github.com/user-attachments/assets/4525520c-5806-427b-835b-2c015aeed34e" />

<img width="1138" height="482" alt="image" src="https://github.com/user-attachments/assets/733d71c7-a863-4c03-88ce-ffc9bc37d9e9" />

## Conclusion 
The Gilbert cell mixer was successfully designed and analyzed using the IHP SG13G2 technology. Transient and AC analyses were performed to verify its functionality and frequency response. The circuit achieved a maximum small-signal gain of 2.5 dB with a 3 dB bandwidth of 5 GHz.

For future work, further analyses will be carried out to fully qualify the mixer’s performance. These include noise figure analysis, conversion gain and loss characterization, linearity tests such as 1 dB compression point (P1dB) and third-order intercept point (IIP3/OIP3), isolation measurements between LO, RF, and IF ports, and power consumption evaluation. These parameters are essential to comprehensively assess the efficiency and suitability of the mixer for RF front-end applications.

## Author
Ajay G Nayak, self.

## Acknowledgement
1. FOSSEE, IIT Bombay
2. Sumanto Kar, eSim Team, FOSSEE

## References
1. M. O. Bekkaoui, "Gilbert cell Mixer design in 65nm CMOS technology," 2017 4th International Conference on Electrical and Electronic Engineering (ICEEE), Ankara, Turkey, 2017, pp. 67-72.
2. U. A. Belorkar, S. A. Ladhake and S. N. Kale, "2.45 GHz Gilbert Mixer using 45 nm CMOS technology," 2012 IEEE Business, Engineering \& Industrial Applications Colloquium (BEIAC), 2012.
