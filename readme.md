# Adapted Modular Scimitar with Payload Mounting Grid

Repository of the HardwareX paper "Field-tested workflow for adapting open-source 3D-printed fixed-wing UAVs for modular payload integration" developed at University of Southern Denmark.

## Abstract

Fixed-wing unmanned aerial vehicles (UAVs) are widely used in environmental monitoring and research, yet sys-
tematic and reproducible methods for integrating arbitrary payloads while preserving aerodynamic performance
remain limited. This work presents a complete hardware workflow for adapting an open-source fixed-wing air-
frame into a modular sensing platform with validated payload integration. The approach combines mechanical
redesign, mass and center of gravity verification, computational fluid dynamics (CFD) aerodynamic assess-
ment, and field validation. The workflow is demonstrated on a sub-1.5 kg 3D-printed Scimitar V2 modified to
be equipped with a reconfigurable payload mounting grid that enables rapid sensor interchange. CFD-guided
design iteration increased aerodynamic efficiency by raising the lift-to-drag ratio from approximately 3.6–5.1
to 8.8–18.2, providing quantitative pre-fabrication screening indicating improved aerodynamic efficiency. Field
testing at RC Parken (Aabenraa, Denmark) in December 2025 validated the sensor logging pipeline by cross-
comparing barometric pressure and demonstrated in-flight temperature and humidity acquisition.

## Directory Structure

```
├── readme.md                    # This file
├── 3D_Printing/                 # 3D printable components
│   ├── 019_Canopy_handle.3mf
│   └── TPU/                     # Flexible TPU parts
│       └── 015_Hinges_TPU.3mf
├── CAD/                         # Complete CAD models (STEP format)
│   ├── Fuselage sections (001-007)
│   ├── Wing designs (008-013)
│   ├── Control surfaces (014-016)
│   ├── Canopy (017, 019)
│   ├── Sensor and component models (018, 020-035)
│   └── [35 STEP files total]
├── CFD/                         # Aerodynamic analysis files
│   ├── project_results.xml
│   ├── Internal_M5GO.*          # Simulation results
│   └── r_000000.fld             # Field data
├── M5 Software/                 # M5Stack firmware
│   └── Drone_Air_Quality_Code.m5f2
├── PX4 Firmware/                # Autopilot configuration
│   ├── Parameters.params        # Pre-tuned parameters
│   └── readme.txt
└── Media/                       # Assembly documentation
    └── Assembly/
```

## License

This project is released under CC BY 4.0.

For questions, contributions, or feedback, please refer to the project repository or contact the team.