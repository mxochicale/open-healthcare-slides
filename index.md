Miguel Xochicale

# 

<div style="background-color: rgba(22,22,22,0.75); border-radius: 10px; text-align:center; padding: 0px; padding-left: 1.5em; padding-right: 1.5em; max-width: min-content; min-width: max-content; margin-left: auto; margin-right: auto; padding-top: 0.2em; padding-bottom: 0.2em; line-height: 1.5em!important;">

<span style="color:#939393; font-size:1.5em; font-weight: bold;">Can
Open-Source Software</span>  
<span style="color:#939393; font-size:1.5em; font-weight: bold;">Revolutionise
Healthcare?</span>

<span style="padding-bottom: 0.5rem;"><br> </span>  
[](http://mxochicale.github.io/) Miguel Xochicale, PhD  
<span style="font-size:0.8em;"><span style="border-bottom: 0.5px solid #00ccff;">[
`mxochicale/`](https://github.com/mxochicale/)</span><span style="border-bottom: 0.5px solid #00ccff;">[`open-healthcare-slides`](https://github.com/mxochicale/open-healthcare-slides)</span></span>

</div>

<div class="footer">

<span class="dim-text" style="&quot;text-align:left;'">2024-04-20 @
[Link for grid-worms-animation
2023](https://github.com/saforem2/grid-worms-animation/)</span>

</div>

# Overview

- [My trajectory](#sec-mt)
- Uses cases
  - [Fetal Ultrasound Image Synthesis](#sec-fus)
  - Real-time AI diagnosis:
    - Endoscopy-based video
    - eye movement disorders
- Takeaways

## My trajectory

<div id="sec-mt" style="margin-top: 0px; font-size: 50%;">

<img src="figures/mx.svg" style="width:100.0%"
data-fig-align="center" />

</div>

## Dating Ultrasound Scan (12 week scan)

<div id="sec-fus" style="margin-top: 0px; font-size: 10%;">

<img src="figures/fetal-ultrasound-image-synthesis/12-week-scan.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

Wright-Gilbertson M. 2014 in PhD thesis;
https://en.wikipedia.org/wiki/Gestational_age; National-Health-Service
2021. Screening for down’s syndrome, edwards’ syndrome and patau’s
syndrome. https://www.nhs.uk/pregnancy/your- pregnancy- care

</div>

## Challenges of US biometric measurements

- Operator dependant,
- Clinical system dependant,
- Fetal position,
- Similar morphological and echogenic characteristics in the US,
- Few public datasets are available (we have only found two)

<div style="font-size: 40%;">

Sciortino et al. in Computers in Biology and Medicine 2017
https://doi.org/10.1016/j.compbiomed.2017.01.008; He et al. in Front.
Med. 2021 https://doi.org/10.3389/fmed.2021.729978

</div>

## TransThalamic

Fetal Brain Ultrasound Image Dataset

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/fetal-planes-dataset-TransThalami.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

Burgos-Artizzu, X et al. (2020). FETAL PLANES DB: Common maternal-fetal
ultrasound images \[Data set\]. In Nature Scientific Reports (1.0, Vol.
10, p. 10200). Zenodo. https://doi.org/10.5281/zenodo.3904280

</div>

## TransCerebellum Plain

Fetal Brain Ultrasound Image Dataset

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/fetal-planes-dataset-TransCerebellum.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

Burgos-Artizzu, X et al. (2020). FETAL PLANES DB: Common maternal-fetal
ultrasound images \[Data set\]. In Nature Scientific Reports (1.0, Vol.
10, p. 10200). Zenodo. https://doi.org/10.5281/zenodo.3904280

</div>

## TransVentricular Plane

Fetal Brain Ultrasound Image Dataset

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/fetal-planes-dataset-TransVentricular.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

Burgos-Artizzu, X et al. (2020). FETAL PLANES DB: Common maternal-fetal
ultrasound images \[Data set\]. In Nature Scientific Reports (1.0, Vol.
10, p. 10200). Zenodo. https://doi.org/10.5281/zenodo.3904280

</div>

## Research Questions

- Research and implement deep learning methods for generating synthetic
  fetal ultrasound images for both normal and abnormal cases,
- Propose and apply methods to evaluate quantitative and qualitative
  images of fetal us image synthesis.

## GAN-based fetal imaging

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/gan-based-fetal-imaging.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

1)  Bautista et al. 2022, ”Empirical Study of Quality Image Assessment
    for Synthesis of Fetal Head Ultrasound Imaging with DCGANs” MIUA
    https://github.com/budai4medtech/miua2022 (b) Liu et al. 2021
    ”Towards Faster and Stabilized GAN Training for High-fidelity
    Few-shot Image Synthesis” https://arxiv.org/abs/2101.04775

</div>

## AI/ML pipeline

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/ai-pipeline-gans-based-pipeline-fetal-imaging.svg"
style="width:100.0%" data-fig-align="center" />

</div>

## Image Quality Assessment

Quaility of synthesised images are evaluated with Frechet inception
distance (FID), measuring the distance between distributions of
synthetised and original images (Heusel et al., 2017).

The lower the FID number is, the more similar the synthetised images are
to the original ones. FID metric showed to work well with fetal head US
compared to other metrics (Bautista et al., 2012).

<div style="font-size: 40%;">

M. Iskandar et al. “Towards Realistic Ultrasound Fetal Brain Imaging
Synthesis” in MIDL2023. https://github.com/budai4medtech/midl2023

</div>

## Methods

Diffusion-Super-Resolution-GAN (DSR-GAN) Transformer-based-GAN

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/methods-diffusion-Super-Resolution-GAN-transformer-based-GAN.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

M. Iskandar et al. “Towards Realistic Ultrasound Fetal Brain Imaging
Synthesis” in MIDL2023. https://github.com/budai4medtech/midl2023

</div>

## Experiments: Design and results

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/results-only-images.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

M. Iskandar et al. “Towards Realistic Ultrasound Fetal Brain Imaging
Synthesis” in MIDL2023. https://github.com/budai4medtech/midl2023

</div>

## Experiments: Design and results

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img src="figures/fetal-ultrasound-image-synthesis/results-plots.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

M. Iskandar et al. “Towards Realistic Ultrasound Fetal Brain Imaging
Synthesis” in MIDL2023. https://github.com/budai4medtech/midl2023

</div>

##  github.com/budai4medtech/midl2023

<div id="sec-hp" style="margin-top: 0px; font-size: 10%;">

<img
src="figures/fetal-ultrasound-image-synthesis/github-repository.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

M. Iskandar et al. “Towards Realistic Ultrasound Fetal Brain Imaging
Synthesis” in MIDL2023. https://github.com/budai4medtech/midl2023

</div>

## Fetal US imaging with Diffusion models

<div id="sec-hp" style="margin-top: 0px; font-size: 50%;">

<img
src="figures/fetal-ultrasound-image-synthesis/diffusion-based-generative-model.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

1)  Ho et al. 2020 ”Denoising Diffusion Probabilistic Models”
    https://arxiv.org/abs/2006.11239
2)  Fiorentino et al. 2022 ”A Review on Deep Learning Algorithms for
    Fetal Ultrasound-Image Analysis” https://arxiv.org/abs/2201.12260

</div>

## xfetus :baby: :brain: :robot:

A library for ultrasound fetal imaging synthesis using:

- GANs,  
- transformers, and  
- diffusion models.

<div style="font-size: 50%;">

<https://github.com/budai4medtech/xfetus>

</div>

<div class="notes">

TODO: \* Resolve PRs https://github.com/budai4medtech/xfetus/pulls \*
Show emojis in the main README

</div>

## Open-Source Software for Surgical Technologies

## Scripts  [`code.py`]()

<div class="panel-tabset">

### Tab A

Content for `Tab A`

### Tab B

Content for `Tab B`

</div>

## :hospital: Case A

## :hospital: Case B

## :wrench: Hackathon

## :recycle: Model verification

1.  AI
2.  Code
3.  …

## :school_satchel: Education

- A
- B

## :medical_symbol: Template for figures

<div id="sec-hp" style="margin-top: 0px; font-size: 50%;">

<img src="figures/00_template-vector-images/drawing-v00.svg"
style="width:100.0%" data-fig-align="center" />

</div>

## Key takeaways
