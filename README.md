# OBS Plugin: YOLO PID Control

<div align="center">

[![GitHub](https://img.shields.io/github/license/wxyahyj/obs-lingleipidkongzhi)](https://github.com/wxyahyj/obs-lingleipidkongzhi/blob/main/LICENSE)
[![GitHub Workflow Status](https://github.com/wxyahyj/obs-lingleipidkongzhi/actions/workflows/push.yaml/badge.svg)](https://github.com/wxyahyj/obs-lingleipidkongzhi/actions/workflows/push.yaml)
[![Total downloads](https://img.shields.io/github/downloads/wxyahyj/obs-lingleipidkongzhi/total)](https://github.com/wxyahyj/obs-lingleipidkongzhi/releases)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/wxyahyj/obs-lingleipidkongzhi)](https://github.com/wxyahyj/obs-lingleipidkongzhi/releases)

</div>

A plugin for [OBS Studio](https://obsproject.com/) that allows you to control PID settings using YOLO detection.

<p align="center">
  <a href="https://github.com/wxyahyj/obs-lingleipidkongzhi/">
    <b>⬇️ Download & Install YOLO PID Control ⬇️</b>
  </a>
</p>

Or, browse versions on [releases page](https://github.com/wxyahyj/obs-lingleipidkongzhi/releases).

## Usage

### Introduction

This plugin is meant to provide PID control functionality using YOLO object detection for OBS Studio.
It allows you to control various parameters based on detected objects in the video stream.

### Support and Help

Reach out to us on [GitHub Discussions](https://github.com/wxyahyj/obs-lingleipidkongzhi/discussions) for online / immediate help.

If you found a bug or want to suggest a feature or improvement please open an [issue](https://github.com/wxyahyj/obs-lingleipidkongzhi/issues).

### Technical Details

GPU support:

- On Windows, we use ONNX Runtime for model inference.
- On Mac we support CoreML for acceleration, which is efficient on Apple Silicon.
- On Linux CUDA, ROCM, and MIGraphX are supported if this plugin is built from source.
- The goal of this plugin is to be available for everyone on every system, even if they don't own a GPU.

Number of CPU threads is controllable through the UI settings. A 2-thread setting works best.

The pretrained YOLO model weights are used for object detection.

### Code Walkthrough

The plugin uses YOLO object detection to identify objects in the video stream and applies PID control based on the detected objects' positions and movements.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=wxyahyj/obs-lingleipidkongzhi&type=Date&theme=dark" />
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=wxyahyj/obs-lingleipidkongzhi&type=Date" />
  <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=wxyahyj/obs-lingleipidkongzhi&type=Date" />
</picture>
