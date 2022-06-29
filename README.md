### CycleGAN 코드 인용시 문구

<img src="https://github.com/sandokim/GANs/blob/main/images/CycleGAN_code_borrow.PNG" width="60%">

### 코드 스타일 및 아이디어 인용시 문구

<img src="https://github.com/sandokim/GANs/blob/main/images/Code_borrow_citation.PNG" width="80%">

### Dataset Experiment / Reference

We conduct quantitative experiments in different settings on front face→profile, Cityscapes [9], Google Map [23], horse→zebra translations. For face→profile, we aim to simulate the real-world application, in which we do not have any paired training identities from source to target but evaluate the performance on the held-out front and profile faces with the paired identities. The Cityscapes and Google Map datasets contain paired images in the training datasets, but all the models are trained in an unpaired manner and also tested on paired held-out testing set.s Additionally, we also test the model the on the popular horse→zebra where paired data are not available.

* Cityscapres <--> Google Map (Paired)
* face --> profile (Unpaired)
* horse --> zebra (Unpaire)

[9] Marius Cordts, Mohamed Omran, Sebastian Ramos, Timo Rehfeld, Markus Enzweiler, Rodrigo Benenson, Uwe Franke, Stefan Roth, and Bernt Schiele. The cityscapes dataset for semantic urban scene understanding. In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), June 2016. 5, 7

[23] Phillip Isola, Jun-Yan Zhu, Tinghui Zhou, and Alexei A Efros. Image-to-image translation with conditional adversarial networks. CVPR, 2017. 2, 5, 7

#### CycleGAN Debugging

Error : Could not connect to Visdom server. 

start the visdom server before starting the training

```python
python -m visdom.server
```

