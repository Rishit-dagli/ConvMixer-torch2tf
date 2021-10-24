# ConvMixer-torch2tf

This repository hosts code for converting the original ConvMixer [^1] (PyTorch) models to TensorFlow. In this repo we convert these 3 ConvMixer models to TensorFlow SavedModels:

| Model Name | resolution | acc@1 | #params | File Size | TensorFlow Model |
|------------|:---:|:---:|:---:|----------:|:--------------:|
| ConvMixer-1536/20 | 224x224 | 81.37 | 51.6 x 10^6 | 184MB | [github](https://github.com/Rishit-dagli/ConvMixer-torch2tf/releases/download/untagged-de81892a1b06347b8d97/convmixer_1536_20.tar.gz)/[drive](https://drive.google.com/file/d/1qrzap4vi2KFQTHxf9h_AMbWGvtbP5rIA/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_1536_20.tar.gz) |
| ConvMixer-768/32 | 224x224 | 80.16 | 21.1 x 10^6 | 75MB | [github](https://github.com/Rishit-dagli/ConvMixer-torch2tf/releases/download/untagged-de81892a1b06347b8d97/convmixer_768_32.tar.gz)/[drive](https://drive.google.com/file/d/1NJgHKjPd3YC8XHypQIs5A05XKd15o0s3/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_768_32.tar.gz) |
| ConvMixer-1024/20 | 224x224 | 76.94 | 24.4 x 10^6 | 87MB | [github](https://github.com/Rishit-dagli/ConvMixer-torch2tf/releases/download/untagged-de81892a1b06347b8d97/convmixer_1024_20.tar.gz)/[drive](https://drive.google.com/file/d/1--jRgK0KmLtWCJswYtfxSIfEcjAOrJyv/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_1024_20.tar.gz) |

ConvMixer is a simple model, proposed in the paper "Patches Are All You Need?" [^2] for image classification pre-trained on ImageNet-1K. ConvMixer uses only standard convolutions to achieve the mixing steps. Despite it's simplicity it outperforms ViT and MLP-Mixer. Using the [`conversion.ipynb`](conversion.ipynb) notebook, one should be able to take a model from the pre-trained models and convert that to TensorFlow and use that with TensorFlow Hub and Keras.

The original model classes and weights were converted using the `onnx-tf` tool [^3].

## References

[^1]: Official Code Implementation: https://github.com/tmp-iclr/convmixer
[^2]: Anonymous. Patches Are All You Need? 2021. openreview.net, https://openreview.net/forum?id=TVHS5Y4dNvM.
[^3]: onnx-tensorflow. Tensorflow Backend for ONNX. https://github.com/onnx/onnx-tensorflow
