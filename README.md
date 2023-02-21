# insect-identification
Insect identification from user images in the wild. Built with Python, PyTorch. Honours dissertation project.


## Colab Notebooks
- [ResNet training over Leeds butterfly dataset](https://colab.research.google.com/drive/1JqHID3-KIvsfbumllTjkLdK874SsaJNE?usp=sharing)
- [ResNet training over Leeds butterfly dataset V2](https://colab.research.google.com/drive/1NaDv2CKRmSXBhmNzefaneiW2hQF0qy_T?usp=sharing)
- [ResNet inference over Leeds butterfly dataset](https://colab.research.google.com/drive/1c8VLUCzBIN1YQsZRbxZehzIvayy_TLSO?usp=sharing)
- [ResNet training with the British Carabid Collection (7 classes version)](https://colab.research.google.com/drive/16oIcx00ae0xaplaCDcvFyCOrd8zcLKLM?usp=sharing) --> Training completed 03/01/22
- [Training with the full IP102](https://colab.research.google.com/drive/1uCMSaN3Xq_CiHeduMSPDhU1hi-STMkER?usp=sharing) -> [Latest results on WandB](https://wandb.ai/mawady-stirling/insect_IP102)
- [Training with the full British Carabid Collection](https://colab.research.google.com/drive/1d4mfJhuquR0AEMNnJK8Xet-4_RD8ooCW?usp=sharing) -> [Latest results on WandB](https://wandb.ai/mawady-stirling/insect_carabids/overview)
- [Inference over 7-class Carabid dataset](https://colab.research.google.com/drive/1lhOWyEJ9Y9N2nN4qeGGJ5_ISNnAHv8Bm?usp=sharing)
- [Inference over entire Carabid set](https://colab.research.google.com/drive/1lhOWyEJ9Y9N2nN4qeGGJ5_ISNnAHv8Bm)
- [iNat2021_mini training](https://colab.research.google.com/drive/14YRnjzAJ7hm8F8V9S6lCQ3I0ZxQIWYEp) 
---
## Gradio demo notebooks
- [Butterfly demo code](https://colab.research.google.com/drive/1bfiqPwL-ueeRDCy_Atl-fmKfhHYo0KnS?usp=sharing)
## Demos running on HuggingFace:
- [Butterfly demo](https://huggingface.co/spaces/ttheland/demo-butterfly-spaces)
---
## Datasets
- [IP102](https://github.com/xpwu95/IP102) [^1] (Classification: > 75,000 images in 102 classes, Detection: 19,000 images) --> The dataset can be downloaded from this [[link](https://drive.google.com/drive/folders/1svFSy2Da3cVMvekBwe13mzyx38XZ9xWo?usp=sharing)]
- [Leeds Butterfly Dataset](http://www.josiahwang.com/dataset/leedsbutterfly/) (Classification: 832 images in 10 classes)
- [British Carabid Collection](https://zenodo.org/record/3549369#.XvI_jMfVLIU) [^2] - (Classification: > 60k specimens in 291 classes)
- [iNaturalist2021 insect subset](https://github.com/visipedia/inat_comp/tree/master/2021) (Classification: 688,942 insect images in 2,526 classes). available through [torchvision](https://pytorch.org/vision/stable/datasets.html#inaturalist).

---

[^1]: Wu, Xiaoping, Chi Zhan, Yu-Kun Lai, Ming-Ming Cheng, and Jufeng Yang. "Ip102: A large-scale benchmark dataset for insect pest recognition." In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pp. 8787-8796. 2019.
[^2]: Hansen, Oskar Liset Pryds, Svenning, Jens-Christian, Olsen, Kent, Dupont, Steen, Garner, Beulhah H., Iosifidis, Alexandros, Price, Benjamin W., & Høye, Toke T. (2019). Image data used for publication "Species-level image classification with convolutional neural network enable insect identification from habitus images " [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3549369
