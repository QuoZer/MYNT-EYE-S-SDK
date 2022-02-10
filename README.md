# MYNT® EYE S SDK

[![](https://img.shields.io/badge/MYNT%20EYE%20S%20SDK-2.5.0-brightgreen.svg?style=flat)](https://github.com/slightech/MYNT-EYE-S-SDK)

## Fork changes

This fork incorporates fixes to some of the issues mentioned on the original repo page. ROS Wrapper nodelet was updated to support plugins. 


## Overview

MYNT® EYE S SDK is a cross-platform library for MYNT® EYE Standard cameras.

The following platforms have been tested:

* Windows 10/11
* Ubuntu 18.04 / 16.04 / 14.04
* Jetson TX2

Please follow the guide doc to install the SDK on different platforms.

## Documentations

* [API Doc](https://github.com/slightech/MYNT-EYE-S-SDK/releases): API reference, some guides and data spec.
  * en: [![](https://img.shields.io/badge/Download-PDF-blue.svg?style=flat)](https://readthedocs.org/projects/mynt-eye-s-sdk/downloads/pdf/latest/) [![](https://img.shields.io/badge/Download-HTML-blue.svg?style=flat)](https://readthedocs.org/projects/mynt-eye-s-sdk/downloads/htmlzip/latest/) [![](https://img.shields.io/badge/Online-HTML-blue.svg?style=flat)](https://mynt-eye-s-sdk.readthedocs.io/en/latest/)

## Plugins 

Get plugin files (and some old sdk docs): [PLUGINS_DRIVE][https://drive.google.com/drive/folders/1eG66rmCCOMrQVYaU8FvtJOEsnEEaxYVc]
## Firmwares

~~[MYNTEYE_BOX]: http://doc.myntai.com/mynteye/s/download~~

Old docs on firmware upgrade: [SDK v1.8][https://slightech.github.io/MYNT-EYE-SDK/upgrade_firmware.html]

Get firmwares from our online disks: [FIRMWARE_DRIVE][https://drive.google.com/drive/folders/1rz7swzOp9zp7Xty-o2cJzLgFYnC71WQZ].


## Config 

There are quite a few config files you may find useful: 
* The ROS Wrapper settings are listed in `wrappers/ros/src/mynt_eye_ros_wrapper/config/process/process_config.yaml`. Disparity algorithm, plugin path and native streams can be set up there. 
* The settings controlling camera sensor parameters cam be accesed and edited via `wrappers/ros/src/mynt_eye_ros_wrapper/config/device`
* ...



## Usage

In short,

```bash
$ make
Usage:
  make help            show help message
  make apidoc          make api doc
  make opendoc         open api doc (html)
  make init            init project
  make build           build project
  make test            build test and run
  make install         install project
  make samples         build samples
  make ros             build ros wrapper
  make clean|cleanall  clean generated or useless things
```

Init project, build samples and run something.

```bash
make init
make samples
./samples/_output/bin/camera_with_junior_device_api
```


## License

This project is licensed under the [Apache License, Version 2.0](LICENSE). Copyright 2018 Slightech Co., Ltd.
