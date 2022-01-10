# insect-identification
Honours dissertation project.

To-Do:
[X] Make to do list through GitHub
[ ] Include Wandb.ai in model training
[ ] Data split and organisation using sklearn
[ ] Dataset download from Drive (zipfile)
[ ] Train model on iNaturalist Insecta subset using torchvision
[ ] Improve current models' performance with data augmentation (random rotations)
[ ] Train model on IP102 dataset

---
## Interim Demo
- [ResNet training over Leeds butterfly dataset](https://colab.research.google.com/drive/1JqHID3-KIvsfbumllTjkLdK874SsaJNE?usp=sharing) --> Seems to be working as expected!
- [ResNet training over Leeds butterfly dataset V2](https://colab.research.google.com/drive/1oSc3CjQWnoguIFReSTg5YSlTJ0R0v5LG?usp=sharing)
  - Add progress bar
  - Add metrics to handle imbalance dataset
  - Automatically download trained data after training
- [ResNet inference over Leeds butterfly dataset](https://colab.research.google.com/drive/1c8VLUCzBIN1YQsZRbxZehzIvayy_TLSO?usp=sharing)
- [ResNet training with the British Carabid Collection (7 classes version)](https://colab.research.google.com/drive/16oIcx00ae0xaplaCDcvFyCOrd8zcLKLM?usp=sharing) --> Training completed 03/01/22
- [Inference over Carabid dataset](https://colab.research.google.com/drive/1lhOWyEJ9Y9N2nN4qeGGJ5_ISNnAHv8Bm?usp=sharing) --> Works great on the training set. So-so performance on images from the wild.
---
## Related implementation
- [wikilimo/mobile-pest-identification](https://github.com/wikilimo/mobile-pest-identification) -- [folder_link]() --> the code looks promising! Let's try it!
- 
---
## Datasets
- [IP102](https://github.com/xpwu95/IP102) [^1] (Classification: > 75,000 images in 102 clasees, Detection: 19,000 images) --> The request was sent (07/10/2021) but no reply! The dataset can be downloaded from this [[link](https://drive.google.com/drive/folders/1svFSy2Da3cVMvekBwe13mzyx38XZ9xWo?usp=sharing)]
- [Leeds Butterfly Dataset](http://www.josiahwang.com/dataset/leedsbutterfly/) (Classification: 832 images in 10 classes)
- [British Carabid Collection](https://zenodo.org/record/3549369#.XvI_jMfVLIU) [^2] - (Classification: > 60k specimens in 100+ classes)
- iNaturlist ???
---
[^1]: Wu, Xiaoping, Chi Zhan, Yu-Kun Lai, Ming-Ming Cheng, and Jufeng Yang. "Ip102: A large-scale benchmark dataset for insect pest recognition." In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pp. 8787-8796. 2019.
[^2]: Hansen, Oskar Liset Pryds, Svenning, Jens-Christian, Olsen, Kent, Dupont, Steen, Garner, Beulhah H., Iosifidis, Alexandros, Price, Benjamin W., & Høye, Toke T. (2019). Image data used for publication "Species-level image classification with convolutional neural network enable insect identification from habitus images " [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3549369
