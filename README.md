# insect-identification
Honours dissertation project.

## To-Do:
### February 2022
- [ ] Train model on IP102 dataset
    * [ ] dataset split using `os.symlink()`
- [ ] Finish Inference and Gradio demo for Carabid model
- [ ] Make the repository public
- [ ] Implement better ways to evaluate model performance on test sets
    * [ ] Table showing average per-class F1 and acc.
    * [ ] [Confusion matrix with Seaborn](https://stackoverflow.com/questions/35572000/how-can-i-plot-a-confusion-matrix)
- [ ] Train model on iNaturalist Insecta subset using torchvision

### January 2022
- [X] Make to do list through GitHub
- [X] Arrange meeting for interim demo (21.1.2022 10am)
- [X] Dataset download from Drive (zipfile)
- [X] Include Wandb.ai in model training. [Instructions](https://wandb.ai/quickstart/pytorch)
    * [X] Ensure hyperparameters are logged for the Carabid training
- [X] Data split and organisation programmatically
- [X] Train model on complete British Carabid set
    * [X] Improve model performance with data augmentation (random rotations)
- [X] Finish poster for session in February

---

## Notes from supervisor:
- Do anlysis using different lightweight classification models (e.g. resnet18, shufflenet, squeezenet, mobilenetv3), with option of quantization.
- Try one-class detection models (e.g. YoloV3, YoloV4, YoloV5, SSD, Retinanet) before classification for accurate recognition results.
- For experimentation, use Wandb.
- For demo, use huggingface with Gradio.
- [Demo for weighted accruacy / better visualization](https://colab.research.google.com/drive/1Jsdfmc4Xd3gJYui2VLXfUfHnOOMJnJAE?usp=sharing)

---

## Interim Demo
- [ResNet training over Leeds butterfly dataset](https://colab.research.google.com/drive/1JqHID3-KIvsfbumllTjkLdK874SsaJNE?usp=sharing) --> Seems to be working as expected!
- [ResNet training over Leeds butterfly dataset V2](https://colab.research.google.com/drive/1NaDv2CKRmSXBhmNzefaneiW2hQF0qy_T?usp=sharing)
  - Add progress bar
  - Add metrics to handle imbalance dataset
  - Automatically download trained data after training
- [ResNet inference over Leeds butterfly dataset](https://colab.research.google.com/drive/1c8VLUCzBIN1YQsZRbxZehzIvayy_TLSO?usp=sharing)
- [ResNet training with the British Carabid Collection (7 classes version)](https://colab.research.google.com/drive/16oIcx00ae0xaplaCDcvFyCOrd8zcLKLM?usp=sharing) --> Training completed 03/01/22
- [Training with the full IP102](https://colab.research.google.com/drive/1uCMSaN3Xq_CiHeduMSPDhU1hi-STMkER?usp=sharing) -- In Progress
- [Training with the full British Carabid Collection](https://colab.research.google.com/drive/1d4mfJhuquR0AEMNnJK8Xet-4_RD8ooCW?usp=sharing) -> [Latest results on WandB](https://wandb.ai/mawady-stirling/insect_carabids/overview)
- [Inference over 7-class Carabid dataset](https://colab.research.google.com/drive/1lhOWyEJ9Y9N2nN4qeGGJ5_ISNnAHv8Bm?usp=sharing) --> Works great on the test set. So-so performance on images from the wild.

---
## Gradio demo notebooks
- [Butterfly demo](https://colab.research.google.com/drive/1bfiqPwL-ueeRDCy_Atl-fmKfhHYo0KnS?usp=sharing)
---
## Datasets
- [IP102](https://github.com/xpwu95/IP102) [^1] (Classification: > 75,000 images in 102 classes, Detection: 19,000 images) --> The request was sent (07/10/2021) but no reply! The dataset can be downloaded from this [[link](https://drive.google.com/drive/folders/1svFSy2Da3cVMvekBwe13mzyx38XZ9xWo?usp=sharing)]
- [Leeds Butterfly Dataset](http://www.josiahwang.com/dataset/leedsbutterfly/) (Classification: 832 images in 10 classes)
- [British Carabid Collection](https://zenodo.org/record/3549369#.XvI_jMfVLIU) [^2] - (Classification: > 60k specimens in 291 classes)
- [iNaturalist2021 insect subset](https://github.com/visipedia/inat_comp/tree/master/2021) (Classification: 688,942 insect images in 2,526 classes). available through [torchvision](https://pytorch.org/vision/stable/datasets.html#inaturalist).

---

[^1]: Wu, Xiaoping, Chi Zhan, Yu-Kun Lai, Ming-Ming Cheng, and Jufeng Yang. "Ip102: A large-scale benchmark dataset for insect pest recognition." In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pp. 8787-8796. 2019.
[^2]: Hansen, Oskar Liset Pryds, Svenning, Jens-Christian, Olsen, Kent, Dupont, Steen, Garner, Beulhah H., Iosifidis, Alexandros, Price, Benjamin W., & Høye, Toke T. (2019). Image data used for publication "Species-level image classification with convolutional neural network enable insect identification from habitus images " [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3549369
