## channel_construction_isac -- Matlab simulation 
The project constructs communication channels based on sensing channels
### System Model ####
In an ISAC system, there are two TRXs with identical mono-static sensing capacities, each of which serves as Tx or Rx in the communication process.
### Parameters ###
For the simulation, we can change various system parameters to obtain distinct channel characteristics. 
1. Geometry parameters include the distance between Tx and Rx, the sensing circles and communication ellipse are determined by the carrier/frequency spacing $\Delta f$.
   note that you can vary the Tx-Rx separation to mimic different scenarios, for example, when separation is 5 m, the simulated scenario can be regarded as indoor.
2. Environment parameters mainly include the number of scatterers and their radar cross-section (RCS) features. We assume that the RCS is an RV following exponential distribution based on the literature.
3. System parameters include frequency, bandwidth,...etc.
### Results ###
Time-frequency domain: we can obtain a complex channel impulse response (CIR) using the simulator, the delay bin is based on the system's bandwidth and spacing. 
Based on this, we can obtain key channel characteristics such as K-factor and RMS delay spread.
Angular domain: we obtain the angular profile based on discrete scatterers. 
Doppler: it is under development
## Citation
to be updated.
## License
The simulation is based on Matlab 2022a.
