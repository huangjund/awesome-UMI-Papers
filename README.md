# Awesome Universal Manipulation Interface [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Representative papers, datasets, code, and hardware for Universal Manipulation Interface (UMI) and UMI-style robot-free manipulation demonstrations.

This list focuses on systems that turn in-the-wild human demonstrations into robot-ready supervision. It is seeded from Jingru Zhang's UMI survey notes and public resources available through 2026-04-20.

To contribute, open a pull request with one link, one short sentence on why it matters for UMI, and 3-5 tags.

**Tags:** `paper`, `preprint`, `survey`, `code`, `hardware`, `data`, `core-umi`, `interface`, `tracking`, `calibration`, `vision`, `multiview`, `active-perception`, `3d-perception`, `tactile`, `force`, `contact-rich`, `dexterous`, `bimanual`, `mobile`, `cross-embodiment`, `imitation-learning`, `diffusion-policy`, `policy-guidance`, `representation-learning`, `dataset`, `vla`.

## Core and Surveys

- **UMI**, *Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots*, RSS 2024. [[📄 Paper](https://www.roboticsproceedings.org/rss20/p045.html)] [[🌍 Website](https://umi-gripper.github.io/)] [[💻 Code](https://github.com/real-stanford/universal_manipulation_interface)] Tags: `paper` `core-umi` `interface` `vision` `imitation-learning`.
- **UMI Topic Overview**, overview of UMI, FastUMI, exUMI, MV-UMI, DexUMI, ActiveUMI, UMI-on-Legs, and UMI-on-Air. [[🧭 Overview](https://www.emergentmind.com/topics/universal-manipulation-interface-umi)] Tags: `survey` `core-umi` `interface` `cross-embodiment`.
- **Diffusion Manipulation Survey**, *Diffusion Models for Robotic Manipulation: A Survey*, 2025.04. [[📄 Paper](https://arxiv.org/abs/2504.08438)] Tags: `survey` `diffusion-policy` `imitation-learning` `policy-guidance`.

## Interfaces, Tracking, and Perception

- **FastUMI**, *A Scalable and Hardware-Independent Universal Manipulation Interface with Dataset*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/zhaxizhuoma25a.html)] [[🌍 Website](https://fastumi.com/FastUMI/)] [[📄 arXiv](https://arxiv.org/abs/2409.19499)] Tags: `paper` `interface` `hardware` `tracking` `dataset`.
- **Actuated UMI Gripper**, open-source motorized UMI-compatible gripper. [[🌍 Website](https://actuated-umi.github.io/)] [[💻 Code](https://github.com/actuated-umi/actuated-umi-gripper)] Tags: `hardware` `interface` `force` `code`.
- **UMI-3D**, *Extending Universal Manipulation Interface from Vision-Limited to 3D Spatial Perception*, 2026.04. [[📄 Paper](https://arxiv.org/abs/2604.14089)] [[🌍 Website](https://umi-3d.github.io/)] Tags: `preprint` `3d-perception` `tracking` `calibration` `vision`.
- **ORB-SLAM3 UMI Fork**, SLAM backend used by the original UMI codebase and tutorials. [[💻 Code](https://github.com/cheng-chi/ORB_SLAM3)] Tags: `code` `tracking` `calibration` `core-umi`.
- **MV-UMI**, *A Scalable Multi-View Interface for Cross-Embodiment Learning*, 2025.09. [[📄 Paper](https://arxiv.org/abs/2509.18757)] [[🌍 Website](https://mv-umi.github.io/)] Tags: `preprint` `multiview` `vision` `cross-embodiment`.
- **ActiveUMI**, *Robotic Manipulation with Active Perception from Robot-Free Human Demonstrations*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.01607)] [[🌍 Website](https://activeumi.github.io/)] Tags: `preprint` `active-perception` `vision` `policy-guidance`.
- **ARCap**, *Collecting High-quality Human Demonstrations for Robot Learning with Augmented Reality Feedback*, ICRA 2025. [[📄 Paper](https://arxiv.org/abs/2410.08464)] [[🌍 Website](https://stanford-tml.github.io/ARCap/)] Tags: `paper` `interface` `cross-embodiment` `imitation-learning` `policy-guidance`.
- **ARMADA**, *Augmented Reality for Robot Manipulation and Robot-Free Data Acquisition*, 2024.12. [[📄 Paper](https://arxiv.org/abs/2412.10631)] [[🌍 Website](https://machinelearning.apple.com/research/armada-augmented-reality)] [[📝 OpenReview](https://openreview.net/forum?id=o7eWqcPfpL)] Tags: `preprint` `interface` `imitation-learning` `cross-embodiment`.

## Tactile, Force, and Dexterity

- **ViTaMIn**, *Learning Contact-Rich Tasks Through Robot-Free Visuo-Tactile Manipulation Interface*, 2025.04. [[📄 Paper](https://arxiv.org/abs/2504.06156)] [[🌍 Website](https://chuanyune.github.io/ViTaMIn_page/)] Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- **Touch in the Wild**, *Learning Fine-Grained Manipulation with a Portable Visuo-Tactile Gripper*, 2025.07. [[📄 Paper](https://arxiv.org/abs/2507.15062)] [[🌍 Website](https://touchinthewild.github.io/)] [[📝 OpenReview](https://openreview.net/forum?id=WabVVQKTUF)] Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- **FreeTacMan**, *Robot-free Visuo-Tactile Data Collection System for Contact-rich Manipulation*, 2025.06. [[📄 Paper](https://arxiv.org/abs/2506.01941)] [[🌍 Website](https://freetacmanblog.github.io/)] Tags: `preprint` `tactile` `contact-rich` `dataset` `interface`.
- **exUMI**, *Extensible Robot Teaching System with Action-aware Task-agnostic Tactile Representation*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/xu25e.html)] [[🌍 Website](https://silicx.github.io/exUMI/)] [[📝 OpenReview](https://openreview.net/forum?id=b86nyIOJWq)] Tags: `paper` `tactile` `tracking` `calibration` `representation-learning`.
- **FARM**, *Tactile-Conditioned Diffusion Policy for Force-Aware Robotic Manipulation*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.13324)] [[🌍 Website](https://tactile-farm.github.io/)] Tags: `preprint` `tactile` `force` `diffusion-policy` `contact-rich`.
- **OmniUMI**, *Towards Physically Grounded Robot Learning via Human-Aligned Multimodal Interaction*, 2026.04. [[📄 Paper](https://arxiv.org/abs/2604.10647)] Tags: `preprint` `tactile` `force` `contact-rich` `diffusion-policy`.
- **ViTaMIn-B**, *A Reliable and Efficient Visuo-Tactile Bimanual Manipulation Interface*, 2025.11. [[📄 Paper](https://arxiv.org/abs/2511.05858)] Tags: `preprint` `bimanual` `tactile` `tracking` `contact-rich`.
- **UMI-FT**, *In-the-Wild Compliant Manipulation with UMI-FT*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.09988)] [[🌍 Website](https://umi-ft.github.io/)] Tags: `preprint` `force` `contact-rich` `policy-guidance`.
- **TacUMI**, *A Multi-Modal Universal Manipulation Interface for Contact-Rich Tasks*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.14550)] Tags: `preprint` `tactile` `force` `contact-rich` `policy-guidance`.
- **DexUMI**, *Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/xu25b.html)] [[🌍 Website](https://dex-umi.github.io/)] [[📄 arXiv](https://arxiv.org/abs/2505.21864)] Tags: `paper` `dexterous` `tactile` `cross-embodiment` `interface`.
- **DexCap**, *Scalable and Portable Mocap Data Collection System for Dexterous Manipulation*, RSS 2024. [[📄 Paper](https://arxiv.org/abs/2403.07788)] [[🌍 Website](https://dex-cap.github.io/)] Tags: `paper` `dexterous` `tracking` `interface` `imitation-learning`.
- **Holo-Dex**, *Teaching Dexterity with Immersive Mixed Reality*, ICRA 2023. [[📄 Paper](https://arxiv.org/abs/2210.06463)] [[🌍 Website](https://holo-dex.github.io/)] Tags: `paper` `dexterous` `interface` `imitation-learning` `dataset`.
- **DIME**, *Dexterous Imitation Made Easy: A Learning-Based Framework for Efficient Dexterous Manipulation*, ICRA 2023. [[📄 Paper](https://arxiv.org/abs/2203.13251)] [[🌍 Website](https://nyu-robot-learning.github.io/dime/)] [[💻 Code](https://github.com/NYU-robot-learning/DIME-Models)] Tags: `paper` `dexterous` `interface` `imitation-learning` `code`.

## Cross-Embodiment Deployment

- **UMI-on-Legs**, *Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers*, CoRL 2024. [[📄 Paper](https://proceedings.mlr.press/v270/ha25a.html)] [[🌍 Website](https://umi-on-legs.github.io/)] [[💻 Code](https://github.com/real-stanford/umi-on-legs)] Tags: `paper` `mobile` `cross-embodiment` `policy-guidance`.
- **UMI-on-Air**, *Embodiment-Aware Guidance for Embodiment-Agnostic Visuomotor Policies*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.02614)] [[🌍 Website](https://umi-on-air.github.io/)] [[📦 Checkpoints](https://huggingface.co/LeCAR-Lab/umi-on-air_checkpoints)] Tags: `preprint` `mobile` `cross-embodiment` `diffusion-policy` `policy-guidance`.
- **HoMMI**, *Learning Whole-Body Mobile Manipulation from Human Demonstrations*, 2026.03. [[📄 Paper](https://arxiv.org/abs/2603.03243)] [[🌍 Website](https://hommi-robot.github.io/)] Tags: `preprint` `mobile` `active-perception` `cross-embodiment` `policy-guidance`.
- **HuMI**, *Humanoid Manipulation Interface: Humanoid Whole-Body Manipulation from Robot-Free Demonstrations*, 2026.02. [[📄 Paper](https://arxiv.org/abs/2602.06643)] [[🌍 Website](https://humanoid-manipulation-interface.github.io/)] [[🗂️ Data](https://huggingface.co/datasets/Richard-Nai/HuMI-Raw-Data)] Tags: `preprint` `mobile` `bimanual` `cross-embodiment` `imitation-learning`.

## Policy Learning

- **Diffusion Policy**, *Visuomotor Policy Learning via Action Diffusion*, RSS 2023. [[📄 Paper](https://arxiv.org/abs/2303.04137)] [[🌍 Website](https://diffusion-policy.cs.columbia.edu/)] [[💻 Code](https://github.com/real-stanford/diffusion_policy)] Tags: `paper` `diffusion-policy` `imitation-learning` `code`.
- **ALOHA / ACT**, *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware*, 2023.04. [[📄 Paper](https://arxiv.org/abs/2304.13705)] [[🌍 Website](https://tonyzhaozh.github.io/aloha/)] [[💻 Code](https://github.com/tonyzhaozh/aloha)] Tags: `paper` `bimanual` `hardware` `imitation-learning` `code`.
- **pi0**, *A Vision-Language-Action Flow Model for General Robot Control*, 2024.10. [[📄 Paper](https://arxiv.org/abs/2410.24164)] [[🌍 Website](https://www.physicalintelligence.company/blog/pi0)] Tags: `paper` `vla` `cross-embodiment` `imitation-learning`.
- **RDT2**, *Exploring the Scaling Limit of UMI Data Towards Zero-Shot Cross-Embodiment Generalization*, 2026.02. [[📄 Paper](https://arxiv.org/abs/2602.03310)] [[🌍 Website](https://rdt-robotics.github.io/rdt2/)] [[🤗 Model](https://huggingface.co/robotics-diffusion-transformer/RDT2-FM)] Tags: `preprint` `vla` `dataset` `cross-embodiment` `imitation-learning`.
- **TouchGuide**, *Inference-Time Steering of Visuomotor Policies via Touch Guidance*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.20239)] [[🌍 Website](https://martelzhang.github.io/touchguide/)] Tags: `preprint` `tactile` `diffusion-policy` `policy-guidance`.

## Datasets and Benchmarks

- **UMI Robot Dataset Community**, community index for UMI-style robot datasets. [[🌍 Website](https://umi-data.github.io/)] Tags: `data` `dataset` `core-umi`.
- **FastUMI-100K**, *Advancing Data-driven Robotic Manipulation with a Large-scale UMI-style Dataset*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.08022)] [[🗂️ Data](https://github.com/MrKeee/FastUMI-100K)] Tags: `preprint` `data` `dataset` `multiview` `vla`.
- **UniDex**, *A Robot Foundation Suite for Universal Dexterous Hand Control from Egocentric Human Videos*, 2026.03. [[📄 Paper](https://arxiv.org/abs/2603.22264)] [[🌍 Website](https://unidex-ai.github.io/)] [[🤗 Model](https://huggingface.co/UniDex-ai/UniDex)] Tags: `preprint` `dexterous` `vla` `dataset` `cross-embodiment`.
- **RoboPaint**, *From Human Demonstration to Any Robot and Any View*, 2026.02. [[📄 Paper](https://arxiv.org/abs/2602.05325)] Tags: `preprint` `dexterous` `tactile` `dataset` `vla`.
- **Open X-Embodiment**, large cross-embodiment robot dataset and benchmark. [[🌍 Website](https://robotics-transformer-x.github.io/)] Tags: `data` `dataset` `cross-embodiment` `vla`.
- **DROID**, *A Large-Scale In-The-Wild Robot Manipulation Dataset*. [[🌍 Website](https://droid-dataset.github.io/)] Tags: `data` `dataset` `interface` `imitation-learning`.
- **BridgeData V2**, large real-world robot manipulation dataset. [[🌍 Website](https://rail-berkeley.github.io/bridgedata/)] Tags: `data` `dataset` `imitation-learning`.

## Related Resources

- **GELLO**, *A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators*. [[🌍 Website](https://wuphilipp.github.io/gello_site/)] Tags: `hardware` `interface` `imitation-learning`.
- **MimicPlay**, *Long-Horizon Imitation Learning by Watching Human Play*. [[🌍 Website](https://mimic-play.github.io/)] Tags: `paper` `imitation-learning` `policy-guidance`.
- **WHIRL**, *Human-to-Robot Imitation in the Wild*, RSS 2022. [[📄 Paper](https://arxiv.org/abs/2207.09450)] [[🌍 Website](https://human2robot.github.io/)] Tags: `paper` `vision` `imitation-learning` `policy-guidance`.
