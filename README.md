# DFA: Dynamic Feature Aggregation for Efficient Video Object Detection

<div align="center">
  <img src="resources/mmtrack-logo.png" width="600"/>
</div>

[![PyPI](https://img.shields.io/pypi/v/mmtrack)](https://pypi.org/project/mmtrack)
[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmtracking.readthedocs.io/en/latest/)
[![badge](https://github.com/open-mmlab/mmtracking/workflows/build/badge.svg)](https://github.com/open-mmlab/mmtracking/actions)
[![codecov](https://codecov.io/gh/open-mmlab/mmtracking/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmtracking)
[![license](https://img.shields.io/github/license/open-mmlab/mmtracking.svg)](https://github.com/open-mmlab/mmtracking/blob/master/LICENSE)

Documentation: https://mmtracking.readthedocs.io/

## Introduction

MMTracking is an open source video perception toolbox based on PyTorch.
It is a part of the OpenMMLab project.

The master branch works with PyTorch 1.3 to 1.7.

<div align="left">
  <img src="https://user-images.githubusercontent.com/24663779/103343312-c724f480-4ac6-11eb-9c22-b56f1902584e.gif" width="800"/>
</div>

### Major features

- **The First Unified Video Perception Platform**

  We are the first open source toolbox that unifies versatile video perception tasks include video object detection, single object tracking, and multiple object tracking.

- **Modular Design**

  We decompose the video perception framework into different components and one can easily construct a customized method by combining different modules.

- **Simple, Fast and Strong**

  **Simple**: MMTracking interacts with other OpenMMLab projects. It is built upon [MMDetection](https://github.com/open-mmlab/mmdetection) that we can capitalize any detector only through modifying the configs.

  **Fast**: All operations run on GPUs. The training and inference speeds are faster than or comparable to other implementations.

  **Strong**: We reproduce state-of-the-art models and some of them even outperform the offical implementations.

## License

This project is released under the [Apache 2.0 license](LICENSE).

## Changelog

v0.5.0 was released in 04/01/2021.
Please refer to [changelog.md](docs/en/changelog.md) for details and release history.

## Benchmark and model zoo

Results and models are available in the [model zoo](docs/en/model_zoo.md).

Supported methods of video object detection:

- [x] [DFF](configs/vid/dff)
- [x] [FGFA](configs/vid/fgfa)
- [x] [SELSA](configs/vid/selsa)
- [x] [FGFA + DFA](configs/vid/fgfa)
- [x] [SELSA + DFA](configs/vid/selsa)

Supported methods of multi object tracking:

- [x] [SORT/DeepSORT](configs/mot/deepsort)
- [x] [Tracktor](configs/mot/tracktor)

Supported methods of single object tracking:

- [x] [SiameseRPN++](configs/sot/siamese_rpn)

## Installation

Please refer to [install.md](docs/en/install.md) for install instructions.

## Get Started

Please see [dataset.md](docs/en/dataset.md) and [quick_run.md](docs/en/quick_run.md) for the basic usage of MMTracking.
We also provide usage [tutorials](docs/en/tutorials/).

## Acknowledgement

MMTracking is an open source project that welcome any contribution and feedback.
We wish that the toolbox and benchmark could serve the growing research
community by providing a flexible as well as standardized toolkit to reimplement existing methods
and develop their own new video perception methods.

## Citation

If you find this repo useful for your research, please consider citing the paper
```
@article{cui2022dfa,
  title={DFA: Dynamic Feature Aggregation for Efficient Video Object Detection},
  author={Cui, Yiming},
  journal={arXiv preprint arXiv:2210.00588},
  year={2022}
}
@article{cui2021tf,
  title={TF-Blender: Temporal Feature Blender for Video Object Detection},
  author={Cui, Yiming and Yan, Liqi and Cao, Zhiwen and Liu, Dongfang},
  journal={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  year={2021}
}
```
