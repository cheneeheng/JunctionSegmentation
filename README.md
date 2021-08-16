# JunctionSegmentation
This repository contains the Cityscapes [1] dataset extension for the paper:  

 Pixelwise Traffic Junction Segmentation for Urban Scene Understanding (https://ieeexplore.ieee.org/document/9294654)
   
```
  @inproceedings{chen2020pixelwise,
    title={Pixelwise Traffic Junction Segmentation for Urban Scene Understanding},
    author={Chen, Ee Heng and Hu, Hanbo and Zeisler, J{\"o}ran and Burschka, Darius},
    booktitle={2020 IEEE 23rd International Conference on Intelligent Transportation Systems (ITSC)},
    pages={1--8},
    year={2020},
    organization={IEEE},
    doi={10.1109/ITSC45102.2020.9294654}
  }
```

 The dataset extension consists of binary junction labels for the densely labeled images (finely annotated). We maintained the original folder structure for ease of use. We provided both the id (34) and trainid (19) for the junction label which can be added into "cityscapesscripts/helpers/labels.py" for evaluation.

* The following line was added into "cityscapesscripts/helpers/labels.py" to obtain the results shown in the paper.
_Label('junction' , 34 , 19 , 'flat' , 1 , False , False , (  0, 255, 0) )_
* Link to Cityscapes dataset : https://www.cityscapes-dataset.com/
* Link to Cityscapes evaluation script : https://github.com/mcordts/cityscapesScripts

[1] M. Cordts, M. Omran, S. Ramos, T. Rehfeld, M. Enzweiler, R. Benenson, U. Franke, S. Roth, and B. Schiele, The cityscapes dataset for semantic urban scene understanding, in Proceedings of the IEEE conference on computer vision and pattern recognition, 2016, pp. 3213-3223.

