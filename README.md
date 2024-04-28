# On Calibration of Modern Medical Vision-Language Models

## Approach

![alt text](./figs/zero_shot_acc_vs_ece2.png)

An extensive empirical investigation across different models, datasets, and prompting
strategies showed that medical vision-language models tend to be largely unreliable out-of-the-box in the zero-shot setting.

## Setup

Requires python >= 3.10, [uncertainty calibration](https://pypi.org/project/uncertainty-calibration/) library, and [OpenAI's CLIP](https://pypi.org/project/open-clip-torch/) library.

## Acquiring Raw Data and Models

The 12 datasets used can be downloaded from:
| Dataset            | Source                                                                                  |
| ------------------ | ----------------------------------------------------------------------------------------|
| Databiox           | https://databiox.com/datasets/                                                          |
| SICAPv2            | https://data.mendeley.com/datasets/9xxm58dvs3/1                                         |
| Skin Cancer        | https://heidata.uni-heidelberg.de/dataset.xhtml?persistentId=doi:10.11588/data/7QCR8S   |
| Renal Cell         | https://zenodo.org/records/7898308                                                      |
| BACH               | https://zenodo.org/records/3632035/files/ICIAR2018_BACH_Challenge.zip                   |
| NCT-NRC            | https://zenodo.org/records/1214456/files/NCT-CRC-HE-100K.zip                            |
| PCAM               | https://patchcamelyon.grand-challenge.org/                                              |
| MHIST              | https://bmirds.github.io/MHIST/                                                         |
| Osteo              | https://www.cancerimagingarchive.net/collection/osteosarcoma-tumor-assessment/          |
| LC25000 (LUNG)     | https://huggingface.co/datasets/1aurent/LC25000                                         |
| LC2500 (Colon)     | https://huggingface.co/datasets/1aurent/LC25000                                         |

The 3 models used can be sourced from: [QuiltNet](https://github.com/wisdomikezogwo/quilt1m), [BioMedCLIP](https://huggingface.co/microsoft/BiomedCLIP-PubMedBERT_256-vit_base_patch16_224), [PLIP](https://huggingface.co/vinid/plip).


