# Awesome Universal Manipulation Interface [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Representative papers, datasets, code, and hardware for Universal Manipulation Interface (UMI) and UMI-style robot-free manipulation demonstrations.

This list focuses on systems that turn in-the-wild human demonstrations into robot-ready supervision. It is seeded from Jingru Zhang's UMI survey notes and public resources available through 2026-04-20.

To contribute, open a pull request with one link, one short sentence on why it matters for UMI, and 3-5 tags.

**Tags:** `paper`, `preprint`, `survey`, `code`, `hardware`, `data`, `core-umi`, `interface`, `tracking`, `calibration`, `vision`, `multiview`, `active-perception`, `3d-perception`, `tactile`, `force`, `contact-rich`, `dexterous`, `bimanual`, `mobile`, `cross-embodiment`, `imitation-learning`, `diffusion-policy`, `policy-guidance`, `representation-learning`, `dataset`, `vla`.

## Core and Surveys

- [UMI](https://www.roboticsproceedings.org/rss20/p045.html) - *Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots*, RSS 2024. [Project](https://umi-gripper.github.io/) [Code](https://github.com/real-stanford/universal_manipulation_interface). Tags: `paper` `core-umi` `interface` `vision` `imitation-learning`.
- [UMI Topic Overview](https://www.emergentmind.com/topics/universal-manipulation-interface-umi) - Overview of UMI, FastUMI, exUMI, MV-UMI, DexUMI, ActiveUMI, UMI-on-Legs, and UMI-on-Air. Tags: `survey` `core-umi` `interface` `cross-embodiment`.
- [Diffusion Manipulation Survey](https://arxiv.org/abs/2504.08438) - *Diffusion Models for Robotic Manipulation: A Survey*, 2025.04. Tags: `survey` `diffusion-policy` `imitation-learning` `policy-guidance`.

## Interfaces, Tracking, and Perception

- [FastUMI](https://proceedings.mlr.press/v305/zhaxizhuoma25a.html) - *A Scalable and Hardware-Independent Universal Manipulation Interface with Dataset*, CoRL 2025. [Project](https://fastumi.com/FastUMI/) [arXiv](https://arxiv.org/abs/2409.19499). Tags: `paper` `interface` `hardware` `tracking` `dataset`.
- [Actuated UMI Gripper](https://actuated-umi.github.io/) - Open-source motorized UMI-compatible gripper. [Code](https://github.com/actuated-umi/actuated-umi-gripper). Tags: `hardware` `interface` `force` `code`.
- [UMI-3D](https://arxiv.org/abs/2604.14089) - *Extending Universal Manipulation Interface from Vision-Limited to 3D Spatial Perception*, 2026.04. [Project](https://umi-3d.github.io/). Tags: `preprint` `3d-perception` `tracking` `calibration` `vision`.
- [ORB-SLAM3 UMI Fork](https://github.com/cheng-chi/ORB_SLAM3) - SLAM backend used by the original UMI codebase and tutorials. Tags: `code` `tracking` `calibration` `core-umi`.
- [MV-UMI](https://arxiv.org/abs/2509.18757) - *A Scalable Multi-View Interface for Cross-Embodiment Learning*, 2025.09. [Project](https://mv-umi.github.io/). Tags: `preprint` `multiview` `vision` `cross-embodiment`.
- [ActiveUMI](https://arxiv.org/abs/2510.01607) - *Robotic Manipulation with Active Perception from Robot-Free Human Demonstrations*, 2025.10. [Project](https://activeumi.github.io/). Tags: `preprint` `active-perception` `vision` `policy-guidance`.

## Tactile, Force, and Dexterity

- [ViTaMIn](https://arxiv.org/abs/2504.06156) - *Learning Contact-Rich Tasks Through Robot-Free Visuo-Tactile Manipulation Interface*, 2025.04. [Project](https://chuanyune.github.io/ViTaMIn_page/). Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- [Touch in the Wild](https://arxiv.org/abs/2507.15062) - *Learning Fine-Grained Manipulation with a Portable Visuo-Tactile Gripper*, 2025.07. [Project](https://touchinthewild.github.io/) [OpenReview](https://openreview.net/forum?id=WabVVQKTUF). Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- [exUMI](https://proceedings.mlr.press/v305/xu25e.html) - *Extensible Robot Teaching System with Action-aware Task-agnostic Tactile Representation*, CoRL 2025. [Project](https://silicx.github.io/exUMI/) [OpenReview](https://openreview.net/forum?id=b86nyIOJWq). Tags: `paper` `tactile` `tracking` `calibration` `representation-learning`.
- [FARM](https://arxiv.org/abs/2510.13324) - *Tactile-Conditioned Diffusion Policy for Force-Aware Robotic Manipulation*, 2025.10. [Project](https://tactile-farm.github.io/). Tags: `preprint` `tactile` `force` `diffusion-policy` `contact-rich`.
- [ViTaMIn-B](https://arxiv.org/abs/2511.05858) - *A Reliable and Efficient Visuo-Tactile Bimanual Manipulation Interface*, 2025.11. Tags: `preprint` `bimanual` `tactile` `tracking` `contact-rich`.
- [UMI-FT](https://arxiv.org/abs/2601.09988) - *In-the-Wild Compliant Manipulation with UMI-FT*, 2026.01. [Project](https://umi-ft.github.io/). Tags: `preprint` `force` `contact-rich` `policy-guidance`.
- [TacUMI](https://arxiv.org/abs/2601.14550) - *A Multi-Modal Universal Manipulation Interface for Contact-Rich Tasks*, 2026.01. Tags: `preprint` `tactile` `force` `contact-rich` `policy-guidance`.
- [DexUMI](https://proceedings.mlr.press/v305/xu25b.html) - *Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation*, CoRL 2025. [Project](https://dex-umi.github.io/) [arXiv](https://arxiv.org/abs/2505.21864). Tags: `paper` `dexterous` `tactile` `cross-embodiment` `interface`.

## Cross-Embodiment Deployment

- [UMI-on-Legs](https://proceedings.mlr.press/v270/ha25a.html) - *Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers*, CoRL 2024. [Project](https://umi-on-legs.github.io/) [Code](https://github.com/real-stanford/umi-on-legs). Tags: `paper` `mobile` `cross-embodiment` `policy-guidance`.
- [UMI-on-Air](https://arxiv.org/abs/2510.02614) - *Embodiment-Aware Guidance for Embodiment-Agnostic Visuomotor Policies*, 2025.10. [Project](https://umi-on-air.github.io/) [Checkpoints](https://huggingface.co/LeCAR-Lab/umi-on-air_checkpoints). Tags: `preprint` `mobile` `cross-embodiment` `diffusion-policy` `policy-guidance`.

## Policy Learning

- [Diffusion Policy](https://arxiv.org/abs/2303.04137) - *Visuomotor Policy Learning via Action Diffusion*, RSS 2023. [Project](https://diffusion-policy.cs.columbia.edu/) [Code](https://github.com/real-stanford/diffusion_policy). Tags: `paper` `diffusion-policy` `imitation-learning` `code`.
- [ALOHA / ACT](https://arxiv.org/abs/2304.13705) - *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware*, 2023.04. [Project](https://tonyzhaozh.github.io/aloha/) [Code](https://github.com/tonyzhaozh/aloha). Tags: `paper` `bimanual` `hardware` `imitation-learning` `code`.
- [pi0](https://arxiv.org/abs/2410.24164) - *A Vision-Language-Action Flow Model for General Robot Control*, 2024.10. [Project](https://www.physicalintelligence.company/blog/pi0). Tags: `paper` `vla` `cross-embodiment` `imitation-learning`.
- [TouchGuide](https://arxiv.org/abs/2601.20239) - *Inference-Time Steering of Visuomotor Policies via Touch Guidance*, 2026.01. [Project](https://martelzhang.github.io/touchguide/). Tags: `preprint` `tactile` `diffusion-policy` `policy-guidance`.

## Datasets and Benchmarks

- [UMI Robot Dataset Community](https://umi-data.github.io/) - Community index for UMI-style robot datasets. Tags: `data` `dataset` `core-umi`.
- [FastUMI-100K](https://arxiv.org/abs/2510.08022) - *Advancing Data-driven Robotic Manipulation with a Large-scale UMI-style Dataset*, 2025.10. [Code and Data](https://github.com/MrKeee/FastUMI-100K). Tags: `preprint` `data` `dataset` `multiview` `vla`.
- [Open X-Embodiment](https://robotics-transformer-x.github.io/) - Large cross-embodiment robot dataset and benchmark. Tags: `data` `dataset` `cross-embodiment` `vla`.
- [DROID](https://droid-dataset.github.io/) - *A Large-Scale In-The-Wild Robot Manipulation Dataset*. Tags: `data` `dataset` `interface` `imitation-learning`.
- [BridgeData V2](https://rail-berkeley.github.io/bridgedata/) - Large real-world robot manipulation dataset. Tags: `data` `dataset` `imitation-learning`.

## Related Resources

- [GELLO](https://wuphilipp.github.io/gello_site/) - *A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators*. Tags: `hardware` `interface` `imitation-learning`.
- [MimicPlay](https://mimic-play.github.io/) - *Long-Horizon Imitation Learning by Watching Human Play*. Tags: `paper` `imitation-learning` `policy-guidance`.
