# ConvMixer-torch-2-tf

In this repo we convert these 3 ConvMixer models to TensorFlow SavedModels:

| Model Name | resolution | acc@1 | #params | File Size | PyTorchModel |
|------------|:---:|:---:|:---:|----------:|:--------------:|
| ConvMixer-1536/20 | 224x224 | 81.37 | 51.6 * 10^6 | 184MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_1536_20_ks9_p7.pth.tar)/[drive](https://drive.google.com/file/d/1qrzap4vi2KFQTHxf9h_AMbWGvtbP5rIA/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_1536_20.tar.gz) |
| ConvMixer-768/32 | 224x224 | 80.16 | 21.1 * 10^6 | 75MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_768_32_ks7_p7_relu.pth.tar)/[drive](https://drive.google.com/file/d/1NJgHKjPd3YC8XHypQIs5A05XKd15o0s3/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_768_32.tar.gz) |
| ConvMixer-1024/20 | 224x224 | 76.94 | 24.4 * 10^6 | 87MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_1024_20_ks9_p14.pth.tar)/[drive](https://drive.google.com/file/d/1--jRgK0KmLtWCJswYtfxSIfEcjAOrJyv/view?usp=sharing)/[bucket](https://storage.googleapis.com/convmixer-hubmodels.appspot.com/convmixer_1024_20.tar.gz) |
