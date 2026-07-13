# Mock Data Set


📁 default.hdf
│
├── 📁 injection_parameters
│   ├── 📄 chirp_distance: The luminosity distance scaled by the system's chirp mass, dictating absolute amplitude.
│   ├── 📄 coa_phase: Coalescence phase of the binary at the merger moment, defining initial wave orientation.
│   ├── 📄 dec: Declination coordinate of the source in the sky, used for antenna projection.
│   ├── 📄 h1_signal: The pure, raw, noiseless gravitational wave template generated for the H1 detector.
│   ├── 📄 h1_snr: The calculated optimal Signal-to-Noise Ratio (SNR) of the injected wave in H1.
│   ├── 📄 inclination: The angle between the binary's orbital angular momentum and the observer's line of sight.
│   ├── 📄 l1_signal: The pure, raw, noiseless gravitational wave template generated for the L1 detector.
│   ├── 📄 l1_snr: The calculated optimal Signal-to-Noise Ratio (SNR) of the injected wave in L1.
│   ├── 📄 mass1: Mass of the primary (heavier) compact object in solar masses (M_sun).
│   ├── 📄 mass2: Mass of the secondary (lighter) compact object in solar masses (M_sun).
│   ├── 📄 polarization: The polarization angle of the incident gravitational wave relative to the detectors.
│   ├── 📄 ra: Right Ascension coordinate of the source in the sky, used for time-of-flight delays.
│   └── 📄 scale_factor: The numerical multiplier applied to the 1.0 Mpc template to reach the target amplitude.
│
├── 📁 injection_samples
│   ├── 📄 event_time: The precise GPS time anchor where the simulated merger peak sits in this window.
│   ├── 📄 h1_strain: Processed data segment for H1 containing Real Noise + Scaled/Shifted Injection.
│   └── 📄 l1_strain: Processed data segment for L1 containing Real Noise + Scaled/Shifted Injection.
│
├── 📁 noise_samples
│   ├── 📄 event_time: The reference GPS time associated with this window for alignment and auditing.
│   ├── 📄 h1_strain: Processed H1 data segment consisting strictly of Pure Real-World Noise.
│   └── 📄 l1_strain: Processed L1 data segment consisting strictly of Pure Real-World Noise.
│
├── 📁 normalization_parameters
│   └── 📄 [metadata]: Calibration scalars (mean, std dev) used to standardize or whiten input tensors before training.
│
└── 📁 static_arguments
    └── 📄 [metadata]: Configuration constants tracking sampling rate, frequency cutoffs, and window durations. # FIXME: I think it is empty