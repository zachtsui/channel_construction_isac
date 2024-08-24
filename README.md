## channel_construction_isac -- Matlab simulation 
The project constructs communication channels based on sensing channels
### System Model ####
In an ISAC system, there are two TRXs with identical mono-static sensing capacities, each of which serves as Tx or Rx in the communication process.
sensing channel1: $h_{T} = \sum_{p=1}^{P} \alpha_p \exp(-j 2\pi f_c \tau_p) \delta(\tau-\tau_p) \delta(\phi_{\rm AOD}-\phi_p)$, 
sensing channel2: $h_{R} = \sum_{k=1}^{K} \beta_k \exp(-j 2\pi f_c \tau_k) \delta(\tau-\tau_k) \delta(\phi_{\rm AOA}-\phi_k)$, 
constructing communication channel:  $h(\tau,\psi, \varphi) = \sum_{i=1}^{C} \eta_i \exp(-j 2\pi f_c \tau_i) \delta(\tau-\tau_i) \delta(\psi-\psi_i)\delta(\varphi-\varphi_i)$.
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
