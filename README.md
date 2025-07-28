# AnimalClue: Recognizing Animals by their Traces  
**ICCV 2025 Highlight**

Risa Shinoda<sup>1,2,4</sup>, Nakamasa Inoue<sup>3,4</sup>, Iro Laina<sup>5</sup>, Christian Rupprecht<sup>5</sup>, Hirokatsu Kataoka<sup>4,5</sup>  

<sup>1</sup>Osaka University,  
<sup>2</sup>Kyoto University,  
<sup>3</sup>Tokyo Institute of Technology,  
<sup>4</sup>National Institute of Advanced Industrial Science and Technology (AIST),  
<sup>5</sup>Visual Geometry Group, University of Oxford

---

##  Project Overview

**AnimalClue** is a benchmark dataset designed to recognize wild animals from indirect traces, such as:

- 🐾 Footprints  
- 🚽 Feces  
- 🪺 Eggs  
- 🪶 Feathers  
- 🦴 Bones  

Our goal is to explore whether current models can infer animal identity from trace evidence without directly seeing the animal itself.

All detection models used in our dataset are publicly available, and we followed their original instructions for inference.

##  Dataset 

We provide YOLO-format datasets (bounding boxes + segmentation masks) on Hugging Face:

| Category   | Hugging Face Dataset Link                                                 | Format           |
|------------|----------------------------------------------------------------------------|------------------|
| Footprint  | [risashinoda/footprint_yolo](https://huggingface.co/datasets/risashinoda/footprint_yolo) | YOLO (bbox) |
| Feces      | [risashinoda/feces_yolo](https://huggingface.co/datasets/risashinoda/feces_yolo) | YOLO (bbox + seg) |
| Egg        | [risashinoda/egg_yolo](https://huggingface.co/datasets/risashinoda/egg_yolo) | YOLO (bbox + seg) |
| Bones      |[risashinoda/bone_yolo](https://huggingface.co/datasets/risashinoda/bone_yolo)     | YOLO (bbox + seg) |
| Feather    | [risashinoda/feather_yolo](https://huggingface.co/datasets/risashinoda/feather_yolo)                                                | YOLO (bbox + seg) |

Each dataset contains:

- `images/`: training and validation images  
- `labels/`: YOLO-style bounding box annotations  
- `data.yaml`: dataset splits and class info

> You can also extract bounding box data for classification purposes.  
> (We will provide sample code for this soon!)

## ✅ To-Do

We are actively working on the following components to complete the AnimalClue release:

- [x] **Upload YOLO images**  

- [x] **Upload animal taxonomy (species hierarchy)**  

- [ ] **Provide detailed metadata**  

- [ ] **Release sample code for training & evaluation**  

