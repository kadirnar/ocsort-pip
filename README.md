<div align="center">
<h2>
  OcSort-Pip: Packaged version of the OcSort repository  
</h2>
<h4>
    <img width="500" alt="teaser" src="doc/sort_video.gif">
</h4>
</div>

## <div align="center">Overview</div>

This repo is a packaged version of the [OcSort](https://github.com/noahcao/OC_SORT) algorithm.
### Installation
```
pip install ocsort
```

### Detection Model + OcSort 
```python
from ocsort.ocsort import OCSort

tracker = OCSort(args)
for image in images:
   dets = detector(image)
   online_targets = tracker.update(dets)
```
### Citation
```bibtex
@article{cao2022observation,
  title={Observation-Centric SORT: Rethinking SORT for Robust Multi-Object Tracking},
  author={Cao, Jinkun and Weng, Xinshuo and Khirodkar, Rawal and Pang, Jiangmiao and Kitani, Kris},
  journal={arXiv preprint arXiv:2203.14360},
  year={2022}
}
```
