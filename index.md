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
- Software as a Medical Device (SaMD)
- Uses cases
  - [Fetal Ultrasound Image Synthesis](#sec-fus)
  - Real-time AI diagnosis
    - Endoscopy-based video
    - Eye movement disorders
- Takeaways

## My trajectory

<div id="sec-mt" style="margin-top: 0px; font-size: 50%;">

<img src="figures/mx.svg" style="width:100.0%"
data-fig-align="center" />

</div>

# Software as a Medical Device (SaMD)

## Regulation vs innovation in MedTech

<div style="margin-top: 0px; font-size: 50%;">

<img
src="figures/regulation-innovation/balance-between-regulation-innovation.svg"
style="width:100.0%" data-fig-align="center" />

</div>

## IEC 62304 standard for software

<div style="margin-top: 0px; font-size: 50%;">

<img src="figures/regulation-innovation/iec62304.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

https://www.iso.org/standard/38421.html

</div>

## Good ML practices by FDA

<div style="margin-top: 0px; font-size: 50%;">

<img src="figures/regulation-innovation/goodALMLFDA.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

US-FDA-Artificial-Intelligence-and-Machine-Learning-Discussion-Paper

</div>

<div class="notes">

Regulatory Framework for Modifications to (AI/ML)-Based Software as a
Medical Device (SaMD)

</div>

## FDA-approved AI-based Medical Devices

<div style="margin-top: 0px; font-size: 50%;">

<img
src="figures/regulation-innovation/fda-approved-ai-based-med-devs.svg"
style="width:100.0%" data-fig-align="center" />

</div>

<div style="font-size: 40%;">

Benjamens, S., Dhunnoo, P. and Meskó, B. The state of artificial
intelligence-based FDA-approved medical devices and algorithms: an
online database. npj Digit. Med. 3, 118 (2020).

</div>

# Fetal Ultrasound Image Synthesis

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

# Developing real-time AI applications for diagnosis

## Real-time AI Applications for Surgery

<div id="fig-template">

<div style="margin-top: 0px; font-size: 80%;">

<img src="figures/holoscan-platform/rtai4spipeline.svg"
style="width:100.0%" data-fig-align="center" />

</div>

Figure 1: Development and deployment pipeline for real-time AI apps for
surgery

</div>

<div class="notes">

Pipeline with development and deployment of real-time AI apps for
surgery

{fig-align=center} {fig-pos=‘b’} b(bottom) h(here) p(page) t(top)

</div>

## NVIDIA Holoscan platform

<div class="columns">

<div class="column" width="50%">

Holoscan-SDK

![](figures/holoscan-platform/holohub.svg)

[
`holoscan-sdk`](https://github.com/nvidia-holoscan/holoscan-sdk/tree/main)

[ `holohub`](https://github.com/nvidia-holoscan/holohub)

</div>

<div class="column" width="50%">

Clara-AGX

![](figures/holoscan-platform/clara_agx_dev_kit_components.svg)

[
`Clara-AGX DevKit`](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/clara-agx/clara_agx_user_guide.md)

[
`Orin-IGX DevKit`](https://github.com/nvidia-holoscan/holoscan-docs/blob/main/devkits/nvidia-igx-orin/nvidia_igx_orin_user_guide.md)

</div>

</div>

<div class="notes">

Holoscan platform

</div>

## Holoscan Core Concepts

<div id="fig-template">

<img src="figures/holoscan-platform/holoscan_core_concepts.svg"
data-fig-align="center" />


Figure 2: Operator: An operator is the most basic unit of work in this
framework.

</div>

<div class="notes">

https://docs.nvidia.com/holoscan/sdk-user-guide/holoscan_operators_extensions.html

</div>

## Bring Your Own Model (BYOM)

<div class="panel-tabset">

### Workflow

<div id="fig-template">

<img src="figures/holoscan-platform/byom.svg" data-fig-align="center" />


Figure 3: Connecting Operators

</div>

### Python

``` python
import os
from argparse import ArgumentParser

from holoscan.core import Application

from holoscan.operators import (
    FormatConverterOp,
    HolovizOp,
    InferenceOp,
    SegmentationPostprocessorOp,
    VideoStreamReplayerOp,
)
from holoscan.resources import UnboundedAllocator


class BYOMApp(Application):
    def __init__(self, data):
        """Initialize the application

Parameters
----------
data : Location to the data
"""

        super().__init__()

        # set name
        self.name = "BYOM App"

        if data == "none":
            data = os.environ.get("HOLOSCAN_INPUT_PATH", "../data")

        self.sample_data_path = data

        self.model_path = os.path.join(os.path.dirname(__file__), "../model")
        self.model_path_map = {
            "byom_model": os.path.join(self.model_path, "identity_model.onnx"),
        }

        self.video_dir = os.path.join(self.sample_data_path, "racerx")
        if not os.path.exists(self.video_dir):
            raise ValueError(f"Could not find video data:{self.video_dir=}")

# Define the workflow
        self.add_flow(source, viz, {("output", "receivers")})
        self.add_flow(source, preprocessor, {("output", "source_video")})
        self.add_flow(preprocessor, inference, {("tensor", "receivers")})
        self.add_flow(inference, postprocessor, {("transmitter", "in_tensor")})
        self.add_flow(postprocessor, viz, {("out_tensor", "receivers")})


def main(config_file, data):
    app = BYOMApp(data=data)
    # if the --config command line argument was provided, it will override this config_file
    app.config(config_file)
    app.run()


if __name__ == "__main__":
    # Parse args
    parser = ArgumentParser(description="BYOM demo application.")
    parser.add_argument(
        "-d",
        "--data",
        default="none",
        help=("Set the data path"),
    )

    args = parser.parse_args()
    config_file = os.path.join(os.path.dirname(__file__), "byom.yaml")
    main(config_file=config_file, data=args.data)
```

### YAML

``` python
%YAML 1.2
replayer:  # VideoStreamReplayer
  basename: "racerx"
  frame_rate: 0 # as specified in timestamps
  repeat: true # default: false
  realtime: true # default: true
  count: 0 # default: 0 (no frame count restriction)

preprocessor:  # FormatConverter
  out_tensor_name: source_video
  out_dtype: "float32"
  resize_width: 512
  resize_height: 512

inference:  # Inference
  backend: "trt"
  pre_processor_map:
    "byom_model": ["source_video"]
  inference_map:
    "byom_model": ["output"]

postprocessor:  # SegmentationPostprocessor
  in_tensor_name: output
  # network_output_type: None
  data_format: nchw

viz:  # Holoviz
  width: 854
  height: 480
  color_lut: [
    [0.65, 0.81, 0.89, 0.1],
    ]
```

</div>

<div class="notes">

Speaker notes go here.

</div>

# Use cases: Real-time AI diagnosis for endoscopic pituitary surgery

## :medical_symbol: Endoscopic Pituitary Surgery

<https://www.youtube.com/embed/EwlRdxokdGk>

<div class="notes">

94,961 views 20 Nov 2012 Barrow Neurological Institute Neurosurgeon
Andrew S. Little, MD, demonstrates the process of removing a tumor of
the pituitary gland using minimally-invasive endoscopic neurosurgery.
https://www.youtube.com/watch?app=desktop&v=EwlRdxokdGk

553,519 views 28 May 2017 The pituitary gland is located at the bottom
of your brain and above the inside of your nose. Endoscopic pituitary
surgery (also called transsphenoidal endoscopic surgery) is a minimally
invasive surgery performed through the nose and sphenoid sinus to remove
pituitary tumors. https://www.youtube.com/watch?v=lwmgNLwt_ts

Mao, Zhehua, Adrito Das, Mobarakol Islam, Danyal Z. Khan, Simon C.
Williams, John G. Hanrahan, Anouk Borg et al. “PitSurgRT: real-time
localization of critical anatomical structures in endoscopic pituitary
surgery.” International Journal of Computer Assisted Radiology and
Surgery (2024): 1-8.

</div>

##  `real-time-ai-for-surgery`

### Getting started docs

<div id="fig-template">

<img src="figures/real-time-ai-for-surgery/getting-started.svg"
data-fig-align="center" />


Figure 4: Getting started documentation provide with a range of links to
setup, use, run and debug application including github workflow.

</div>

<div class="notes">

Speaker notes go here.

</div>

##  `real-time-ai-for-surgery`

### 🏥 Endoscopic pituitary surgery

<div class="panel-tabset">

### 👃 Multi-head Model

<img src="figures/real-time-ai-for-surgery/eps-mhm.svg"
data-fig-align="center" />

### 🌓 PhaseNet Model

<img src="figures/real-time-ai-for-surgery/eps-pnm.svg"
data-fig-align="center" />

</div>

<div class="notes">

Speaker notes go here.

</div>

##  `real-time-ai-for-surgery`

### 🏥 Endoscopic pituitary surgery

<div class="panel-tabset">

### 🔱 Multi AI models (python)

<div class="code-with-filename">

**multi-ai.py**

``` python

...

        # Define the workflow
        if is_v4l2:
            self.add_flow(source, viz, {("signal", "receivers")})
            self.add_flow(source, preprocessor_v4l2, {("signal", "source_video")})
            self.add_flow(source, preprocessor_phasenet_v4l2, {("signal", "source_video")})
            for op in [preprocessor_v4l2, preprocessor_phasenet_v4l2]:
                self.add_flow(op, multi_ai_inference_v4l2, {("", "receivers")})
            ### connect infereceOp to postprocessors
            self.add_flow(
                multi_ai_inference_v4l2, multiheadOp, {("transmitter", "in_tensor_postproOp")}
            )
            self.add_flow(multi_ai_inference_v4l2, segpostprocessor, {("transmitter", "")})
            self.add_flow(multi_ai_inference_v4l2, phasenetOp, {("", "in")})

        else:
            self.add_flow(source, viz, {("", "receivers")})
            self.add_flow(source, preprocessor_replayer, {("output", "source_video")})
            self.add_flow(source, preprocessor_phasenet_replayer, {("output", "source_video")})
            for op in [preprocessor_replayer, preprocessor_phasenet_replayer]:
                self.add_flow(op, multi_ai_inference_replayer, {("", "receivers")})
            ### connect infereceOp to postprocessors
            self.add_flow(
                multi_ai_inference_replayer, multiheadOp, {("transmitter", "in_tensor_postproOp")}
            )
            self.add_flow(multi_ai_inference_replayer, segpostprocessor, {("transmitter", "")})
            self.add_flow(multi_ai_inference_replayer, phasenetOp, {("", "in")})

        ## connect postprocessors outputs for visualisation with holoviz
        self.add_flow(multiheadOp, viz, {("out_tensor_postproOp", "receivers")})
        self.add_flow(segpostprocessor, viz, {("", "receivers")})
        self.add_flow(phasenetOp, viz, {("out", "receivers")})
        self.add_flow(phasenetOp, viz, {("output_specs", "input_specs")})

...
```

</div>

### 🔱 Multi AI models (YAML)

<div class="code-with-filename">

**multi-ai.yaml**

``` python

...

 multi_ai_inference_v4l2:
  #
  #
  # Multi-AI Inference Operator InferenceOp()
  #
  #
  backend: "trt"
  pre_processor_map:
    "pit_surg_model": ["prepro_v4l2"]
    "phasenet_model": ["prepro_PNv4l2"]
  inference_map:
    "pit_surg_model": ["segmentation_masks", "landmarks"]
    "phasenet_model": ["out"]
  enable_fp16: False
  parallel_inference: true # optional param, default to true
  infer_on_cpu: false # optional param, default to false
  input_on_cuda: true # optional param, default to true
  output_on_cuda: true # optional param, default to true
  transmit_on_cuda: true # optional param, default to true
  is_engine_path: false # optional param, default to false

multi_ai_inference_replayer:
  #
  #
  # Multi-AI Inference Operator InferenceOp()
  #
  #
  backend: "trt"
  pre_processor_map:
    "pit_surg_model": ["prepro_replayer"]
    "phasenet_model": ["prepro_PNreplayer"]
  inference_map:
    "pit_surg_model": ["segmentation_masks", "landmarks"]
    "phasenet_model": ["out"]
  enable_fp16: False
  parallel_inference: true # optional param, default to true
  infer_on_cpu: false # optional param, default to false
  input_on_cuda: true # optional param, default to true
  output_on_cuda: true # optional param, default to true
  transmit_on_cuda: true # optional param, default to true
  is_engine_path: false # optional param, default to false

...
```

</div>

</div>

<div class="notes">

Speaker notes go here.

<img src="figures/00_template-vector-images/drawing-v00.svg"
data-fig-align="center" /> \`\`\`{.python
filename=“unit-test-example.py” code-line-numbers=“\|30-36”}

</div>

##  `real-time-ai-for-surgery`

### 🤝 Contributing

<div id="fig-template">

<img src="figures/real-time-ai-for-surgery/contributing.svg"
data-fig-align="center" />


Figure 5: real-time-ai-for-surgery follows the Contributor Covenant Code
of Conduct. Contributions, issues and feature requests are welcome.

</div>

<div class="notes">

Speaker notes go here.

</div>

##  `real-time-ai-for-surgery`

### GitHub templates

<div class="panel-tabset">

### 🎒 new users

<img src="figures/real-time-ai-for-surgery/gh_templates_new_users.svg"
data-fig-align="center" />

### 🔩 new models

<img src="figures/real-time-ai-for-surgery/gh_templates_new_models.svg"
data-fig-align="center" />

### :recycle: PRs

<img src="figures/real-time-ai-for-surgery/gh_templates_PRs.svg"
data-fig-align="center" />

</div>

<div class="notes">

Speaker notes go here. {.scrollable}

</div>

##  `real-time-ai-for-surgery`

### Release version summaries

<div class="panel-tabset">

### v0.1.0

<img src="figures/real-time-ai-for-surgery/v0.1.0-rtai4s.svg"
data-fig-align="center" />

### v0.2.0

<img src="figures/real-time-ai-for-surgery/v0.2.0-rtai4s.svg"
data-fig-align="center" />

### v0.3.0

<img src="figures/real-time-ai-for-surgery/v0.3.0-rtai4s.svg"
data-fig-align="center" />

### v0.4.0

<img src="figures/real-time-ai-for-surgery/v0.4.0-rtai4s.svg"
data-fig-align="center" />

### v0.5.0

<img src="figures/real-time-ai-for-surgery/v0.5.0-rtai4s.svg"
data-fig-align="center" />

</div>

<div class="notes">

Speaker notes go here. {.scrollable}

</div>

# Use cases: Real-time AI diagnosis for eye movement disorders

## :robot: :eyes: AI in ophthalmic imaging modalities

<div id="fig-template">

<img src="figures/ophthalmology/li2023-fig2.jpg"
data-fig-align="center" />


Figure 6: Practical application of AI in all common ophthalmic imaging
modalities

</div>

<div style="font-size: 40%;">

Li, Zhongwen, Lei Wang, Xuefang Wu, Jiewei Jiang, Wei Qiang, He Xie,
Hongjian Zhou, Shanjun Wu, Yi Shao, and Wei Chen. “Artificial
intelligence in ophthalmology: The path to the real-world clinic.” Cell
Reports Medicine 4, no. 7 (2023).

</div>

<div class="notes">

Nystagmus {.scrollable}

</div>

## :robot: :eyes: Eye movement disorders

<div class="columns">

<div class="column" width="50%">

- Nystagmus is an eye movement disorder characterized by involunatry eye
  oscillations.​
- Pathologic nystagmus is estimated to be 24 per 10,000 with a slight
  predilection toward European ancestry \[1\]​.

</div>

<div class="column" width="50%">

![](figures/ophthalmology/nystagmus.gif)

</div>

</div>

<div style="font-size: 40%;">

\[1\] Sarvananthan, Nagini, Mylvaganam Surendran, Eryl O. Roberts,
Sunila Jain, Shery Thomas, Nitant Shah, Frank A. Proudlock et al. “The
prevalence of nystagmus: the Leicestershire nystagmus survey.”
Investigative ophthalmology & visual science 50, no. 11 (2009):
5201-5206.​

</div>

<div class="notes">

Nystagmus {.scrollable}

</div>

## :robot: :eyes: Real-time AI Diagnosis for Nystagmus

<img src="figures/nystagmus/animation-2024-09-13%2016-45.gif"
data-fig-align="center" />

<div class="notes">

Demo {.scrollable}

</div>

## :robot: :eyes: Real-time AI Diagnosis for Nystagmus

Future work

<div class="columns">

<div class="column" width="50%">

- Real-time AI guidance for high-quality images (Liu et al. 2023)
  <img src="figures/ophthalmology/liu_2023_graphical_abstract.jpg"
  style="width:50.0%" data-fig-align="center" />

</div>

<div class="column" width="50%">

- Implement UNET-Visual Transformer models (Yao et al. 2022)  
  <img src="figures/ophthalmology/yao2022_fig1.png" style="width:80.0%"
  data-fig-align="center" />

</div>

</div>

<div style="font-size: 40%;">

Liu, L., Wu, X., Lin, D., Zhao, L., Li, M., Yun, D., Lin, Z., Pang, J.,
Li, L., Wu, Y. and Lai, W., 2023. DeepFundus: a flow-cytometry-like
image quality classifier for boosting the whole life cycle of medical
artificial intelligence. Cell Reports Medicine, 4(2).

Yao, Chang, Menghan Hu, Qingli Li, Guangtao Zhai, and Xiao-Ping Zhang.
“Transclaw u-net: claw u-net with transformers for medical image
segmentation.” In 2022 5th International Conference on Information
Communication and Signal Processing (ICICSP), pp. 280-284. IEEE, 2022.

</div>

<div class="notes">

Plans {.scrollable}

</div>

# Open-Source Software for Surgical Technologies

## 

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

- A5\* B

# Key takeaways

- Implement UNET-Visual Transformer models (Yao et al. 2022) \## :medi\*
  A5\* B cal_symbol: Template for figures

<div id="sec-hp" style="margin-top: 0px; font-size: 50%;">

<img src="figures/00_template-vector-images/drawing-v00.svg"
style="width:100.0%" data-fig-align="center" />

</div>

## 🙌 Acknowledgements

- Diego Kaski

Yao, Chang, Menghan Hu, Qingli Li, Guangtao Zhai, and Xiao-Ping Zhang.
“Transclaw u-net: claw u-net with transformers for medical image
segmentation.” In 2022 5th International Conference on Information
Communication and Signal Processing (ICICSP), pp. 280-284. IEEE, 2022.
\* UCL Queen Square Institute of Neurology \* Zhehua Mao, Sophia Bano
and Matt Clarkson \* Wellcome / EPSRC Centre for Interventional and
Surgical Sciences (WEISS) \* Steve Thompson \* Advanced Research
Computing Centre (ARC) \* Mikael Brudfors and Nadim Daher \* NVIDIA
Healthcare AI