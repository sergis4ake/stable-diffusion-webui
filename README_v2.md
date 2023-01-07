# Installation on Linux

 1. Create conda env with "sd" as name
 2. Activate environment
 3. Install pytorch and cuda in the new environment (here)[https://pytorch.org/get-started/locally/]
 4. `$ conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia`
 5. Install xformers for the recent PyTorch installation: 
   - `git clone https://github.com/facebookresearch/xformers`
   - `pip install ninja` - for speed up the following build
   - `pip install -v -U git+https://github.com/facebookresearch/xformers.git@main#egg=xformers`
 6. Check `xformers` installation: `python -m xformers.info`
 7. Once `xformers` has been installed, add `--xformers` as argument to starter webui, in the `webui.sh`

