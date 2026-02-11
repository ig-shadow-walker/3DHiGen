# Stable3DGen

## Installation
Clone the repo:
```bash
git clone --recursive https://github.com/ig-shadow-walker/3DHiGen.git
cd Stable3DGen
```

Create a conda environment (optional):
```bash
conda create -n stablex python=3.10
conda activate stablex
```

Install dependencies (CUDA 12.4 / cu124; replace `cu124` with your CUDA version if different):
```bash
# PyTorch with CUDA 12.4
pip install torch==2.4.0 torchvision==0.19.0 --index-url https://download.pytorch.org/whl/cu124
pip install spconv-cu124==2.3.8 xformers==0.0.27.post2
# other dependencies
pip install -r requirements.txt
```

## Local Demo 🤗
Run by:
```bash
python app.py
```

<!-- License -->
## License
The model and code of Stable3DGen are adapted from [**Trellis**](https://github.com/microsoft/TRELLIS), which are licensed under the [MIT License](LICENSE). While the original Trellis is MIT licensed, we have specifically removed its dependencies on certain NVIDIA libraries (kaolin, nvdiffrast, flexicube) to ensure this adapted version can be used commercially. Stable3DGen itself is distributed under the [MIT License](LICENSE).

## Citation
If you find this work helpful, please consider citing our paper:
```
@article{ye2025hi3dgen,
  title={Hi3DGen: High-fidelity 3D Geometry Generation from Images via Normal Bridging},
  author={Ye, Chongjie and Wu, Yushuang and Lu, Ziteng and Chang, Jiahao and Guo, Xiaoyang and Zhou, Jiaqing and Zhao, Hao and Han, Xiaoguang},
  journal={arXiv preprint arXiv:2503.22236}, 
  year={2025}
}
```
