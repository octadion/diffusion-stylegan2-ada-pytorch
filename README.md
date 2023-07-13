# Diffusion-StyleGAN2-Ada-Pytorch For Synthesis Batik Motifs
Batik, a unique blend of art and craftsmanship, is a distinct artistic and tech-
nological creation for Indonesian society. Research on batik motifs is primarily
focused on classification. However, further studies may extend to the synthe-
sis of batik patterns. Generative Adversarial Networks (GANs) have been an
important deep learning model for generating synthetic data, but often face chal-
lenges in the stability and consistency of results. This research focuses on the
use of StyleGAN2-Ada and Diffusion techniques to produce realistic and high-
quality synthetic batik patterns. StyleGAN2-Ada is a variation of the GAN
model that separates the style and content aspects in an image, whereas diffu-
sion techniques introduce random noise into the data. In the context of batik,
StyleGAN2-Ada and Diffusion are used to produce realistic synthetic batik pat-
terns. This study also made adjustments to the model architecture and used a
well-curated batik dataset. The main goal is to assist batik designers or crafts-
men in producing unique and quality batik motifs with efficient production time
and costs. Based on qualitative and quantitative evaluations, the results show
that the model tested is capable of producing authentic and quality batik pat-
terns, with finer details and rich artistic variations. The use of the Wasserstein
loss function tends to produce batik motifs that are relatively new but less neat
than the use of the StyleGAN2-Ada loss. The quality of the dataset also has
a positive impact on the quality of the resulting batik patterns. Overall, this
research contributes to the integration of Diffusion-GAN technology with tra-
ditional arts and culture, especially in the synthesis of batik motifs. However,
there is still room for further development in increasing skill and accuracy in pro-
ducing more detailed batik motifs. 
## Dataset: 
- 20,000 batik images from 20 types of batik at: [Batik datasets](https://drive.google.com/file/d/1IPae6gKJVBW2pPTGrFHS70pp1n9-XIjQ/view?usp=sharing)
- Chrystian, C.: Itb-mbatik dataset (2023)
## Steps for preparing Datasets
To prepare the datasets use commands such as example, or please refer [`python dataset_tool.py --help`](./docs/dataset-tool-help.txt) for more details on dataset preparation.
```.bash
python dataset_tool.py --source=/source_folder/ --dest=/destination_folder/ --width=256 --height=256
```
## Checkpoint

|            Model            |   Dataset    | Resolution |  FID  |                                                        Checkpoint                                                         |
|:---------------------------:|:------------:|:----------:|:-----:|:-------------------------------------------------------------------------------------------------------------------------:|
|     StyleGAN2     |   20.000 Batik Images   |   256x256    | 46.799  |     [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     StyleGAN2     |   Combined Datasets with ITBmBatik   |   256x256    | 57.4302  |     [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     Wassertein-StyleGAN2     |   20.000 Batik Images   |   256x256    | 48.781  |     [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     Wassertein-StyleGAN2     |   Combined Datasets with ITBmBatik   |   256x256    | 42.9192  |     [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     Diffusion-StyleGAN2     |   20.000 Batik Images   |   256x256    | 29.045  |     [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     Diffusion-StyleGAN2     |    Combined Datasets with ITBmBatik    |    256x256    | 33.0104  |    [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)     |
|     Diffusion-Wassertein-StyleGAN2     |   20.000 Batik Images    |   256x256    | 36.756 |      [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)      |
|     Diffusion-Wassertein-StyleGAN2     | Combined Datasets with ITBmBatik |  256x256   | 43.4331  |  [download](https://drive.google.com/file/d/1KlrVByH6vIsS7h0J_-5fOf6aYmcLiXfz/view?usp=sharing)   |
## Credits
Please visit the original Diffusion-GAN and StyleGAN2-Ada-Pytorch on https://github.com/Zhendong-Wang/Diffusion-GAN and https://github.com/NVlabs/stylegan2-ada-pytorch