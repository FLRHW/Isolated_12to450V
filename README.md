<p align="center" width="100%">
  <a href="https://github.com/FLRHW/StepUp_module_12to450V/actions/workflows/ci.yaml">
    <img alt="CI Badge" src="https://github.com/FLRHW/StepUp_module_12to450V/actions/workflows/ci.yaml/badge.svg?branch=">
  </a>
</p>

<p align="center" width="100%">
    <img src="Logos/module.png">
</p>

***

<p align="center">
  <img alt="3D Top Angled" src="Images/StepUp_module_12to450V-angled_top.png" width="45%">
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="3D Bottom Angled" src="Images/StepUp_module_12to450V-angled_bottom.png" width="45%">
</p>

***

# **StepUp_module_12to450V**
This repository contains a reverse‑engineered KiCad schematic and PCB layout from a commercial module originally purchased from AliExpress.

## Project overview
This project documents the electrical design and PCB layout of a third‑party module by recreating them from scratch in KiCad for learning, repair, and interoperability purposes. The repository does not include any original vendor design files, firmware, branding, or trademarks.

## Origin and scope
Original hardware: generic module purchased from AliExpress (exact vendor and listing may change over time, the following terms can help finding similar modules: "70W DC-DC 12V 24V To 200V-450V Voltage Adjustable Boost Power Converter Nixie Clock Tube Amplifier Capacitor Charging").  
Status: unofficial, reverse‑engineered reference design; not affiliated with, endorsed by, or supported by the original manufacturer or seller.  
Contents: KiCad schematic, PCB layout, netlists, and supporting documentation created from measurements and inspection of a physical unit.

## Intended use
This repository is intended for:
* Educational use and study of the circuit;
* Repair, modification, or replacement of compatible hardware;
* Integration into hobby or research projects, subject to any third‑party IP that may apply in your jurisdiction. Users are responsible for checking any patent, copyright, or regulatory constraints that may apply to their own use.

## License
The KiCad design files and documentation in this repository are released under the CERN Open Hardware Licence v2 – Permissive (CERN‑OHL‑P‑2.0). SPDX identifier: CERN-OHL-P-2.0 See the LICENSE file for the full legal text and conditions.  
In short and non‑legal terms, you are free to use, modify, manufacture, and distribute hardware based on these files, provided you respect attribution requirements and the terms in the license.

## Trademarks and third‑party rights
All product names, logos, and brands of the original module are the property of their respective owners and are not included or licensed here.  
Any reference to third‑party marks is purely descriptive and does not imply endorsement or affiliation.  
If you are the rights holder for the original hardware and have concerns about this documentation, please open an issue in the repository.

## Safety and disclaimer
* The design is provided as is, with no warranty of any kind;
* Use it at your own risk; always review the schematic, layout, and component ratings before using it;
* High voltage can cause injury, death, or damage to equipment; ensure appropriate protections and testing procedures.

## Contributing
Contributions are welcome. Please use pull requests and issues to propose changes or discuss potential improvements.

***

## DIRECTORY STRUCTURE
    │
    ├─ Computations       # Misc calculations
    ├─ HTML               # HTML files for generated webpage
    ├─ Images             # Pictures and renders
    │
    ├─ kibot_resources    # External resources for KiBot
    │  ├─ colors          # Color theme for KiCad
    │  ├─ fonts           # Fonts used in the project
    │  ├─ scripts         # External scripts used with KiBot
    │  └─ templates       # Templates for KiBot generated reports
    │
    ├─ kibot_yaml         # KiBot YAML config files
    ├─ KiRI               # KiRI (PCB diff viewer) files
    │
    ├─ lib                # KiCad footprint and symbol libraries
    │  ├─ 3d_models       # Component 3D models
    │  ├─ lib_fp          # Footprint libraries
    │  └─ lib_sym         # Symbol libraries
    │
    ├─ Logos              # Logos
    │
    ├─ Manufacturing      # Assembly and fabrication documents
    │  ├─ Assembly        # Assembly documents (BoM, pos, notes)
    │  │
    │  └─ Fabrication     # Fabrication documents (ZIP, notes)
    │     ├─ Drill Tables # CSV drill tables
    │     └─ Gerbers      # Gerbers
    │
    ├─ Report             # Reports for ERC/DRC
    ├─ Schematic          # PDF of schematic
    ├─ Templates          # Title block templates
    ├─ Testing
    │  └─ Testpoints      # Testpoints tables      
    │
    └─ Variants           # Outputs for assembly variants
