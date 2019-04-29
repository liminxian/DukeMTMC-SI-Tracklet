# DukeMTMC-SI-Tracklet

DukeMTMC-SI-Tracklet [1] is an auto-detected tracklets subset of the [DukeMTMC](http://vision.cs.duke.edu/DukeMTMC/) tracking dataset [2] for tracklet-based person re-identification.

We built this new tracklet person re-id dataset as follows. We first deployed an efficient deep learning tracker that leverages a COCO+PASCAL trained SSD for pedestrian detection and an ImageNet trained Inception for person appearance matching. Applying this tracker to all DukeMTMC raw videos, we generated 19,135 person tracklets. Due to the inevitable detection and tracking errors caused by background clutters and visual ambiguity, these tracklets may present typical mistakes (e.g.ID switch) and corruptions (e.g. occlusion).

We finally obtained 12,647 person tracklets from 1,788 unique IDs. To match DukeMTMC-ReID and DukeMTMC-VideoReID, we set the same 702 training IDs with the remaining 1,086 people for performance test (missing 14 test IDs against DukeMTMC-ReID due to tracking failures).

### Dataset Offline
According to the request of Duke University, we have to take DukeMTMC-SI-Tracklet dataset offline. We are sorry about that.

### References
- [1] Minxian Li, Xiatian Zhu, Shaogang Gong. [Unsupervised Tracklet Person Re-Identification](http://www.eecs.qmul.ac.uk/~sgg/papers/LiEtAl_PAMI2019.pdf). TPAMI 2019.

- [2] Ergys Ristani, Francesco Solera, Roger S. Zou, Rita Cucchiara, Carlo Tomasi. [Performance Measures and a Data Set for Multi-Target, Multi-Camera Tracking](https://users.cs.duke.edu/~tomasi/papers/ristani/ristaniBmtt16.pdf). ECCVWS 2016.

**Please cite** the following two papers if this dataset helps your research.
```
@article{LiTPAMI2019,
 title={Unsupervised Tracklet Person Re-Identification},
 author = {Li, Minxian and Zhu, Xiatian and Gong, Shaogang},
 journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
 year={2019}
}

@inproceedings{ristani2016MTMC,
  title = {Performance Measures and a Data Set for Multi-Target, Multi-Camera Tracking},
  author = {Ristani, Ergys and Solera, Francesco and Zou, Roger and Cucchiara, Rita and Tomasi, Carlo},
  booktitle = {European Conference on Computer Vision workshop on Benchmarking Multi-Target Tracking},
  year = {2016}
}
```
