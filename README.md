This repository contains the code of the implementation of the paper entitled "[Urban Sound Classification Using Convolutional Neural Network and Long Short Term Memory Based on Multiple Features](https://ieeexplore.ieee.org/document/9268723/)" published in **2020 Fourth International Conference On Intelligent Computing in Data Sciences (ICDS)**.

## Abstract of the Paper
There are many sounds all around us and our brain can easily and clearly identify them. Furthermore, our brain processes the received sound signals continuously and provides us with relevant environmental knowledge. Although not up to the level of accuracy of the brain, there are some smart devices which can extract necessary information from an audio signal with the help of different algorithms. Over the years several models like the Convolutional Neural Network (CNN), Artificial Neural Network (ANN), Region-Convolutional Neural Network (R-CNN) and many machine learning techniques have been adopted to classify sound accurately and these have shown promising results in the recent years in distinguishing spectra-temporal pictures and different sound classes. The novelty of our research lies in showing that the long-short term memory (LSTM) shows a better result in classification accuracy compared to CNN for many features used. Moreover, we have tested the accuracy of the models based on different techniques such as augmentation and stacking of different spectral-features. In such a way it was possible with our LSTM model, to reach an accuracy of 98.81%, which is state-of-the-art performance on the UrbanSound8k dataset.

## Dataset
UrbanSound8k, a popular dataset for urban sound classification, consists of 8732 labeled sound clips from 10 different classes.
* Available at: https://urbansounddataset.weebly.com/urbansound8k.html

## Extracted Features from Audio Files

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/MFCC.PNG" width="400" />
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Mel-Spectrogram.PNG" width="400" />
</p>

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Chroma_STFT.PNG" width="400" />
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Chroma_CQT.PNG" width="400" />
</p>

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Chroma_Cens.PNG" width="400" />
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Spectral.PNG" width="400" />
</p>

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Tonnetz.PNG" width="400" />
</p>

**<p align="center">Figure 1: Extracted spetral feature from audio clip.</p>**

## Data Augmentation

Three distinct data augmentation techniques were employed, resulting in an expansion of the original 8732 audio files from the UrbanSound8K dataset to a total of 78588 labeled audio clips.

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Pitch%20Shift.PNG" width="400" />
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Time%20Stretch.PNG" width="400" />
</p>

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/Time%20Stretch%20and%20Pitch%20Shift.PNG" width="400" />
</p>

**<p align="center">Figure 2: Audio signals after applying different augmentation techniques.</p>**

## Performance Evaluation 

<p align="center">
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/CNN%20vs%20LSTM%20without%20Augmentation.JPG" width="400" />
<img src="https://github.com/arkog96/Urban-Sound-Classification-using-CNN-and-LSTM-based-on-Multiple-Features/blob/main/figures/CNN%20vs%20LSTM%20with%20Augmentation.png" width="400" />
</p>

**<p align="center">Figure 3: Performance comparison of CNN and LSTM using different spectral features with/without Data Augmentation.</p>**

## System Requirements 
* Python 3+
* [LibROSA](https://librosa.org/doc/latest/index.html)
* [FFmpeg](https://pypi.org/project/ffmpeg-python/)
* [Tensorflow](https://pypi.org/project/tensorflow/)
* [Keras](https://pypi.org/project/keras/)
* [Scikit-learn](https://scikit-learn.org/)
  
## Contact Information
In case of any enquiry, question or collaboration opportunities, kindly reach out to me at:
* Email: [arko.g96@gmail.com](mailto:arko.g96@gmail.com)
* LinkedIn: [Arka Ghosh](https://www.linkedin.com/in/llarkaghoshll/)

## Citation

If you find the resources within this repository helpful, kindly cite this using: 
```
@inproceedings{das2020urban,
  title={Urban sound classification using convolutional neural network and long short term memory based on multiple features},
  author={Das, Joy Krishan and Ghosh, Arka and Pal, Abhijit Kumar and Dutta, Sumit and Chakrabarty, Amitabha},
  booktitle={2020 Fourth International Conference On Intelligent Computing in Data Sciences (ICDS)},
  pages={1--9},
  year={2020},
  organization={IEEE}
}
```


