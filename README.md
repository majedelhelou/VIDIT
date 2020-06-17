# VIDIT: Virtual Image Dataset for Illumination Transfer

We will be releasing more data (including depth maps per image) in the coming weeks/months, you can *watch* the repository if you would like to be notified.

:fire: **News** :fire: VIDIT is used for the relighting challenge in the [AIM workshop](https://data.vision.ee.ethz.ch/cvl/aim20/), part of ECCV 2020. Check out the [relighting competition](https://competitions.codalab.org/competitions/24671) beginning May 13th 2020, it is made up of 3 tracks for [one-to-one](https://competitions.codalab.org/competitions/24671) and [any-to-any](https://competitions.codalab.org/competitions/24674) illumination transfer, and for [illumination estimation](https://competitions.codalab.org/competitions/24773).

### [Paper](https://arxiv.org/abs/2005.05460)

> **Abstract:** *Deep image relighting is gaining more interest lately, as it allows photo enhancement through illumination-specific retouching without human effort. Aside from aesthetic enhancement and photo montage, image relighting is valuable for domain adaptation, whether to augment datasets for training or to normalize input test data. Accurate relighting is, however, very challenging for various reasons, such as the difficulty in removing and recasting shadows and the modeling of different surfaces. We present a novel dataset, the Virtual Image Dataset for Illumination Transfer (VIDIT), in an effort to create a reference evaluation benchmark and to push forward the development of illumination manipulation methods. Virtual datasets are not only an important step towards achieving real-image performance but have also proven capable of improving training even when real datasets are possible to acquire and available. VIDIT contains 300 virtual scenes used for training, where every scene is captured 40 times in total: from 8 equally-spaced azimuthal angles, each lit with 5 different illuminants.*

## Content
VIDIT includes 390 different Unreal Engine scenes, each captured with 40 illumination settings, resulting in 15,600 images. The illumination settings are all the combinations of 5 color temperatures (2500K, 3500K, 4500K, 5500K and 6500K) and 8 light directions (N, NE, E, SE, S, SW, W, NW). Original image resolution is 1024x1024.

<p align="center">
  <img src="gifs/diagram.png" width="300px"/>
</p>

### Examples with varying direction
<p align="center">
<img src="gifs/A_directions.gif" width="200" /> 
<img src="gifs/B_directions.gif" width="200" />
<img src="gifs/C_directions.gif" width="200" /> 
<img src="gifs/D_directions.gif" width="200" />
</p>


### Examples with varying color temperature
<p align="center">
<img src="gifs/A_illuminants.gif" width="200" /> 
<img src="gifs/B_illuminants.gif" width="200" />
<img src="gifs/C_illuminants.gif" width="200" /> 
<img src="gifs/D_illuminants.gif" width="200" />
</p>

## Getting the data
The **training** dataset in full 1024x1024 resolution is available for download:

**[Mirror 1](https://drive.google.com/open?id=1i_2lIXi-gXgIouDCYnfrdtY3wzTiH1E9)**

**[Mirror 2](https://datasets.epfl.ch/vidit/VIDIT_train.zip)**

Validation data is gradually made available to the ECCV 2020 competition participants, it will be made available here soon. Test data will remain private.

## Citation

    @article{elhelou2020vidit,
        title={{VIDIT}: Virtual Image Dataset for Illumination Transfer},
        author={El Helou, Majed and Zhou, Ruofan and Barthas, Johan and S{\"u}sstrunk, Sabine},
        journal={arXiv preprint arXiv:2005.05460},
        year={2020}
    }
