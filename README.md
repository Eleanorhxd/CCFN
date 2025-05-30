# CCFN: Collaborative cross-modal fusion network for radiology report generation


## Highlight

- 1.	Proposes a collaborative cross-modal fusion network for radiology report generation.
- 2.	Constructs visual collaborative enhancement module to accurately identify abnormal lesions.
- 3.	Designs cross-modal semantic fusion to perform information alignment between different modalities.


## Requirements
- `Python >= 3.6`
- `Pytorch >= 1.7`
- `torchvison`

## Data

Download IU X-Ray and MIMIC-CXR datasets, and place them in `data` folder.

- IU X-Ray dataset is available  from [here](https://iuhealth.org/find-medical-services/x-rays)
- MIMIC-CXR dataset is available from [here](https://physionet.org/content/mimic-cxr-jpg/2.0.0/)

## Folder Structure
- config : setup training arguments and data path
- data : store IU and MIMIC dataset
- models:  our model
- modules: 
    - the layer define of our model 
    - dataloader
    - loss function
    - metrics
    - tokenizer
    - some utils
- preprocess: data preprocess
- pycocoevalcap: Microsoft COCO Caption Evaluation Tools

## Training & Testing

The source code for training can be found here：

Run `train.py` to train a model on the IU X-Ray data and MIMIC-CXR data.

Run `test.py` to test a model on the IU X-Ray data and MIMIC-CXR.

To run the command, you only need to specify the config file and the GPU ID and iteration version of the model to be used

## Acknowledgement
We appreciate for all code providers, especially for [R2GenCMN]([https://github.com/foxlf823/Multi-Filter-Residual-Convolutional-Neural-Network](https://github.com/zhjohnchan/R2GenCMN)).
