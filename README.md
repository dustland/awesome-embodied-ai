# Awesome Embodied AI [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome projects, resources, and research related to **Embodied AI** and **Humanoid Robotics**.

## Contents

- [Introduction](#introduction)
- [Scene Understanding](#scene-understanding)
- [Data Collection](#data-collection)
- [Action Output](#action-output)
- [Open Source Projects](#open-source-projects)
- [Datasets](#datasets)
- [Companies & Robots](#companies--robots)
- [Research Papers](#research-papers)
- [Community](#community)

## Introduction

Embodied Intelligence refers to AI systems that learn and interact through physical embodiment, often in robotics platforms. This list focuses on projects combining artificial intelligence with physical interaction capabilities.

## Scene Understanding

### Image Processing

|            | Description               | Paper                                     | Code                                                         |
| ---------- | ------------------------- | ----------------------------------------- | ------------------------------------------------------------ |
| SAM        | Segmentation              | [Paper](https://arxiv.org/abs/2304.02643) | [Code](https://github.com/facebookresearch/segment-anything) |
| YOLO-World | Open-Vocabulary Detection | [Paper](https://arxiv.org/abs/2401.17270) | [Code](https://github.com/AILab-CVC/YOLO-World)              |

### Point Cloud Processing

|            | Description   | Paper                                     | Code                                                         |
| ---------- | ------------- | ----------------------------------------- | ------------------------------------------------------------ |
| SAM3D      | Segmentation  | [Paper](https://arxiv.org/abs/2306.03908) | [Code](https://github.com/Pointcept/SegmentAnything3D)       |
| PointMixer | Understanding | [Paper](https://arxiv.org/abs/2401.17270) | [Code](https://github.com/LifeBeyondExpectations/PointMixer) |

### Multi-Modal Grounding

|              | Description                   | Paper                                                   | Code                                                               |
| ------------ | ----------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------ |
| GPT4V        | MLM(Image+Language->Language) | [Paper](https://arxiv.org/abs/2303.08774)               |                                                                    |
| Claude3-Opus | MLM(Image+Language->Language) | [Paper](https://www.anthropic.com/news/claude-3-family) |                                                                    |
| GLaMM        | Pixel Grounding               | [Paper](https://arxiv.org/abs/2311.03356)               | [Code](https://github.com/mbzuai-oryx/groundingLMM)                |
| All-Seeing   | Pixel Grounding               | [Paper](https://arxiv.org/abs/2402.19474)               | [Code](https://github.com/OpenGVLab/all-seeing)                    |
| LEO          | 3D                            | [Paper](https://arxiv.org/abs/2311.12871)               | [Code](https://github.com/embodied-generalist/embodied-generalist) |

## Data Collection

### From Video

|               | Description | Paper                                                      | Code                                      |
| ------------- | ----------- | ---------------------------------------------------------- | ----------------------------------------- |
| Vid2Robot     |             | [Paper](https://vid2robot.github.io/vid2robot.pdf)         |                                           |
| RT-Trajectory |             | [Paper](https://arxiv.org/abs/2311.01977)                  |                                           |
| MimicPlay     |             | [Paper](https://mimic-play.github.io/assets/MimicPlay.pdf) | [Code](https://github.com/j96w/MimicPlay) |

### Hardware

|           | Description    | Paper                                                      | Code                                                                      |
| --------- | -------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------- |
| UMI       | Two-Fingers    | [Paper](https://arxiv.org/abs/2402.10329)                  | [Code](https://github.com/real-stanford/universal_manipulation_interface) |
| DexCap    | Five-Fingers   | [Paper](https://dex-cap.github.io/assets/DexCap_paper.pdf) | [Code](https://github.com/j96w/DexCap)                                    |
| HIRO Hand | Hand-over-hand | [Paper](https://sites.google.com/view/hiro-hand)           |                                                                           |

### Generative Simulation

|          | Description | Paper                                     | Code                                                    |
| -------- | ----------- | ----------------------------------------- | ------------------------------------------------------- |
| MimicGen |             | [Paper](https://arxiv.org/abs/2310.17596) | [Code](https://github.com/NVlabs/mimicgen_environments) |
| RoboGen  |             | [Paper](https://arxiv.org/abs/2311.01455) | [Code](https://github.com/Genesis-Embodied-AI/RoboGen)  |

## Action Output

### Generative Imitation Learning

|                  | Description | Paper                                     | Code                                                      |
| ---------------- | ----------- | ----------------------------------------- | --------------------------------------------------------- |
| Diffusion Policy |             | [Paper](https://arxiv.org/abs/2303.04137) | [Code](https://github.com/real-stanford/diffusion_policy) |
| ACT              |             | [Paper](https://arxiv.org/abs/2304.13705) | [Code](https://github.com/tonyzhaozh/act)                 |

### Affordance Map

|                              | Description                                | Paper                                                                                                                     | Code                                                                                         |
| ---------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| CLIPort                      | Pick&Place                                 | [Paper](https://arxiv.org/pdf/2109.12098.pdf)                                                                             | [Code](https://github.com/cliport/cliport)                                                   |
| Robo-Affordances             | Contact&Post-contact trajectories          | [Paper](https://arxiv.org/abs/2304.08488)                                                                                 | [Code](https://github.com/shikharbahl/vrb)                                                   |
| Robo-ABC                     |                                            | [Paper](https://arxiv.org/abs/2401.07487)                                                                                 | [Code](https://github.com/TEA-Lab/Robo-ABC)                                                  |
| Where2Explore                | Few shot learning from semantic similarity | [Paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/0e7e2af2e5ba822c9ad35a37b31b5dd4-Paper-Conference.pdf) |                                                                                              |
| Move as You Say              | Affordance to motion from diffusion model  | [Paper](https://arxiv.org/pdf/2403.18036.pdf)                                                                             |                                                                                              |
| AffordanceLLM                | Grounding affordance with LLM              | [Paper](https://arxiv.org/pdf/2401.06341.pdf)                                                                             |                                                                                              |
| Environment-aware Affordance |                                            | [Paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/bf78fc727cf882df66e6dbc826161e86-Paper-Conference.pdf) |                                                                                              |
| OpenAD                       | Open-Voc Affordance Detection              | [Paper](https://www.csc.liv.ac.uk/~anguyen/assets/pdfs/2023_OpenAD.pdf)                                                   | [Code](https://github.com/Fsoft-AIC/Open-Vocabulary-Affordance-Detection-in-3D-Point-Clouds) |
| RLAfford                     | End-to-End affordance learning             | [Paper](https://gengyiran.github.io/pdf/RLAfford.pdf)                                                                     |                                                                                              |
| General Flow                 | Collect affordance from video              | [Paper](https://general-flow.github.io/general_flow.pdf)                                                                  | [Code](https://github.com/michaelyuancb/general_flow)                                        |
| PreAffordance                | Pre-grasping planning                      | [Paper](https://arxiv.org/pdf/2404.03634.pdf)                                                                             |                                                                                              |
| ScenFun3d                    | Fine-grained functionality                 | [Paper](https://aycatakmaz.github.io/data/SceneFun3D-preprint.pdf)                                                        | [Code](https://github.com/SceneFun3D/scenefun3d)                                             |

### Question & Answer from LLM

|          | Description | Paper                                         | Code                                              |
| -------- | ----------- | --------------------------------------------- | ------------------------------------------------- |
| COPA     |             | [Paper](https://arxiv.org/abs/2403.08248)     |                                                   |
| ManipLLM |             | [Paper](https://arxiv.org/abs/2312.16217)     |                                                   |
| ManipVQA |             | [Paper](https://arxiv.org/pdf/2403.11289.pdf) | [Code](https://github.com/SiyuanHuang95/ManipVQA) |

### Language Corrections

|          | Description | Paper                                     | Code                                           |
| -------- | ----------- | ----------------------------------------- | ---------------------------------------------- |
| OLAF     |             | [Paper](https://arxiv.org/pdf/2310.17555) |                                                |
| YAYRobot |             | [Paper](https://arxiv.org/abs/2403.12910) | [Code](https://github.com/yay-robot/yay_robot) |

### Planning from LLM

|        | Description  | Paper                                     | Code                                                                          |
| ------ | ------------ | ----------------------------------------- | ----------------------------------------------------------------------------- |
| SayCan | API Level    | [Paper](https://arxiv.org/abs/2204.01691) | [Code](https://github.com/google-research/google-research/tree/master/saycan) |
| VILA   | Prompt Level | [Paper](https://arxiv.org/abs/2311.17842) |                                                                               |

## Open Source Projects

### Simulation Environments

- [Genesis](https://github.com/Genesis-Embodied-AI/Genesis) - Genesis is a physics platform designed for general-purpose Robotics/Embodied AI/Physical AI applications. It is simultaneously multiple things: A universal physics engine re-built from the ground up, capable of simulating a wide range of materials and physical phenomena.; A lightweight, ultra-fast, pythonic, and user-friendly robotics simulation platform. [⭐22747]
- [Habitat Sim](https://github.com/facebookresearch/habitat-sim) - A flexible, high-performance 3D simulator for Embodied AI research. Habitat-Sim is typically used with Habitat-Lab, a modular high-level library for end-to-end experiments in embodied AI. [⭐5000]
- [Isaac Sim](https://developer.nvidia.com/isaac/sim) - NVIDIA Isaac Sim™ is a reference application built on NVIDIA Omniverse that enables developers to simulate and test AI-driven robotics solutions in physically based virtual environments.
- [MuJoCo](https://mujoco.org/) - Physics engine for robotics, biomechanics, and graphics
- [PyBullet](https://pybullet.org/) - Physics simulation for robotics and machine learning
- [Gazebo](http://gazebosim.org/) - Robot simulation environment
- [SAPIEN](https://sapien.ucsd.edu/) - A SimulAted Part-based Interactive ENvironment
- [Webots](https://cyberbotics.com/) - Webots is an open source and multi-platform desktop application used to simulate robots. It provides a complete development environment to model, program and simulate robots.

### Perceptions

### Teleops & Retargeting

- [AnyTeleop](https://yzqin.github.io/anyteleop/) - A General Vision-Based Dexterous Robot Arm-Hand Teleoperation System
- [Dex Retargeting](https://github.com/dexsuite/dex-retargeting) - Various retargeting optimizers to translate human hand motion to robot hand motion.

### Feedback Generation

- [ChatTTS](https://github.com/2noise/ChatTTS) - A generative speech model for daily dialogue
- [Real3D-Portrait](https://real3dportrait.github.io/) - One-shot Realistic 3D Talking Portrait Synthesis
- [Hallo2](https://fudan-generative-vision.github.io/hallo2) - Long-Duration and High-Resolution Audio-driven Portrait Image Animation

## Research Frameworks

### Learning Frameworks

- [MoveIt](https://moveit.ros.org/) - Motion planning framework
- [OMPL](https://ompl.kavrakilab.org/) - Open Motion Planning Library
- [Drake](https://drake.mit.edu/) - Planning and control toolkit
- [GR-1](https://gr1-manipulation.github.io/) - ByteDance Research: Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation
- [Universal Manipulation Interface(UMI)](https://umi-gripper.github.io/)
- [Meta Motivo](https://metamotivo.metademolab.com/demo) - A first-of-its-kind behavioral foundation model to control a virtual physics-based humanoid agent for a wide range of whole-body tasks.
- [OpenVLA](https://openvla.github.io/) - OpenVLA sets a new state of the art for generalist robot manipulation policies. It supports controlling multiple robots out of the box and can be quickly adapted to new robot setups via parameter-efficient fine-tuning.

## Datasets

### Robot Learning Datasets & Models

- [RoboNet](https://www.robonet.wiki/) - Large-scale robot manipulation dataset
- [BEHAVIOR-1K](https://behavior.stanford.edu/) - Dataset of human household activities
- [Google Robot Data](https://github.com/google-research/robotics_datasets) - Various robotics datasets
- [Contact-GraspNet](https://github.com/NVlabs/contact-graspnet) - Dataset for robotic grasping
- [π0](https://github.com/Physical-Intelligence/openpi) - Opensource VLA models by Physical Intelligence

### Human Motion Datasets

- [AMASS](https://amass.is.tue.mpg.de/) - Large human motion dataset
- [Human3.6M](http://vision.imar.ro/human3.6m/) - Large-scale dataset for human sensing
- [CMU Graphics Lab Motion Capture Database](http://mocap.cs.cmu.edu/)

### Benchmarks

- [CALVIN](http://calvin.cs.uni-freiburg.de/) - CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks
- [DexYCB](https://dex-ycb.github.io/) - A Benchmark for Capturing Hand Grasping of Objects

## Companies & Robots

### Research Labs

- [Berkeley AI Research (BAIR)](https://bair.berkeley.edu/)
- [Stanford Robotics & Embodied Artificial Intelligence Lab (REAL)](http://real.stanford.edu/)
- [MIT CSAIL](https://www.csail.mit.edu/)
- [Google Research](https://research.google/research-areas/robotics/)
- [UT Austin Robot Perception and Learning Lab (RPL)](https://rpl.cs.utexas.edu/)

### Companies

- [Boston Dynamics](https://www.bostondynamics.com/)
- [Agility Robotics](https://www.agilityrobotics.com/)
- [Figure AI](https://www.figure.ai/)
- [1X Technologies](https://www.1x.tech/)
- [Sanctuary AI](https://www.sanctuary.ai/)
- [Fourier Intelligence](https://www.fftai.com) [[Github]](https://github.com/FFTAI/) [[Docs]](https://fftai.github.io/)
- [AgiBot](https://www.agibot.com/) [Github](https://github.com/AgibotTech)

### Humanoid Robotics

- [Atlas](https://www.bostondynamics.com/atlas) - Advanced humanoid robot by Boston Dynamics
- [Digit](https://www.agilityrobotics.com/digit) - Bipedal robot by Agility Robotics
- [Tesla Optimus](https://www.tesla.com/optimus) - Tesla's humanoid robot project
- [Figure 01](https://www.figure.ai/) - General purpose humanoid robot
- [Phoenix](https://github.com/PhoenixNine/Phoenix) - Open-source humanoid robot design
- [Fourier GR-2](https://www.fftai.com/products-gr2) - Fourier General Purpose Humanoid Robotics

## Research Papers

- [OKAMI: Teaching Humanoid Robots Manipulation Skills through Single Video Imitation](https://ut-austin-rpl.github.io/OKAMI/)
- [GR-MG: Leveraging Partially Annotated Data via Multi-Modal Goal Conditioned Policy](https://arxiv.org/abs/2408.14368)

### Researchers

[Yuke Zhu](https://yukezhu.me) [Yuzhe Qin](https://yzqin.github.io/) [Jim Fan](https://jimfan.me/)

## Community

### Conferences

- [RSS](http://www.roboticsconference.org/) - Robotics: Science and Systems
- [ICRA](https://www.icra2024.org/) - International Conference on Robotics and Automation
- [CoRL](https://www.corl2024.org/) - Conference on Robot Learning
- [IROS](https://iros2024.org/) - International Conference on Intelligent Robots and Systems

### Forums & Discussion

- [ROS Discourse](https://discourse.ros.org/)
- [Robotics StackExchange](https://robotics.stackexchange.com/)
- [Reddit r/robotics](https://www.reddit.com/r/robotics/)

## Contributing

Please read the [contribution guidelines](CONTRIBUTING.md) before making a contribution.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.