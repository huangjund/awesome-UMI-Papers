# Awesome Universal Manipulation Interface [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Representative papers, datasets, code, and hardware for Universal Manipulation Interface (UMI) and UMI-style robot-free manipulation demonstrations.

This list focuses on systems that turn in-the-wild human demonstrations into robot-ready supervision.

To contribute, open a pull request with one link, one short sentence on why it matters for UMI, and 3-5 tags.

**Tags:** `paper`, `preprint`, `survey`, `code`, `hardware`, `data`, `core-umi`, `interface`, `tracking`, `calibration`, `vision`, `multiview`, `active-perception`, `3d-perception`, `tactile`, `force`, `contact-rich`, `dexterous`, `bimanual`, `mobile`, `cross-embodiment`, `imitation-learning`, `diffusion-policy`, `policy-guidance`, `representation-learning`, `dataset`, `vla`.

## Challenge
- **Maniskill ViTac Challenge 2026**, [[🌍 Website](https://callmeray.github.io/Mani_ViTac_Challenge_2026_page/)] Tags:`data` `core-umi` `tactile` `force` `dataset`.

## Core and Surveys

- **Diffusion Manipulation Survey**, *Diffusion Models for Robotic Manipulation: A Survey*, 2025.04. [[📄 Paper](https://arxiv.org/abs/2504.08438)] Tags: `survey` `diffusion-policy` `imitation-learning` `policy-guidance`.
- **UMI**, *Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots*, RSS 2024. [[📄 Paper](https://www.roboticsproceedings.org/rss20/p045.html)] [[🌍 Website](https://umi-gripper.github.io/)] [[💻 Code](https://github.com/real-stanford/universal_manipulation_interface)] Tags: `paper` `core-umi` `interface` `vision` `imitation-learning`.
- **UMI Topic Overview**, overview of UMI, FastUMI, exUMI, MV-UMI, DexUMI, ActiveUMI, UMI-on-Legs, and UMI-on-Air. [[🧭 Overview](https://www.emergentmind.com/topics/universal-manipulation-interface-umi)] Tags: `survey` `core-umi` `interface` `cross-embodiment`.

## Interfaces, Tracking, and Perception

- **UMI-3D**, *Extending Universal Manipulation Interface from Vision-Limited to 3D Spatial Perception*, 2026.04. [[📄 Paper](https://arxiv.org/abs/2604.14089)] [[🌍 Website](https://umi-3d.github.io/)] Tags: `preprint` `3d-perception` `tracking` `calibration` `vision`.
- **UMIGen**, *A Unified Framework for Egocentric Point Cloud Generation and Cross-Embodiment Robotic Imitation Learning*, 2025.11. [[📄 Paper](https://arxiv.org/abs/2511.09302)] Tags: `preprint` `3d-perception` `cross-embodiment` `imitation-learning` `tracking`.
- **ActiveUMI**, *Robotic Manipulation with Active Perception from Robot-Free Human Demonstrations*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.01607)] [[🌍 Website](https://activeumi.github.io/)] Tags: `preprint` `active-perception` `vision` `policy-guidance`.
- **MV-UMI**, *A Scalable Multi-View Interface for Cross-Embodiment Learning*, 2025.09. [[📄 Paper](https://arxiv.org/abs/2509.18757)] [[🌍 Website](https://mv-umi.github.io/)] Tags: `preprint` `multiview` `vision` `cross-embodiment`.
- **FastUMI**, *A Scalable and Hardware-Independent Universal Manipulation Interface with Dataset*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/zhaxizhuoma25a.html)] [[🌍 Website](https://fastumi.com/FastUMI/)] [[📄 arXiv](https://arxiv.org/abs/2409.19499)] Tags: `paper` `interface` `hardware` `tracking` `dataset`.
- **Agricultural UMI Hardware**, *Advances on Affordable Hardware Platforms for Human Demonstration Acquisition in Agricultural Applications*, ERF 2025. [[📄 Paper](https://arxiv.org/abs/2506.09494)] [[📦 Record](https://zenodo.org/records/15111126)] Tags: `paper` `hardware` `tracking` `interface` `imitation-learning`.
- **Actuated UMI Gripper**, open-source motorized UMI-compatible gripper. [[🌍 Website](https://actuated-umi.github.io/)] [[💻 Code](https://github.com/actuated-umi/actuated-umi-gripper)] Tags: `hardware` `interface` `force` `code`.
- **ORB-SLAM3 UMI Fork**, SLAM backend used by the original UMI codebase and tutorials. [[💻 Code](https://github.com/cheng-chi/ORB_SLAM3)] Tags: `code` `tracking` `calibration` `core-umi`.

## Tactile, Force, and Dexterity

- **OmniUMI**, *Towards Physically Grounded Robot Learning via Human-Aligned Multimodal Interaction*, 2026.04. [[📄 Paper](https://arxiv.org/abs/2604.10647)] Tags: `preprint` `tactile` `force` `contact-rich` `diffusion-policy`.
- **TacUMI**, *A Multi-Modal Universal Manipulation Interface for Contact-Rich Tasks*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.14550)] Tags: `preprint` `tactile` `force` `contact-rich` `policy-guidance`.
- **UMI-FT**, *In-the-Wild Compliant Manipulation with UMI-FT*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.09988)] [[🌍 Website](https://umi-ft.github.io/)] Tags: `preprint` `force` `contact-rich` `policy-guidance`.
- **TacThru-UMI**, *Simultaneous Tactile-Visual Perception for Learning Multimodal Robot Manipulation*, RA-L 2026. [[📄 Paper](https://arxiv.org/abs/2512.09851)] [[🌍 Website](https://tacthru.yuyang.li/)] [[💻 Code](https://github.com/YuyangLee/TacThru)] [[🗂️ Data](https://huggingface.co/datasets/aidenli/tacthru_umi_tasks)] Tags: `paper` `tactile` `vision` `diffusion-policy` `dataset`.
- **ViTaMIn-B**, *A Reliable and Efficient Visuo-Tactile Bimanual Manipulation Interface*, 2025.11. [[📄 Paper](https://arxiv.org/abs/2511.05858)] Tags: `preprint` `bimanual` `tactile` `tracking` `contact-rich`.
- **FARM**, *Tactile-Conditioned Diffusion Policy for Force-Aware Robotic Manipulation*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.13324)] [[🌍 Website](https://tactile-farm.github.io/)] Tags: `preprint` `tactile` `force` `diffusion-policy` `contact-rich`.
- **Touch in the Wild**, *Learning Fine-Grained Manipulation with a Portable Visuo-Tactile Gripper*, 2025.07. [[📄 Paper](https://arxiv.org/abs/2507.15062)] [[🌍 Website](https://touchinthewild.github.io/)] [[📝 OpenReview](https://openreview.net/forum?id=WabVVQKTUF)] Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- **FreeTacMan**, *Robot-free Visuo-Tactile Data Collection System for Contact-rich Manipulation*, 2025.06. [[📄 Paper](https://arxiv.org/abs/2506.01941)] [[🌍 Website](https://freetacmanblog.github.io/)] Tags: `preprint` `tactile` `contact-rich` `dataset` `interface`.
- **DexUMI**, *Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/xu25b.html)] [[🌍 Website](https://dex-umi.github.io/)] [[📄 arXiv](https://arxiv.org/abs/2505.21864)] Tags: `paper` `dexterous` `tactile` `cross-embodiment` `interface`.
- **exUMI**, *Extensible Robot Teaching System with Action-aware Task-agnostic Tactile Representation*, CoRL 2025. [[📄 Paper](https://proceedings.mlr.press/v305/xu25e.html)] [[🌍 Website](https://silicx.github.io/exUMI/)] [[📝 OpenReview](https://openreview.net/forum?id=b86nyIOJWq)] Tags: `paper` `tactile` `tracking` `calibration` `representation-learning`.
- **ViTaMIn**, *Learning Contact-Rich Tasks Through Robot-Free Visuo-Tactile Manipulation Interface*, 2025.04. [[📄 Paper](https://arxiv.org/abs/2504.06156)] [[🌍 Website](https://chuanyune.github.io/ViTaMIn_page/)] Tags: `preprint` `tactile` `contact-rich` `representation-learning`.

## Cross-Embodiment Deployment

- **UMI-Underwater**, *Learning Underwater Manipulation without Underwater Teleoperation*, 2026.03. [[📄 Paper](https://arxiv.org/abs/2603.27012)] [[🌍 Website](https://umi-under-water.github.io/)] [[💻 Code](https://github.com/umi-under-water/UMI_underwater)] Tags: `preprint` `3d-perception` `dataset` `diffusion-policy` `policy-guidance`.
- **HoMMI**, *Learning Whole-Body Mobile Manipulation from Human Demonstrations*, 2026.03. [[📄 Paper](https://arxiv.org/abs/2603.03243)] [[🌍 Website](https://hommi-robot.github.io/)] Tags: `preprint` `mobile` `active-perception` `cross-embodiment` `policy-guidance`.
- **HuMI**, *Humanoid Manipulation Interface: Humanoid Whole-Body Manipulation from Robot-Free Demonstrations*, 2026.02. [[📄 Paper](https://arxiv.org/abs/2602.06643)] [[🌍 Website](https://humanoid-manipulation-interface.github.io/)] [[🗂️ Data](https://huggingface.co/datasets/Richard-Nai/HuMI-Raw-Data)] Tags: `preprint` `mobile` `bimanual` `cross-embodiment` `imitation-learning`.
- **UMI-on-Air**, *Embodiment-Aware Guidance for Embodiment-Agnostic Visuomotor Policies*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.02614)] [[🌍 Website](https://umi-on-air.github.io/)] [[📦 Checkpoints](https://huggingface.co/LeCAR-Lab/umi-on-air_checkpoints)] Tags: `preprint` `mobile` `cross-embodiment` `diffusion-policy` `policy-guidance`.
- **UMI-on-Legs**, *Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers*, CoRL 2024. [[📄 Paper](https://proceedings.mlr.press/v270/ha25a.html)] [[🌍 Website](https://umi-on-legs.github.io/)] [[💻 Code](https://github.com/real-stanford/umi-on-legs)] Tags: `paper` `mobile` `cross-embodiment` `policy-guidance`.

## Policy Learning

- **RDT2**, *Exploring the Scaling Limit of UMI Data Towards Zero-Shot Cross-Embodiment Generalization*, 2026.02. [[📄 Paper](https://arxiv.org/abs/2602.03310)] [[🌍 Website](https://rdt-robotics.github.io/rdt2/)] [[🤗 Model](https://huggingface.co/robotics-diffusion-transformer/RDT2-FM)] Tags: `preprint` `vla` `dataset` `cross-embodiment` `imitation-learning`.
- **TouchGuide**, *Inference-Time Steering of Visuomotor Policies via Touch Guidance*, 2026.01. [[📄 Paper](https://arxiv.org/abs/2601.20239)] [[🌍 Website](https://martelzhang.github.io/touchguide/)] Tags: `preprint` `tactile` `diffusion-policy` `policy-guidance`.
- **pi0**, *A Vision-Language-Action Flow Model for General Robot Control*, 2024.10. [[📄 Paper](https://arxiv.org/abs/2410.24164)] [[🌍 Website](https://www.physicalintelligence.company/blog/pi0)] Tags: `paper` `vla` `cross-embodiment` `imitation-learning`.
- **ALOHA / ACT**, *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware*, 2023.04. [[📄 Paper](https://arxiv.org/abs/2304.13705)] [[🌍 Website](https://tonyzhaozh.github.io/aloha/)] [[💻 Code](https://github.com/tonyzhaozh/aloha)] Tags: `paper` `bimanual` `hardware` `imitation-learning` `code`.
- **Diffusion Policy**, *Visuomotor Policy Learning via Action Diffusion*, RSS 2023. [[📄 Paper](https://arxiv.org/abs/2303.04137)] [[🌍 Website](https://diffusion-policy.cs.columbia.edu/)] [[💻 Code](https://github.com/real-stanford/diffusion_policy)] Tags: `paper` `diffusion-policy` `imitation-learning` `code`.

## Datasets and Benchmarks

- **UMI Robot Dataset Community**, community index for UMI-style robot datasets. [[🌍 Website](https://umi-data.github.io/)] Tags: `data` `dataset` `core-umi`.
- **Hoi!**, *A Multimodal Dataset for Force-Grounded, Cross-View Articulated Manipulation*, 2025.12. [[📄 Paper](https://arxiv.org/abs/2512.04884)] [[🌍 Website](https://timengelbracht.github.io/Hoi-Dataset-Website/)] Tags: `preprint` `data` `dataset` `tactile` `force`.
- **FastUMI-100K**, *Advancing Data-driven Robotic Manipulation with a Large-scale UMI-style Dataset*, 2025.10. [[📄 Paper](https://arxiv.org/abs/2510.08022)] [[🗂️ Data](https://github.com/MrKeee/FastUMI-100K)] Tags: `preprint` `data` `dataset` `multiview` `vla`.
- **DROID**, *A Large-Scale In-The-Wild Robot Manipulation Dataset*. [[🌍 Website](https://droid-dataset.github.io/)] Tags: `data` `dataset` `interface` `imitation-learning`.
- **Open X-Embodiment**, large cross-embodiment robot dataset and benchmark. [[🌍 Website](https://robotics-transformer-x.github.io/)] Tags: `data` `dataset` `cross-embodiment` `vla`.
- **BridgeData V2**, large real-world robot manipulation dataset. [[🌍 Website](https://rail-berkeley.github.io/bridgedata/)] Tags: `data` `dataset` `imitation-learning`.

## Related Resources

- **MimicPlay**, *Long-Horizon Imitation Learning by Watching Human Play*. [[🌍 Website](https://mimic-play.github.io/)] Tags: `paper` `imitation-learning` `policy-guidance`.
- **GELLO**, *A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators*. [[🌍 Website](https://wuphilipp.github.io/gello_site/)] Tags: `hardware` `interface` `imitation-learning`.
- **WHIRL**, *Human-to-Robot Imitation in the Wild*, RSS 2022. [[📄 Paper](https://arxiv.org/abs/2207.09450)] [[🌍 Website](https://human2robot.github.io/)] Tags: `paper` `vision` `imitation-learning` `policy-guidance`.
