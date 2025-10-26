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

### Transient
RF INPUT : V(VRF+) - V(VRF-)
<img width="647" height="464" alt="image" src="https://github.com/user-attachments/assets/4ed6d0d3-b51f-4700-bded-ce87f67fa46c" />


LO INPUT : V(VLO+) - V(VLO-)

<img width="656" height="471" alt="image" src="https://github.com/user-attachments/assets/073c026c-2c45-4bd2-a06b-239b94386f93" />

VOUT : V(VOUT+) - V(VOUT-)

<img width="650" height="470" alt="image" src="https://github.com/user-attachments/assets/64056d17-12a0-47bb-8252-ec473f220f41" />



### AC

<img width="1105" height="484" alt="image" src="https://github.com/user-attachments/assets/4525520c-5806-427b-835b-2c015aeed34e" />

<img width="1138" height="482" alt="image" src="https://github.com/user-attachments/assets/733d71c7-a863-4c03-88ce-ffc9bc37d9e9" />


## Author
Ajay G Nayak, self.

## Acknowledgement
1. FOSSEE,IIT Bombay
2. Sumanto Kar, eSim Team, FOSSEE

## References


