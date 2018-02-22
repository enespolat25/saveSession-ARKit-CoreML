# saveSession-ARKit-CoreML
A project to show the possibility to save and load session in ARKit using CoreML, the end goal is to make a guided tours app
the instructons, the code and a video showing how the app works will be uploaded shortly

[Demo Video - on Youtube](will be uploaded shortly)

Based on [CoreML-in-ARKit by hanleyweng](https://github.com/hanleyweng/CoreML-in-ARKit)

Model: Inception V3

Language: Swift 4.0

Written in: Xcode 9.0

Content Technology: SceneKit

Tested on iPhone 6s running iOS 11.2.6 (15D100)

## Instructions

You'll have to download "Inceptionv3.mlmodel" from [Apple's Machine Learning page](https://developer.apple.com/machine-learning/), and copy it into your XCode project. (As depicted in the following gif)

![Gif to show dragging and dropping of model into XCode](post-media/AddingMLModel.gif)

[_(Gif via Atomic14)_](https://github.com/atomic14/VisionCoreMLSample)

If you're having issues, double check that the model is part of a target [(source: stackoverflow)](https://stackoverflow.com/questions/45884085/model-is-not-part-of-any-target-add-the-model-to-a-target-to-enable-generation).

## Footnotes

The Objects are the real objects seen by the camera
The anchor is an object that you set as the reference point the reference system in every sesson of ARKit
The nodes are arkit nodes composed by a point and a the name of an object
You can change the anchor using the change anchor button but the nodes will be resetted

The precision is given by by the precision of the compass, the more still you are the better is the precision
Is planned the automatic addiction of multiple anchors to improve precision
