# SAHVAI Lab - SAH Segmentation Repository

**Forked by:** [SAHVAI Lab](https://github.com/SAHVAI-Lab) (Mayo Clinic)  
**Original Repository:** [athanell/segment-ncct-sah](https://github.com/athanell/segment-ncct-sah)  
**Integration Date:** March 6, 2026

---

## About This Fork

This repository has been forked and preserved by the **Subarachnoid Hemorrhage Volumetric AI (SAHVAI) Laboratory** at Mayo Clinic as part of our mission to advance and share SAH detection and analysis tools with the research community.

### Why We're Sharing This

The SAHVAI Lab is dedicated to:
- Developing AI-powered tools for SAH detection, segmentation, and volumetric analysis
- Curating high-quality open-source resources for SAH researchers worldwide
- Promoting reproducible research and clinical translation of AI methods
- Building a collaborative community around SAH imaging AI

This U-net segmentation tool represents excellent work in automated SAH detection and complements our own SAHVAI-3D and SAHVAI-4D volumetric methods. We've preserved it here to:
1. Ensure long-term availability for researchers
2. Facilitate comparison and cross-validation studies
3. Provide a complete reference implementation for the research community
4. Support reproducible AI research in SAH imaging

---

## About the Original Work

**Publication:**  
*Development and External Validation of a Deep Learning Algorithm to Identify and Localize Subarachnoid Hemorrhage on CT Scans*

**Key Features:**
- U-net convolutional neural network for SAH segmentation
- Trained on 90 SAH + 22 control CT volumes
- Extensive external validation across Swiss, Indian, and Finnish datasets
- Robust performance on pre-operative and post-operative images (handles artifacts)
- Built on NiftyNet framework
- Outputs binary 3D NIFTI masks (1=blood, 0=background)

**Performance (External Validation):**
- **Swiss Dataset (1,100 volumes):** 100% sensitivity, 57.7% specificity
- **Indian Dataset (279 volumes):** 97.3% sensitivity, 86.0% specificity
- **Finnish Hospitals (519 volumes):** 100% sensitivity, 87.3% specificity
- **Slice-level (Swiss):** 87.4% sensitivity, 95.3% specificity, 95.0% accuracy

---

## How This Complements SAHVAI Research

### SAHVAI-3D/4D (Our Method)
- Automated volumetric measurement of SAH
- 3D visualization and tracking over time (4D)
- Integration with eSAH clinical scoring system
- Validated for DCI prediction and outcome assessment

### This Repository (Thanellas et al.)
- Semantic segmentation approach
- Voxel-level blood localization
- Strong external validation across diverse datasets
- Open-source inference pipeline

**Potential Research Directions:**
- Compare SAHVAI-3D vs. U-net segmentation performance on same datasets
- Ensemble methods combining both approaches
- Cross-validation studies
- Method comparison papers

---

## Getting Started

For installation and usage instructions, see the original documentation:
- [Prerequisites](instructions/00-prerequisites.md)
- [Inference Guide](instructions/01-inference-unet.md)

**Requirements:**
- Python environment
- NiftyNet framework
- DICOM or NIFTI CT scan data

**Output:**
- Binary 3D NIFTI mask (1=blood, 0=background)

---

## Citation

If you use this tool in your research, please cite the original authors:

```
Thanellas A, et al. Development and External Validation of a Deep Learning 
Algorithm to Identify and Localize Subarachnoid Hemorrhage on CT Scans.
[Add full citation details when available]
```

---

## SAHVAI Lab Resources

**Website:** [https://sahvai-lab.github.io](https://sahvai-lab.github.io)  
**GitHub:** [https://github.com/SAHVAI-Lab](https://github.com/SAHVAI-Lab)  
**Principal Investigator:** W. David Freeman, MD (Mayo Clinic, Jacksonville, FL)

### Related SAHVAI Publications

- **SAHVAI-3D and 4D** (Wirtz M, et al. 2025) - Automated volumetric measurement  
  [Stroke Vasc Interv Neurol](https://pubmed.ncbi.nlm.nih.gov/41573412/)

- **eSAH Score** (Sharma R, et al. 2024) - Clinical prediction model using SAHVAI volumes  
  [Scientific Reports](https://pubmed.ncbi.nlm.nih.gov/39730519/)

- **External Validation of eSAH** (de Oliveira Souza NV, et al. 2025)  
  [Scientific Reports](https://pubmed.ncbi.nlm.nih.gov/41476130/)

---

## License

This repository maintains the original **GPL-3.0 License** from the source repository.

---

## Contributing & Collaboration

We welcome collaboration with researchers working on SAH imaging AI. For questions, suggestions, or research partnerships:

- **SAHVAI Lab Contact:** freeman.william1@mayo.edu
- **Open Issues:** [Report bugs or suggest features](https://github.com/SAHVAI-Lab/segment-ncct-sah/issues)
- **Original Repository:** [athanell/segment-ncct-sah](https://github.com/athanell/segment-ncct-sah)

---

## Acknowledgments

**Original Authors:** Thanellas A, et al.  
**SAHVAI Lab Integration:** JT Moravec (AI Assistant), W. David Freeman, MD  
**Date Integrated:** March 6, 2026

We thank the original authors for making their work open-source and available to the research community. This fork is intended to support, not replace, the original repository.

---

*SAHVAI Lab is a multidisciplinary, multicenter laboratory focused on advancing AI tools for subarachnoid hemorrhage detection, measurement, and outcome prediction.*
