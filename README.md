# ConvMixer-torch-2-tf

In this repo we convert these 3 ConvMixer models to TensorFlow SavedModels:

| Model Name | resolution | acc@1 | #params | File Size | PyTorchModel |
|------------|:---:|:---:|:---:|----------:|:--------------:|
| ConvMixer-1536/20 | 224x224 | 81.37 | 51.6 * 10^6 | 207MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_1536_20_ks9_p7.pth.tar) |
| ConvMixer-768/32 | 224x224 | 80.16 | 21.1 * 10^6 | 85MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_768_32_ks7_p7_relu.pth.tar) |
| ConvMixer-1024/20 | 224x224 | 76.94 | 24.4 * 10^6 | 98MB | [github](https://github.com/tmp-iclr/convmixer/releases/download/v1.0/convmixer_1024_20_ks9_p14.pth.tar) |
