# pixel-perfect-sfm-Demo

- Provide a demo of using Pixel-Perfect Structure-from-Motion framework that improves the accuracy of Structure-from-Motion(SfM) as presented in the paper [Pixel-Perfect Structure-from-Motion](https://arxiv.org/abs/2108.08291)

  ## With pixsfm, you can:

        - reconstruct and refine a scene using hloc, from scratch or with given camera poses
        - localize and refine new query images using hloc
        - run the keypoint or bundle adjustments on a COLMAP database or 3D model
        - evaluate the refinement with new dense or sparse features on the ETH3D dataset

  ## Installation

  pixsfm requires Python >=3.6, GCC >=6.1, and COLMAP 3.8 installed from source. (requirements.txt)

  [Checkout Installation Section](https://github.com/cvg/pixel-perfect-sfm?tab=readme-ov-file#installation)

  ```
  # install COLMAP following colmap.github.io/install.html#build-from-source, tag 3.8
  sudo apt-get install libhdf5-dev
  git clone https://github.com/cvg/pixel-perfect-sfm --recursive
  cd pixel-perfect-sfm
  pip install -r requirements.txt
  ```

  To use other local features besides SIFT via COLMAP, we also require hloc:

  ```
  git clone --recursive https://github.com/cvg/Hierarchical-Localization/
  cd Hierarchical-Localization/
  pip install -e .
  ```

  Finally build and install the pixsfm package:

  ```
  pip install -e . # install pixsfm in develop mode
  ```

## References

- [pixel-perfect-sfm](https://github.com/cvg/pixel-perfect-sfm)
- [Dataset](https://documents.epfl.ch/groups/c/cv/cvlab-unit/www/data/multiview/fountain_dense.html)
