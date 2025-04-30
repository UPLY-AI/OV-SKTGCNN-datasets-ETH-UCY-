# Dataset Repository for: Enhanced Pedestrian Trajectory Prediction via Overlapping Field-of-View Domains and Integrated Kolmogorov-Arnold Networks (OV-SKTGCNN)

[![License](https://img.shields.io/badge/Data_License-CC_BY_NC_4.0-blue.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

This repository serves as a documentation hub for the trajectory datasets used in the OV-SKTGCNN model. **Note:** This repository does NOT contain any code or model implementations - it solely provides dataset provenance information.

## Dataset Provenance

The trajectory data used in our study follows the exact implementation from Social-STGCNN [[17]](https://arxiv.org/abs/2002.11927), processed from two public pedestrian video sources:

### Original Video Sources
1. **ETH Pedestrian Dataset**  
   Original videos published by Pellegrini et al. [[27]](https://doi.org/10.1109/ICCV.2009.5459260)  
   Access raw videos at: https://data.vision.ee.ethz.ch/cvl/aem/ewap_dataset_full.tgz

2. **UCY Crowd Dataset**  
   Original videos published by Lerner et al. [[28]](https://doi.org/10.1111/j.1467-8659.2007.01089.x)
   Access raw videos at: https://graphics.cs.ucy.ac.cy/research/downloads/crowd-data

### Processed Trajectory Data
The structured trajectory files containing:
- Agent positions in world coordinates
- Velocity measurements
- Timestamp information

Are available through the Social-STGCNN GitHub repository:  
https://github.com/abduallahmohamed/Social-STGCNN

The data schema and preprocessing methodology are fully described in the original Social-STGCNN paper [[17]](https://arxiv.org/abs/2002.11927).

## Data Compatibility Verification
Our OV-SKTGCNN implementation maintains strict compatibility with the original data format:
- No modifications to data structures
- Preserved original sampling rates (2.5 Hz)
- Consistent coordinate normalization
- Identical train/test splits

This ensures direct comparability with baseline models using the same dataset configuration.

## Usage Notes
This repository is provided for:
- Transparent documentation of data provenance
- Easy reference for replication studies
- Comparison with our OV-SKTGCNN results

**All dataset copyright remains with the original authors.** Please observe the license terms from both the original video sources and the Social-STGCNN repository when using this data.

## Citation
When using this data configuration, please cite both the original datasets and the Social-STGCNN processing methodology:
```bibtex
@INPROCEEDINGS{5459260,
  author={Pellegrini, S. and Ess, A. and Schindler, K. and van Gool, L.},
  booktitle={2009 IEEE 12th International Conference on Computer Vision}, 
  title={You'll never walk alone: Modeling social behavior for multi-target tracking}, 
  year={2009},
  volume={},
  number={},
  pages={261-268},
  keywords={Predictive models;Vehicle dynamics;Layout;Humans;Computer vision;Trajectory;Cameras;Legged locomotion;Path planning;Computer science},
  doi={10.1109/ICCV.2009.5459260}}

@inproceedings{lerner2007crowds,
  title={Crowds by example},
  author={Lerner, Alon and Chrysanthou, Yiorgos and Lischinski, Dani},
  booktitle={Computer graphics forum},
  volume={26},
  number={3},
  pages={655--664},
  year={2007},
  organization={Wiley Online Library}
}

@article{almomen2020social,
  title={Social-STGCNN: A Social Spatio-Temporal Graph Convolutional Neural Network for Human Trajectory Prediction},
  author={Almomen, Abduallah and Kim, Kyungtae and How, Jonathan},
  journal={arXiv preprint arXiv:2002.11927},
  year={2020}
}
