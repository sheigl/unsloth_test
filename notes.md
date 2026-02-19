uv pip install setuptools
uv pip install unsloth unsloth-zoo
uv pip install --upgrade --pre torch torchaudio torchvision --index-url https://download.pytorch.org/whl/nightly/xpu
uv pip install -U --index-url https://aiinfra.pkgs.visualstudio.com/PublicPackages/_packaging/Triton-Nightly/pypi/simple/ triton-nightly
uv pip install intel-extension-for-pytorch==2.8.10+xpu --extra-index-url https://pytorch-extension.intel.com/release-whl/stable/xpu/us

uv pip install torch==2.8.0 torchvision==0.23.0 torchaudio==2.8.0 --index-url https://download.pytorch.org/whl/xpu

/home/sheigl/code/unsloth_test/.venv/lib/python3.11/site-packages/unsloth/kernels/moe/grouped_gemm/interface.py
gpu_supports_tma = False if torch.xpu else torch.cuda.get_device_capability()[0] >= 9