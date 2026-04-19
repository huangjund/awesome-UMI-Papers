# Awesome Universal Manipulation Interface [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of Universal Manipulation Interface (UMI) and UMI-style systems for in-the-wild robot demonstration, scalable manipulation data collection, and deployable robot policies.

This list is for robot learning researchers, builders of data-collection hardware, and anyone trying to understand how handheld human demonstrations become robot-ready supervision. It is seeded from Jingru Zhang's UMI survey notes and public papers available through 2026-04-20.

Contributions are welcome. Please read [contributing.md](contributing.md) before opening a pull request.

## Contents

- [Overview](#overview)
- [Surveys and Roadmaps](#surveys-and-roadmaps)
- [Core UMI](#core-umi)
- [UMI-Style Interfaces and Hardware](#umi-style-interfaces-and-hardware)
- [Tracking, Calibration, and Spatial Perception](#tracking-calibration-and-spatial-perception)
- [Multi-View and Active Perception](#multi-view-and-active-perception)
- [Tactile, Force, and Contact-Rich UMI](#tactile-force-and-contact-rich-umi)
- [Dexterous, Bimanual, and Human-Hand Interfaces](#dexterous-bimanual-and-human-hand-interfaces)
- [Cross-Embodiment and Mobile Deployment](#cross-embodiment-and-mobile-deployment)
- [Policy Learning and Representation Learning](#policy-learning-and-representation-learning)
- [Datasets and Benchmarks](#datasets-and-benchmarks)
- [Code, Hardware, and Build Guides](#code-hardware-and-build-guides)
- [Related Background](#related-background)

## Overview

Universal Manipulation Interface (UMI) is a family of portable data-collection systems that let people demonstrate manipulation skills with handheld interfaces instead of teleoperating a robot in every target environment. The central promise is to collect diverse, fast, in-the-wild demonstrations while preserving enough sensing, pose, timing, and action structure for robot policy learning.

Recommended reading paths: new readers should start with Core UMI and then skim Datasets and Benchmarks; hardware builders should read UMI-Style Interfaces and Hardware, Tracking, Calibration, and Spatial Perception, and Code, Hardware, and Build Guides; policy researchers should jump to Policy Learning and Representation Learning and then follow the modality-specific sections; contact-rich manipulation readers should focus on Tactile, Force, and Contact-Rich UMI.

Compact tag set: `paper`, `preprint`, `survey`, `code`, `hardware`, `data`, `core-umi`, `interface`, `tracking`, `vision`, `multiview`, `active-perception`, `3d-perception`, `tactile`, `force`, `contact-rich`, `dexterous`, `bimanual`, `mobile`, `cross-embodiment`, `imitation-learning`, `diffusion-policy`, `policy-guidance`, `representation-learning`, `dataset`, and `vla`.

## Surveys and Roadmaps

- [Universal Manipulation Interface (UMI)](https://www.emergentmind.com/topics/universal-manipulation-interface-umi) - Topic overview that situates UMI, FastUMI, exUMI, MV-UMI, DexUMI, ActiveUMI, UMI-on-Legs, and UMI-on-Air across hardware, sensing, and policy design. Tags: `survey` `core-umi` `interface` `cross-embodiment`.
- [Diffusion Models for Robotic Manipulation: A Survey](https://arxiv.org/abs/2504.08438) - Broader policy-learning context for diffusion-based manipulation methods used by many UMI-style systems. Tags: `survey` `diffusion-policy` `imitation-learning` `policy-guidance`.

## Core UMI

- [Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots](https://www.roboticsproceedings.org/rss20/p045.html) - The RSS 2024 root system for UMI: handheld grippers, wrist-only egocentric sensing, latency matching, and relative trajectory actions for robot-agnostic manipulation policies. [project](https://umi-gripper.github.io/) [code](https://github.com/real-stanford/universal_manipulation_interface). Tags: `paper` `core-umi` `interface` `vision` `imitation-learning`.

## UMI-Style Interfaces and Hardware

- [FastUMI: A Scalable and Hardware-Independent Universal Manipulation Interface with Dataset](https://proceedings.mlr.press/v305/zhaxizhuoma25a.html) - Redesigns UMI around modular, hardware-decoupled components, simpler tracking, and faster verification for larger-scale data collection. [project](https://fastumi.com/FastUMI/) [arXiv](https://arxiv.org/abs/2409.19499). Tags: `paper` `interface` `hardware` `tracking` `dataset`.
- [Actuated UMI Gripper](https://actuated-umi.github.io/) - Open-source actuated gripper that matches the handheld UMI geometry, useful when the deployment gripper must mirror data-collection hardware. [code](https://github.com/actuated-umi/actuated-umi-gripper). Tags: `hardware` `interface` `force` `code`.

## Tracking, Calibration, and Spatial Perception

- [UMI-3D: Extending Universal Manipulation Interface from Vision-Limited to 3D Spatial Perception](https://arxiv.org/abs/2604.14089) - Adds a lightweight LiDAR-centric SLAM and spatiotemporal calibration stack to make UMI-style data more robust under occlusion, weak texture, and dynamic scenes. [project](https://umi-3d.github.io/). Tags: `preprint` `3d-perception` `tracking` `calibration` `vision`.
- [ORB-SLAM3 UMI Fork](https://github.com/cheng-chi/ORB_SLAM3) - SLAM backend used by the original UMI codebase and tutorials. Tags: `code` `tracking` `calibration` `core-umi`.

## Multi-View and Active Perception

- [MV-UMI: A Scalable Multi-View Interface for Cross-Embodiment Learning](https://arxiv.org/abs/2509.18757) - Adds third-person context to egocentric UMI observations while masking and inpainting human pixels to preserve cross-embodiment transfer. [project](https://mv-umi.github.io/). Tags: `preprint` `multiview` `vision` `cross-embodiment`.
- [ActiveUMI: Robotic Manipulation with Active Perception from Robot-Free Human Demonstrations](https://arxiv.org/abs/2510.01607) - Records operator head motion and active egocentric viewing so policies can learn when and how to move their viewpoint during long-horizon or occluded tasks. [project](https://activeumi.github.io/). Tags: `preprint` `active-perception` `vision` `policy-guidance`.

## Tactile, Force, and Contact-Rich UMI

- [ViTaMIn: Learning Contact-Rich Tasks Through Robot-Free Visuo-Tactile Manipulation Interface](https://arxiv.org/abs/2504.06156) - Introduces a robot-free visuo-tactile handheld interface with a compliant gripper and tactile representation learning for contact-rich tasks. [project](https://chuanyune.github.io/ViTaMIn_page/). Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- [Touch in the Wild: Learning Fine-Grained Manipulation with a Portable Visuo-Tactile Gripper](https://arxiv.org/abs/2507.15062) - Uses a lightweight tactile gripper and cross-modal representation learning for fine-grained tasks collected across real-world environments. [project](https://touchinthewild.github.io/) [OpenReview](https://openreview.net/forum?id=WabVVQKTUF). Tags: `preprint` `tactile` `contact-rich` `representation-learning`.
- [exUMI: Extensible Robot Teaching System with Action-aware Task-agnostic Tactile Representation](https://proceedings.mlr.press/v305/xu25e.html) - Extends UMI with robust AR-based proprioception, modular tactile sensing, automated calibration, and tactile prediction pretraining. [project](https://silicx.github.io/exUMI/) [OpenReview](https://openreview.net/forum?id=b86nyIOJWq). Tags: `paper` `tactile` `tracking` `calibration` `representation-learning`.
- [Tactile-Conditioned Diffusion Policy for Force-Aware Robotic Manipulation](https://arxiv.org/abs/2510.13324) - FARM modifies UMI with GelSight tactile sensing and an actuated matching gripper so policies can predict pose, grip width, and grip force. [project](https://tactile-farm.github.io/). Tags: `preprint` `tactile` `force` `diffusion-policy` `contact-rich`.
- [ViTaMIn-B: A Reliable and Efficient Visuo-Tactile Bimanual Manipulation Interface](https://arxiv.org/abs/2511.05858) - Builds a bimanual visuo-tactile interface with DuoTact sensors, tactile point-cloud representations, and Meta Quest based 6-DoF pose tracking. Tags: `preprint` `bimanual` `tactile` `tracking` `contact-rich`.
- [In-the-Wild Compliant Manipulation with UMI-FT](https://arxiv.org/abs/2601.09988) - Mounts compact six-axis force/torque sensors on each finger and learns adaptive compliance policies for force-sensitive in-the-wild manipulation. [project](https://umi-ft.github.io/). Tags: `preprint` `force` `contact-rich` `policy-guidance`.
- [TacUMI: A Multi-Modal Universal Manipulation Interface for Contact-Rich Tasks](https://arxiv.org/abs/2601.14550) - Combines visual, tactile, force/torque, and pose signals in a compact robot-compatible gripper, then uses temporal modeling for event segmentation. Tags: `preprint` `tactile` `force` `contact-rich` `policy-guidance`.

## Dexterous, Bimanual, and Human-Hand Interfaces

- [DexUMI: Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation](https://proceedings.mlr.press/v305/xu25b.html) - Uses wearable hand exoskeletons, retargeting, tactile input, and robot-hand inpainting to transfer human dexterity to multiple robot hands. [project](https://dex-umi.github.io/) [arXiv](https://arxiv.org/abs/2505.21864). Tags: `paper` `dexterous` `tactile` `cross-embodiment` `interface`.

## Cross-Embodiment and Mobile Deployment

- [UMI-on-Legs: Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers](https://proceedings.mlr.press/v270/ha25a.html) - Deploys UMI-trained manipulation policies on a quadruped by passing task-frame end-effector trajectories to a simulation-trained whole-body controller. [project](https://umi-on-legs.github.io/) [code](https://github.com/real-stanford/umi-on-legs). Tags: `paper` `mobile` `cross-embodiment` `policy-guidance`.
- [UMI-on-Air: Embodiment-Aware Guidance for Embodiment-Agnostic Visuomotor Policies](https://arxiv.org/abs/2510.02614) - Guides diffusion-policy samples with low-level controller feedback so UMI-trained policies stay feasible on constrained aerial manipulators. [project](https://umi-on-air.github.io/) [checkpoints](https://huggingface.co/LeCAR-Lab/umi-on-air_checkpoints). Tags: `preprint` `mobile` `cross-embodiment` `diffusion-policy` `policy-guidance`.

## Policy Learning and Representation Learning

- [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/abs/2303.04137) - Widely used action-generation backbone for UMI and UMI-style visuomotor policies. [project](https://diffusion-policy.cs.columbia.edu/) [code](https://github.com/real-stanford/diffusion_policy). Tags: `paper` `diffusion-policy` `imitation-learning` `code`.
- [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware](https://arxiv.org/abs/2304.13705) - ACT/ALOHA work that provides a strong behavior-cloning baseline and low-cost manipulation hardware reference for later UMI-style datasets. [project](https://tonyzhaozh.github.io/aloha/) [code](https://github.com/tonyzhaozh/aloha). Tags: `paper` `bimanual` `hardware` `imitation-learning` `code`.
- [pi0: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) - Generalist VLA model family often discussed as a downstream consumer for large UMI-style datasets and cross-embodiment data. [project](https://www.physicalintelligence.company/blog/pi0). Tags: `paper` `vla` `cross-embodiment` `imitation-learning`.
- [TouchGuide: Inference-Time Steering of Visuomotor Policies via Touch Guidance](https://arxiv.org/abs/2601.20239) - Steers pretrained diffusion or flow visuomotor policies with tactile feasibility feedback at inference time instead of retraining the base policy. [project](https://martelzhang.github.io/touchguide/). Tags: `preprint` `tactile` `diffusion-policy` `policy-guidance`.

## Datasets and Benchmarks

- [UMI Robot Dataset Community](https://umi-data.github.io/) - Community index for UMI-style robot datasets and related resources. Tags: `data` `dataset` `core-umi`.
- [FastUMI-100K: Advancing Data-driven Robotic Manipulation with a Large-scale UMI-style Dataset](https://arxiv.org/abs/2510.08022) - Large multimodal UMI-style dataset with 100K+ trajectories, household tasks, multi-view fisheye video, end-effector states, and text annotations. [code and data](https://github.com/MrKeee/FastUMI-100K). Tags: `preprint` `data` `dataset` `multiview` `vla`.

## Code, Hardware, and Build Guides

Builder-facing entry points are attached directly to the relevant papers above. Start with the `project`, `code`, and `hardware` links in Core UMI, UMI-Style Interfaces and Hardware, Tactile, Force, and Contact-Rich UMI, Dexterous, Bimanual, and Human-Hand Interfaces, and Cross-Embodiment and Mobile Deployment.

## Related Background

- [Open X-Embodiment](https://robotics-transformer-x.github.io/) - Cross-embodiment robot dataset and model benchmark useful for comparing the role of UMI-style data at larger scale. Tags: `data` `dataset` `cross-embodiment` `vla`.
- [DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset](https://droid-dataset.github.io/) - Robot-collected in-the-wild manipulation dataset that complements robot-free UMI-style data collection. Tags: `data` `dataset` `interface` `imitation-learning`.
- [BridgeData V2](https://rail-berkeley.github.io/bridgedata/) - Large real-world robot manipulation dataset for studying data diversity, multi-task imitation, and generalization. Tags: `data` `dataset` `imitation-learning`.
- [GELLO: A General, Low-Cost, and Intuitive Teleoperation Framework for Robot Manipulators](https://wuphilipp.github.io/gello_site/) - Low-cost robot teleoperation baseline that contrasts with robot-free handheld UMI demonstrations. Tags: `hardware` `interface` `imitation-learning`.
- [MimicPlay: Long-Horizon Imitation Learning by Watching Human Play](https://mimic-play.github.io/) - Human-guided long-horizon manipulation learning background relevant to demonstration collection and skill decomposition. Tags: `paper` `imitation-learning` `policy-guidance`.
