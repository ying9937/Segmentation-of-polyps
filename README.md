# 息肉分割

## 		1.数据相关说明：

本研究的训练集和测试集以及模型相关权重（300轮以内的最佳权重）可以在该链接下载：https://drive.google.com/drive/folders/1scOMQk3PPxkKcLRNLMJrHR_1NpZOsvRV?usp=sharing

你可以使用Sample-dataset.h5中的简单数据跑通代码

## 		2.文件相关说明：

以下是code文件夹目录下文件和说明：

	│  How to use h5 files.ipynb  （h5文件使用方法）
	|  Sample-dataset.h5（样例数据）
	│  The random numbers partition Train and Val.ipynb（从训练集划分验证集）
	│  Train.txt（划分出的训练集）
	│  Val.txt（划分出的验证集）
	│
	├─Deep learning Mode（深度学习模型文件夹）
	│      FPN+V3.ipynb（FPN+V3模型代码）
	│      Linknet+V3.ipynb（Linknet+V3模型代码）
	│      PraNet.ipynb（PraNet模型代码）
	│      PSPnet+V3.ipynb（PSPnet+V3模型代码）
	│      SegNet-VGG.ipynb（SegNet-VGG模型代码）
	│      SegNet.ipynb（SegNet模型代码）
	│      U-net++.ipynb（U-net++模型代码）
	│      U-net+V3.ipynb（U-net+V3模型代码）
	│
	└─Digital Image Methods（数字图像增强技术方法文件夹）
	├─1.Edge detection（边缘检测技术）
	│      1. img+edge Enhancing images.ipynb（边缘图像+原始图像得到增强后图像的代码）
	│      1.BHPF (Extract edges in batches).ipynb（巴特沃斯高通滤波器获取边缘图像的代码）
	│      1.Canny (Extract edges in batches).ipynb（Canny算子获取边缘图像的代码）
	│      1.GHPF (Extract edges in batches).ipynb（高斯高通滤波器获取边缘图像的代码）
	│      1.IHPF (Extract edges in batches).ipynb（理想高通滤波器算子获取边缘图像的代码）
	│      1.Marr (Extract edges in batches).ipynb（Marr 算子获取边缘图像的代码）
	│      1.Prewitt (Extract edges in batches).ipynb（Prewitt 算子获取边缘图像的代码）
	│      1.Roberts (Extract edges in batches).ipynb（Roberts 算子获取边缘图像的代码）
	│      1.Sobel (Extract edges in batches).ipynb（Sobel 算子获取边缘图像的代码）
	│
	├─2.Highlight repair（高光修复技术）
	│      2.Highlight repair(Dynamic threshold percentage+FMM).ipynb（百分比动态阈值+FMM技术修复高光的代码）
	│      2.Highlight repair(Dynamic threshold percentage+NS).ipynb（百分比动态阈值+NS技术修复高光的代码）
	│      2.Highlight repair(Dynamic threshold statistics+FMM).ipynb.ipynb（统计动态阈值+FMM技术修复高光的代码）
	│      2.Highlight repair(Fixed threshold+FMM).ipynb（固定阈值+FMM技术修复高光的代码）
	│      2.Highlight repair(Fixed threshold+NS).ipynb（固定阈值+NS技术修复高光的代码）
	│
	└─3.Image channel（图像通道转化技术）
	        3.Image channel transformation(RGB to CMY).ipynb（RGB图像通道转CMY图像通道的代码）
	        3.Image channel transformation(RGB to HSI).ipynb（RGB图像通道转HSI图像通道的代码）
	        3.Image channel transformation(RGB to YIQ).ipynb（RGB图像通道转YIQ图像通道的代码）

## 3.相关python包的版本说明：

Windows：

```

(tf26) C:\Users\w>conda list
# packages in environment at C:\Users\w\.conda\envs\tf26:
#
# Name                    Version                   Build  Channel
absl-py                   2.1.0                    pypi_0    pypi
anyio                     4.2.0            py38haa95532_0
argon2-cffi               21.3.0             pyhd3eb1b0_0
argon2-cffi-bindings      21.2.0           py38h2bbff1b_0
arrow                     1.3.0                    pypi_0    pypi
asttokens                 2.0.5              pyhd3eb1b0_0
astunparse                1.6.3                    pypi_0    pypi
async-lru                 2.0.4            py38haa95532_0
attrs                     23.1.0           py38haa95532_0
babel                     2.11.0           py38haa95532_0
backcall                  0.2.0              pyhd3eb1b0_0
beautifulsoup4            4.12.2           py38haa95532_0
bleach                    4.1.0              pyhd3eb1b0_0
brotli-python             1.0.9            py38hd77b12b_7
ca-certificates           2023.12.12           haa95532_0
cachetools                5.3.3                    pypi_0    pypi
certifi                   2024.2.2         py38haa95532_0
cffi                      1.16.0           py38h2bbff1b_0
charset-normalizer        2.0.4              pyhd3eb1b0_0
colorama                  0.4.6            py38haa95532_0
comm                      0.1.2            py38haa95532_0
contourpy                 1.1.1                    pypi_0    pypi
cudatoolkit               11.3.1               h59b6b97_2
cudnn                     8.2.1                cuda11.3_0
cycler                    0.12.1                   pypi_0    pypi
debugpy                   1.6.7            py38hd77b12b_0
decorator                 5.1.1              pyhd3eb1b0_0
defusedxml                0.7.1              pyhd3eb1b0_0
efficientnet              1.0.0                    pypi_0    pypi
exceptiongroup            1.2.0            py38haa95532_0
executing                 0.8.3              pyhd3eb1b0_0
flatbuffers               1.12                     pypi_0    pypi
fonttools                 4.49.0                   pypi_0    pypi
fqdn                      1.5.1                    pypi_0    pypi
gast                      0.4.0                    pypi_0    pypi
google-auth               2.28.1                   pypi_0    pypi
google-auth-oauthlib      0.4.6                    pypi_0    pypi
google-pasta              0.2.0                    pypi_0    pypi
grpcio                    1.62.0                   pypi_0    pypi
h5py                      3.10.0                   pypi_0    pypi
icu                       73.1                 h6c2663c_0
idna                      3.4              py38haa95532_0
image-classifiers         1.0.0                    pypi_0    pypi
imageio                   2.34.0                   pypi_0    pypi
importlib-metadata        7.0.1            py38haa95532_0
importlib_metadata        7.0.1                hd3eb1b0_0
importlib_resources       6.1.1            py38haa95532_1
ipykernel                 6.28.0           py38haa95532_0
ipython                   8.12.2           py38haa95532_0
ipywidgets                8.0.4            py38haa95532_0
isoduration               20.11.0                  pypi_0    pypi
jedi                      0.18.1           py38haa95532_1
jinja2                    3.1.3            py38haa95532_0
joblib                    1.4.2                    pypi_0    pypi
jpeg                      9e                   h2bbff1b_1
json5                     0.9.6              pyhd3eb1b0_0
jsonpointer               3.0.0                    pypi_0    pypi
jsonschema                4.19.2           py38haa95532_0
jsonschema-specifications 2023.7.1         py38haa95532_0
jupyter                   1.0.0            py38haa95532_9
jupyter-lsp               2.2.0            py38haa95532_0
jupyter_client            8.6.0            py38haa95532_0
jupyter_console           6.6.3            py38haa95532_0
jupyter_core              5.5.0            py38haa95532_0
jupyter_events            0.8.0            py38haa95532_0
jupyter_server            2.10.0           py38haa95532_0
jupyter_server_terminals  0.4.4            py38haa95532_1
jupyterlab                4.0.11           py38haa95532_0
jupyterlab_pygments       0.1.2                      py_0
jupyterlab_server         2.25.1           py38haa95532_0
jupyterlab_widgets        3.0.9            py38haa95532_0
jupyterthemes             0.20.0                   pypi_0    pypi
keras                     2.9.0                    pypi_0    pypi
keras-applications        1.0.8                    pypi_0    pypi
keras-preprocessing       1.1.2                    pypi_0    pypi
kiwisolver                1.4.5                    pypi_0    pypi
krb5                      1.20.1               h5b6d351_0
lazy-loader               0.3                      pypi_0    pypi
lesscpy                   0.15.1                   pypi_0    pypi
libclang                  16.0.6                   pypi_0    pypi
libclang13                14.0.6          default_h8e68704_1
libffi                    3.4.4                hd77b12b_0
libpng                    1.6.39               h8cc25b3_0
libpq                     12.17                h906ac69_0
libsodium                 1.0.18               h62dcd97_0
lz4-c                     1.9.4                h2bbff1b_0
markdown                  3.5.2                    pypi_0    pypi
markupsafe                2.1.3            py38h2bbff1b_0
matplotlib                3.7.5                    pypi_0    pypi
matplotlib-inline         0.1.6            py38haa95532_0
mistune                   2.0.4            py38haa95532_0
nbclient                  0.8.0            py38haa95532_0
nbconvert                 7.10.0           py38haa95532_0
nbformat                  5.9.2            py38haa95532_0
nest-asyncio              1.6.0            py38haa95532_0
networkx                  3.1                      pypi_0    pypi
notebook                  7.0.8            py38haa95532_0
notebook-shim             0.2.3            py38haa95532_0
numpy                     1.24.4                   pypi_0    pypi
oauthlib                  3.2.2                    pypi_0    pypi
opencv-python             4.9.0.80                 pypi_0    pypi
openssl                   3.0.13               h2bbff1b_0
opt-einsum                3.3.0                    pypi_0    pypi
overrides                 7.4.0            py38haa95532_0
packaging                 23.1             py38haa95532_0
pandocfilters             1.5.0              pyhd3eb1b0_0
parso                     0.8.3              pyhd3eb1b0_0
pickleshare               0.7.5           pyhd3eb1b0_1003
pillow                    10.2.0                   pypi_0    pypi
pip                       23.3.1           py38haa95532_0
pkgutil-resolve-name      1.3.10           py38haa95532_1
platformdirs              3.10.0           py38haa95532_0
ply                       3.11                     py38_0
prometheus_client         0.14.1           py38haa95532_0
prompt-toolkit            3.0.43           py38haa95532_0
prompt_toolkit            3.0.43               hd3eb1b0_0
protobuf                  3.19.6                   pypi_0    pypi
psutil                    5.9.0            py38h2bbff1b_0
pure_eval                 0.2.2              pyhd3eb1b0_0
pyasn1                    0.5.1                    pypi_0    pypi
pyasn1-modules            0.3.0                    pypi_0    pypi
pycparser                 2.21               pyhd3eb1b0_0
pydot                     4.0.0                    pypi_0    pypi
pygments                  2.15.1           py38haa95532_1
pyparsing                 3.1.1                    pypi_0    pypi
pyqt                      5.15.10          py38hd77b12b_0
pyqt5-sip                 12.13.0          py38h2bbff1b_0
pysocks                   1.7.1            py38haa95532_0
python                    3.8.18               h1aa4202_0
python-dateutil           2.8.2              pyhd3eb1b0_0
python-fastjsonschema     2.16.2           py38haa95532_0
python-json-logger        2.0.7            py38haa95532_0
pytz                      2023.3.post1     py38haa95532_0
pywavelets                1.4.1                    pypi_0    pypi
pywin32                   305              py38h2bbff1b_0
pywinpty                  2.0.10           py38h5da7b33_0
pyyaml                    6.0.1            py38h2bbff1b_0
pyzmq                     25.1.2           py38hd77b12b_0
qt-main                   5.15.2              h19c9488_10
qtconsole                 5.5.0            py38haa95532_0
qtpy                      2.4.1            py38haa95532_0
referencing               0.30.2           py38haa95532_0
requests                  2.31.0           py38haa95532_1
requests-oauthlib         1.3.1                    pypi_0    pypi
rfc3339-validator         0.1.4            py38haa95532_0
rfc3986-validator         0.1.1            py38haa95532_0
rpds-py                   0.10.6           py38h062c2fa_0
rsa                       4.9                      pypi_0    pypi
scikit-image              0.21.0                   pypi_0    pypi
scikit-learn              1.3.2                    pypi_0    pypi
scipy                     1.10.1                   pypi_0    pypi
segmentation-models       1.0.1                    pypi_0    pypi
send2trash                1.8.2            py38haa95532_0
setuptools                68.2.2           py38haa95532_0
sip                       6.7.12           py38hd77b12b_0
six                       1.16.0             pyhd3eb1b0_1
sniffio                   1.3.0            py38haa95532_0
soupsieve                 2.5              py38haa95532_0
sqlite                    3.41.2               h2bbff1b_0
stack_data                0.2.0              pyhd3eb1b0_0
tensorboard               2.9.1                    pypi_0    pypi
tensorboard-data-server   0.6.1                    pypi_0    pypi
tensorboard-plugin-wit    1.8.1                    pypi_0    pypi
tensorflow-estimator      2.9.0                    pypi_0    pypi
tensorflow-gpu            2.9.0                    pypi_0    pypi
tensorflow-io-gcs-filesystem 0.31.0                   pypi_0    pypi
termcolor                 2.4.0                    pypi_0    pypi
terminado                 0.17.1           py38haa95532_0
threadpoolctl             3.5.0                    pypi_0    pypi
tifffile                  2023.7.10                pypi_0    pypi
tinycss2                  1.2.1            py38haa95532_0
tomli                     2.0.1            py38haa95532_0
tornado                   6.3.3            py38h2bbff1b_0
traitlets                 5.7.1            py38haa95532_0
types-python-dateutil     2.9.0.20241206           pypi_0    pypi
typing-extensions         4.9.0            py38haa95532_1
typing_extensions         4.9.0            py38haa95532_1
uri-template              1.3.0                    pypi_0    pypi
urllib3                   2.1.0            py38haa95532_1
vc                        14.2                 h21ff451_1
vs2015_runtime            14.27.29016          h5e58377_2
wcwidth                   0.2.5              pyhd3eb1b0_0
webcolors                 24.8.0                   pypi_0    pypi
webencodings              0.5.1                    py38_1
websocket-client          0.58.0           py38haa95532_4
werkzeug                  3.0.1                    pypi_0    pypi
wheel                     0.41.2           py38haa95532_0
widgetsnbextension        4.0.5            py38haa95532_0
win_inet_pton             1.1.0            py38haa95532_0
winpty                    0.4.3                         4
wrapt                     1.16.0                   pypi_0    pypi
xz                        5.4.5                h8cc25b3_0
yaml                      0.2.5                he774522_0
zeromq                    4.3.5                hd77b12b_0
zipp                      3.17.0           py38haa95532_0
zlib                      1.2.13               h8cc25b3_0
zstd                      1.5.5                hd43e919_0
```

Linux：其中SegNet-Simple.ipynb和SegNet.ipynb为linux环境，相关python包为：

```
(base) wujieyu@lthpc:~$ conda activate tf
(tf) wujieyu@lthpc:~$ conda list
# packages in environment at /data/wujieyu/anaconda3/envs/tf:
#
# Name                    Version                   Build  Channel
_libgcc_mutex             0.1                        main  
_openmp_mutex             5.1                       1_gnu  
absl-py                   2.1.0            py39h06a4308_0  
anyio                     4.9.0                    pypi_0    pypi
aom                       3.6.0                h6a678d5_0  
argon2-cffi               23.1.0                   pypi_0    pypi
argon2-cffi-bindings      21.2.0                   pypi_0    pypi
arrow                     1.3.0                    pypi_0    pypi
asttokens                 3.0.0                    pypi_0    pypi
astunparse                1.6.3                      py_0  
async-lru                 2.0.5                    pypi_0    pypi
attrs                     25.3.0                   pypi_0    pypi
babel                     2.17.0                   pypi_0    pypi
beautifulsoup4            4.13.4                   pypi_0    pypi
blas                      1.0                         mkl  
bleach                    6.2.0                    pypi_0    pypi
brotli-python             1.0.9            py39h6a678d5_9  
bzip2                     1.0.8                h4bc722e_7    conda-forge
c-ares                    1.19.1               h5eee18b_0  
ca-certificates           2025.4.26            hbd8a1cb_0    conda-forge
cairo                     1.16.0               hb05425b_5  
certifi                   2025.4.26          pyhd8ed1ab_0    conda-forge
cffi                      1.17.1                   pypi_0    pypi
charset-normalizer        3.3.2              pyhd3eb1b0_0  
comm                      0.2.2                    pypi_0    pypi
contourpy                 1.3.0                    pypi_0    pypi
cuda-crt-tools            12.4.131             h06a4308_0  
cuda-cudart               12.4.127             h99ab3db_0  
cuda-cudart_linux-64      12.4.127             hd681fbe_0  
cuda-cupti                12.4.127             h6a678d5_1  
cuda-nvcc-tools           12.4.131             h99ab3db_0  
cuda-nvrtc                12.4.127             h99ab3db_1  
cuda-nvtx                 12.4.127             h6a678d5_1  
cuda-nvvm-tools           12.4.131             h6a678d5_0  
cuda-version              12.4                 hbda6634_3  
cudnn                     9.1.1.17               cuda12_1  
cycler                    0.12.1                   pypi_0    pypi
cyrus-sasl                2.1.28               h52b45da_1  
dav1d                     1.2.1                hd590300_0    conda-forge
dbus                      1.13.18              hb2f20db_0  
debugpy                   1.8.14                   pypi_0    pypi
decorator                 5.2.1                    pypi_0    pypi
defusedxml                0.7.1                    pypi_0    pypi
efficientnet              1.0.0                    pypi_0    pypi
eigen                     3.4.0                h4bd325d_0    conda-forge
exceptiongroup            1.2.2                    pypi_0    pypi
executing                 2.2.0                    pypi_0    pypi
expat                     2.7.0                h5888daf_0    conda-forge
fastjsonschema            2.21.1                   pypi_0    pypi
ffmpeg                    6.1.1                h2a67f75_3  
flatbuffers               24.3.25              h6a678d5_0  
fontconfig                2.14.1               h55d465d_3  
fonttools                 4.57.0                   pypi_0    pypi
fqdn                      1.5.1                    pypi_0    pypi
freetype                  2.10.4               h0708190_1    conda-forge
gast                      0.5.3              pyhd3eb1b0_0  
giflib                    5.2.2                h5eee18b_0  
glib                      2.78.4               h6a678d5_0  
glib-tools                2.78.4               h6a678d5_0  
google-pasta              0.2.0              pyhd3eb1b0_0  
graphite2                 1.3.14               h295c915_1  
grpcio                    1.62.2           py39h6a678d5_0  
gst-plugins-base          1.14.1               h6a678d5_1  
gstreamer                 1.14.1               h5eee18b_1  
h11                       0.16.0                   pypi_0    pypi
h5py                      3.12.1           py39h5842655_1  
harfbuzz                  10.2.0               hf296adc_0  
hdf5                      1.14.5               h2b7332f_2  
httpcore                  1.0.9                    pypi_0    pypi
httpx                     0.28.1                   pypi_0    pypi
icu                       73.1                 h6a678d5_0  
idna                      3.7              py39h06a4308_0  
image-classifiers         1.0.0                    pypi_0    pypi
imageio                   2.37.0                   pypi_0    pypi
importlib-metadata        8.5.0            py39h06a4308_0  
importlib-resources       6.5.2                    pypi_0    pypi
intel-openmp              2023.1.0         hdb19cb5_46306  
ipykernel                 6.29.5                   pypi_0    pypi
ipython                   8.18.1                   pypi_0    pypi
ipywidgets                8.1.7                    pypi_0    pypi
isoduration               20.11.0                  pypi_0    pypi
jedi                      0.19.2                   pypi_0    pypi
jinja2                    3.1.6                    pypi_0    pypi
joblib                    1.5.1                    pypi_0    pypi
jpeg                      9e                   h5eee18b_3  
json5                     0.12.0                   pypi_0    pypi
jsonpointer               3.0.0                    pypi_0    pypi
jsonschema                4.23.0                   pypi_0    pypi
jsonschema-specifications 2025.4.1                 pypi_0    pypi
jupyter                   1.1.1                    pypi_0    pypi
jupyter-client            8.6.3                    pypi_0    pypi
jupyter-console           6.6.3                    pypi_0    pypi
jupyter-core              5.7.2                    pypi_0    pypi
jupyter-events            0.12.0                   pypi_0    pypi
jupyter-lsp               2.2.5                    pypi_0    pypi
jupyter-server            2.15.0                   pypi_0    pypi
jupyter-server-terminals  0.5.3                    pypi_0    pypi
jupyterlab                4.4.2                    pypi_0    pypi
jupyterlab-pygments       0.3.0                    pypi_0    pypi
jupyterlab-server         2.27.3                   pypi_0    pypi
jupyterlab-widgets        3.0.15                   pypi_0    pypi
keras                     3.6.0            py39h06a4308_0  
keras-applications        1.0.8                    pypi_0    pypi
keras-unet                0.1.2                    pypi_0    pypi
kiwisolver                1.4.7                    pypi_0    pypi
krb5                      1.20.1               h143b758_1  
lame                      3.100             h166bdaf_1003    conda-forge
lazy-loader               0.4                      pypi_0    pypi
ld_impl_linux-64          2.40                 h12ee557_0  
leptonica                 1.82.0               h42c8aad_2  
lerc                      4.0.0                h0aef613_1    conda-forge
libabseil                 20240116.2      cxx17_h6a678d5_0  
libarchive                3.7.7                hfab0078_0  
libclang                  14.0.6          default_hc6dbbc7_2  
libclang13                14.0.6          default_he11475f_2  
libcublas                 12.4.5.8             h99ab3db_1  
libcufft                  11.2.1.3             h99ab3db_1  
libcups                   2.4.2                h2d74bed_1  
libcurand                 10.3.5.147           h99ab3db_1  
libcurl                   8.12.1               hc9e6f67_0  
libcusolver               11.6.1.9             h99ab3db_1  
libcusparse               12.3.1.170           h99ab3db_1  
libdeflate                1.22                 hb9d3cd8_0    conda-forge
libedit                   3.1.20230828         h5eee18b_0  
libev                     4.33                 h7f8727e_1  
libexpat                  2.7.0                h5888daf_0    conda-forge
libffi                    3.4.4                h6a678d5_1  
libgcc                    15.1.0               h767d61c_2    conda-forge
libgcc-ng                 15.1.0               h69a702a_2    conda-forge
libgfortran-ng            11.2.0               h00389a5_1  
libgfortran5              11.2.0               h1234567_1  
libglib                   2.78.4               hdc74915_0  
libgomp                   15.1.0               h767d61c_2    conda-forge
libgrpc                   1.62.2               h2d74bed_0  
libiconv                  1.18                 h4ce23a2_1    conda-forge
libllvm14                 14.0.6               hecde1de_4  
libnghttp2                1.57.0               h2d74bed_0  
libnvjitlink              12.4.127             h99ab3db_1  
libogg                    1.3.5                hd0c01bc_1    conda-forge
libopus                   1.5.2                hd0c01bc_0    conda-forge
libpng                    1.6.39               h5eee18b_0  
libpq                     17.4                 hdbd6064_0  
libprotobuf               4.25.3               he621ea3_0  
libssh2                   1.11.1               h251f7ec_0  
libstdcxx                 15.1.0               h8f9b012_2    conda-forge
libstdcxx-ng              11.2.0               h1234567_1  
libtheora                 1.1.1             h4ab18f5_1006    conda-forge
libtiff                   4.5.1                hffd6297_1  
libuuid                   1.41.5               h5eee18b_0  
libvorbis                 1.3.7                h9c3ff4c_0    conda-forge
libvpx                    1.13.1               h6a678d5_0  
libwebp                   1.3.2                h11a3e52_0  
libwebp-base              1.3.2                hd590300_1    conda-forge
libxcb                    1.17.0               h8a09558_0    conda-forge
libxkbcommon              1.9.2                h65c71a3_0    conda-forge
libxml2                   2.13.8               hfdd30dd_0  
lz4-c                     1.9.4                h6a678d5_1  
markdown                  3.8              py39h06a4308_0  
markdown-it-py            2.2.0            py39h06a4308_1  
markupsafe                3.0.2            py39h5eee18b_0  
matplotlib                3.9.4                    pypi_0    pypi
matplotlib-inline         0.1.7                    pypi_0    pypi
mdurl                     0.1.0            py39h06a4308_0  
mistune                   3.1.3                    pypi_0    pypi
mkl                       2023.1.0         h213fc3f_46344  
mkl-service               2.4.0            py39h5eee18b_2  
mkl_fft                   1.3.11           py39h5eee18b_0  
mkl_random                1.2.8            py39h1128e8f_0  
ml_dtypes                 0.4.1            py39hc74f9fe_0  
mysql                     8.4.0                h29a9f33_1  
namex                     0.0.7            py39h06a4308_0  
nbclient                  0.10.2                   pypi_0    pypi
nbconvert                 7.16.6                   pypi_0    pypi
nbformat                  5.10.4                   pypi_0    pypi
nccl                      2.21.5.1             ha515578_0  
ncurses                   6.4                  h6a678d5_0  
nest-asyncio              1.6.0                    pypi_0    pypi
networkx                  3.2.1                    pypi_0    pypi
notebook                  7.4.2                    pypi_0    pypi
notebook-shim             0.2.4                    pypi_0    pypi
numpy                     1.26.4           py39h5f9d8c6_0  
numpy-base                1.26.4           py39hb5e798b_0  
opencv                    4.10.0           py39h2484693_2  
openh264                  2.1.1                h780b84a_0    conda-forge
openjpeg                  2.5.2                he7f1fd0_0  
openldap                  2.6.4                h42fbc30_0  
openssl                   3.5.0                h7b32b05_1    conda-forge
opt_einsum                3.3.0              pyhd3eb1b0_1  
optree                    0.14.1           py39hdb19cb5_0  
overrides                 7.7.0                    pypi_0    pypi
packaging                 24.2             py39h06a4308_0  
pandocfilters             1.5.1                    pypi_0    pypi
parso                     0.8.4                    pypi_0    pypi
pcre2                     10.42                hebb0a14_1  
pexpect                   4.9.0                    pypi_0    pypi
pillow                    11.2.1                   pypi_0    pypi
pip                       25.1               pyhc872135_2  
pixman                    0.46.0               h29eaf8c_0    conda-forge
platformdirs              4.3.8                    pypi_0    pypi
prometheus-client         0.21.1                   pypi_0    pypi
prompt-toolkit            3.0.51                   pypi_0    pypi
protobuf                  4.25.3           py39he36ed58_1  
psutil                    7.0.0                    pypi_0    pypi
pthread-stubs             0.4               hb9d3cd8_1002    conda-forge
ptyprocess                0.7.0                    pypi_0    pypi
pure-eval                 0.2.3                    pypi_0    pypi
pycparser                 2.22                     pypi_0    pypi
pygments                  2.19.1           py39h06a4308_0  
pyparsing                 3.2.3                    pypi_0    pypi
pysocks                   1.7.1            py39h06a4308_0  
python                    3.9.21               he870216_1  
python-dateutil           2.9.0.post0              pypi_0    pypi
python-flatbuffers        24.3.25          py39h06a4308_0  
python-json-logger        3.3.0                    pypi_0    pypi
pyyaml                    6.0.2                    pypi_0    pypi
pyzmq                     26.4.0                   pypi_0    pypi
qt-main                   5.15.2              hb6262e9_12  
re2                       2022.04.01           h295c915_0  
readline                  8.2                  h5eee18b_0  
referencing               0.36.2                   pypi_0    pypi
requests                  2.32.3           py39h06a4308_1  
rfc3339-validator         0.1.4                    pypi_0    pypi
rfc3986-validator         0.1.1                    pypi_0    pypi
rich                      13.9.4           py39h06a4308_0  
rpds-py                   0.24.0                   pypi_0    pypi
scikit-image              0.24.0                   pypi_0    pypi
scikit-learn              1.6.1                    pypi_0    pypi
scipy                     1.13.1                   pypi_0    pypi
segmentation-models       1.0.1                    pypi_0    pypi
send2trash                1.8.3                    pypi_0    pypi
setuptools                78.1.1           py39h06a4308_0  
six                       1.17.0           py39h06a4308_0  
snappy                    1.2.1                h6a678d5_0  
sniffio                   1.3.1                    pypi_0    pypi
soupsieve                 2.7                      pypi_0    pypi
sqlite                    3.45.3               h5eee18b_0  
stack-data                0.6.3                    pypi_0    pypi
tbb                       2021.8.0             hdb19cb5_0  
tensorboard               2.17.0           py39h06a4308_0  
tensorboard-data-server   0.7.0            py39h52d8a92_1  
tensorflow                2.17.0          cuda124py39ha1f05a4_200  
tensorflow-base           2.17.0          cuda124py39h3b6feb8_200  
tensorflow-estimator      2.17.0          cuda124py39he5efd2c_200  
tensorflow-gpu            2.17.0          cuda124py39hd65659d_200  
termcolor                 2.1.0            py39h06a4308_0  
terminado                 0.18.1                   pypi_0    pypi
tesseract                 5.2.0                h6a678d5_2  
threadpoolctl             3.6.0                    pypi_0    pypi
tifffile                  2024.8.30                pypi_0    pypi
tinycss2                  1.4.0                    pypi_0    pypi
tk                        8.6.14               h39e8969_0  
tomli                     2.2.1                    pypi_0    pypi
tornado                   6.4.2                    pypi_0    pypi
traitlets                 5.14.3                   pypi_0    pypi
types-python-dateutil     2.9.0.20241206           pypi_0    pypi
typing-extensions         4.12.2           py39h06a4308_0  
typing_extensions         4.12.2           py39h06a4308_0  
tzdata                    2025b                h04d1e81_0  
uri-template              1.3.0                    pypi_0    pypi
urllib3                   2.3.0            py39h06a4308_0  
wcwidth                   0.2.13                   pypi_0    pypi
webcolors                 24.11.1                  pypi_0    pypi
webencodings              0.5.1                    pypi_0    pypi
websocket-client          1.8.0                    pypi_0    pypi
werkzeug                  3.1.3            py39h06a4308_0  
wheel                     0.45.1           py39h06a4308_0  
widgetsnbextension        4.0.14                   pypi_0    pypi
wrapt                     1.17.0           py39h5eee18b_0  
xkeyboard-config          2.44                 hb9d3cd8_0    conda-forge
xorg-libx11               1.8.12               h4f16b4b_0    conda-forge
xorg-libxau               1.0.12               hb9d3cd8_0    conda-forge
xorg-libxdmcp             1.1.5                hb9d3cd8_0    conda-forge
xz                        5.6.4                h5eee18b_1  
zipp                      3.21.0           py39h06a4308_0  
zlib                      1.2.13               h5eee18b_1  
zstd                      1.5.6                hc292b87_0  
```



# Segmentation-of-polyps

## 1.Data Related Notes：

The training and test sets for this study and the weights associated with the model (the best weights within 300 rounds) can be downloaded at:https://drive.google.com/drive/folders/1scOMQk3PPxkKcLRNLMJrHR_1NpZOsvRV?usp=sharing

You can run the code using the simple data in Sample-dataset.h5

## 2.Notes on the file:

Here are the files and instructions in the code folder:

	│  How to use h5 files.ipynb  （The usage method of h5 files）
	|  Sample-dataset.h5（Sample data）
	│  The random numbers partition Train and Val.ipynb（Split the validation set from the training set）
	│  Train.txt（The split training set）
	│  Val.txt（The split validation set）
	│
	├─Deep learning Mode（Deep Learning Models folder）
	│      FPN+V3.ipynb（Code for the FPN+V3 model）
	│      Linknet+V3.ipynb（Code for the Linknet+V3 model）
	│      PraNet.ipynb（Code for the PraNet model）
	│      PSPnet+V3.ipynb（Code for the PSPnet+V3 model）
	│      SegNet-VGG.ipynb（Code for the SegNet-VGG model）
	│      SegNet.ipynb（Code for the SegNet model）
	│      U-net++.ipynb（Code for the U-net++ model）
	│      U-net+V3.ipynb（Code for the U-net+V3 model）
	│
	└─Digital Image Methods（Digital image enhancement Techniques methods folder）
	├─1.Edge detection（Edge detection technology）
	│      1. img+edge Enhancing images.ipynb（Edge image + Code for the enhanced image obtained from the original image）
	│      1.BHPF (Extract edges in batches).ipynb（Butterworth high-pass filter obtains the code of the edge image）
	│      1.Canny (Extract edges in batches).ipynb（The Canny operator obtains the code of the edge image）
	│      1.GHPF (Extract edges in batches).ipynb（Gaussian high-pass filter obtains the code of the edge image）
	│      1.IHPF (Extract edges in batches).ipynb（Code for obtaining the edge image for the ideal high-pass filter operator）
	│      1.Marr (Extract edges in batches).ipynb（Marr operator obtains the code of the edge image）
	│      1.Prewitt (Extract edges in batches).ipynb（Prewitt operator obtains the code of the edge image）
	│      1.Roberts (Extract edges in batches).ipynb（Roberts operator obtains the code of the edge image）
	│      1.Sobel (Extract edges in batches).ipynb（Sobel operator gets the code of the edge image）
	│
	├─2.Highlight repair（Highlight repair technique）
	│      2.Highlight repair(Dynamic threshold percentage+FMM).ipynb（Percentage dynamic threshold +FMM technique fixes the code for highlights）
	│      2.Highlight repair(Dynamic threshold percentage+NS).ipynb（Percentage dynamic threshold +NS technique fixes the code for highlights）
	│      2.Highlight repair(Dynamic threshold statistics+FMM).ipynb.ipynb（Code with statistical dynamic thresholding +FMM technique for fixing highlights）
	│      2.Highlight repair(Fixed threshold+FMM).ipynb（Code with fixed threshold +FMM technique to fix highlights）
	│      2.Highlight repair(Fixed threshold+NS).ipynb（Fixed threshold +NS technique fixes the code for highlights）
	│
	└─3.Image channel（Image channel conversion techniques）
	        3.Image channel transformation(RGB to CMY).ipynb（RGB image channel to CMY image channel code）
	        3.Image channel transformation(RGB to HSI).ipynb（RGB image channel to HSI image channel code）
	        3.Image channel transformation(RGB to YIQ).ipynb（RGB image channel to YIQ image channel code）

## 3.Version notes for python packages:

Windows：

```
(tf26) C:\Users\w>conda list
# packages in environment at C:\Users\w\.conda\envs\tf26:
#
# Name                    Version                   Build  Channel
absl-py                   2.1.0                    pypi_0    pypi
anyio                     4.2.0            py38haa95532_0
argon2-cffi               21.3.0             pyhd3eb1b0_0
argon2-cffi-bindings      21.2.0           py38h2bbff1b_0
arrow                     1.3.0                    pypi_0    pypi
asttokens                 2.0.5              pyhd3eb1b0_0
astunparse                1.6.3                    pypi_0    pypi
async-lru                 2.0.4            py38haa95532_0
attrs                     23.1.0           py38haa95532_0
babel                     2.11.0           py38haa95532_0
backcall                  0.2.0              pyhd3eb1b0_0
beautifulsoup4            4.12.2           py38haa95532_0
bleach                    4.1.0              pyhd3eb1b0_0
brotli-python             1.0.9            py38hd77b12b_7
ca-certificates           2023.12.12           haa95532_0
cachetools                5.3.3                    pypi_0    pypi
certifi                   2024.2.2         py38haa95532_0
cffi                      1.16.0           py38h2bbff1b_0
charset-normalizer        2.0.4              pyhd3eb1b0_0
colorama                  0.4.6            py38haa95532_0
comm                      0.1.2            py38haa95532_0
contourpy                 1.1.1                    pypi_0    pypi
cudatoolkit               11.3.1               h59b6b97_2
cudnn                     8.2.1                cuda11.3_0
cycler                    0.12.1                   pypi_0    pypi
debugpy                   1.6.7            py38hd77b12b_0
decorator                 5.1.1              pyhd3eb1b0_0
defusedxml                0.7.1              pyhd3eb1b0_0
efficientnet              1.0.0                    pypi_0    pypi
exceptiongroup            1.2.0            py38haa95532_0
executing                 0.8.3              pyhd3eb1b0_0
flatbuffers               1.12                     pypi_0    pypi
fonttools                 4.49.0                   pypi_0    pypi
fqdn                      1.5.1                    pypi_0    pypi
gast                      0.4.0                    pypi_0    pypi
google-auth               2.28.1                   pypi_0    pypi
google-auth-oauthlib      0.4.6                    pypi_0    pypi
google-pasta              0.2.0                    pypi_0    pypi
grpcio                    1.62.0                   pypi_0    pypi
h5py                      3.10.0                   pypi_0    pypi
icu                       73.1                 h6c2663c_0
idna                      3.4              py38haa95532_0
image-classifiers         1.0.0                    pypi_0    pypi
imageio                   2.34.0                   pypi_0    pypi
importlib-metadata        7.0.1            py38haa95532_0
importlib_metadata        7.0.1                hd3eb1b0_0
importlib_resources       6.1.1            py38haa95532_1
ipykernel                 6.28.0           py38haa95532_0
ipython                   8.12.2           py38haa95532_0
ipywidgets                8.0.4            py38haa95532_0
isoduration               20.11.0                  pypi_0    pypi
jedi                      0.18.1           py38haa95532_1
jinja2                    3.1.3            py38haa95532_0
joblib                    1.4.2                    pypi_0    pypi
jpeg                      9e                   h2bbff1b_1
json5                     0.9.6              pyhd3eb1b0_0
jsonpointer               3.0.0                    pypi_0    pypi
jsonschema                4.19.2           py38haa95532_0
jsonschema-specifications 2023.7.1         py38haa95532_0
jupyter                   1.0.0            py38haa95532_9
jupyter-lsp               2.2.0            py38haa95532_0
jupyter_client            8.6.0            py38haa95532_0
jupyter_console           6.6.3            py38haa95532_0
jupyter_core              5.5.0            py38haa95532_0
jupyter_events            0.8.0            py38haa95532_0
jupyter_server            2.10.0           py38haa95532_0
jupyter_server_terminals  0.4.4            py38haa95532_1
jupyterlab                4.0.11           py38haa95532_0
jupyterlab_pygments       0.1.2                      py_0
jupyterlab_server         2.25.1           py38haa95532_0
jupyterlab_widgets        3.0.9            py38haa95532_0
jupyterthemes             0.20.0                   pypi_0    pypi
keras                     2.9.0                    pypi_0    pypi
keras-applications        1.0.8                    pypi_0    pypi
keras-preprocessing       1.1.2                    pypi_0    pypi
kiwisolver                1.4.5                    pypi_0    pypi
krb5                      1.20.1               h5b6d351_0
lazy-loader               0.3                      pypi_0    pypi
lesscpy                   0.15.1                   pypi_0    pypi
libclang                  16.0.6                   pypi_0    pypi
libclang13                14.0.6          default_h8e68704_1
libffi                    3.4.4                hd77b12b_0
libpng                    1.6.39               h8cc25b3_0
libpq                     12.17                h906ac69_0
libsodium                 1.0.18               h62dcd97_0
lz4-c                     1.9.4                h2bbff1b_0
markdown                  3.5.2                    pypi_0    pypi
markupsafe                2.1.3            py38h2bbff1b_0
matplotlib                3.7.5                    pypi_0    pypi
matplotlib-inline         0.1.6            py38haa95532_0
mistune                   2.0.4            py38haa95532_0
nbclient                  0.8.0            py38haa95532_0
nbconvert                 7.10.0           py38haa95532_0
nbformat                  5.9.2            py38haa95532_0
nest-asyncio              1.6.0            py38haa95532_0
networkx                  3.1                      pypi_0    pypi
notebook                  7.0.8            py38haa95532_0
notebook-shim             0.2.3            py38haa95532_0
numpy                     1.24.4                   pypi_0    pypi
oauthlib                  3.2.2                    pypi_0    pypi
opencv-python             4.9.0.80                 pypi_0    pypi
openssl                   3.0.13               h2bbff1b_0
opt-einsum                3.3.0                    pypi_0    pypi
overrides                 7.4.0            py38haa95532_0
packaging                 23.1             py38haa95532_0
pandocfilters             1.5.0              pyhd3eb1b0_0
parso                     0.8.3              pyhd3eb1b0_0
pickleshare               0.7.5           pyhd3eb1b0_1003
pillow                    10.2.0                   pypi_0    pypi
pip                       23.3.1           py38haa95532_0
pkgutil-resolve-name      1.3.10           py38haa95532_1
platformdirs              3.10.0           py38haa95532_0
ply                       3.11                     py38_0
prometheus_client         0.14.1           py38haa95532_0
prompt-toolkit            3.0.43           py38haa95532_0
prompt_toolkit            3.0.43               hd3eb1b0_0
protobuf                  3.19.6                   pypi_0    pypi
psutil                    5.9.0            py38h2bbff1b_0
pure_eval                 0.2.2              pyhd3eb1b0_0
pyasn1                    0.5.1                    pypi_0    pypi
pyasn1-modules            0.3.0                    pypi_0    pypi
pycparser                 2.21               pyhd3eb1b0_0
pydot                     4.0.0                    pypi_0    pypi
pygments                  2.15.1           py38haa95532_1
pyparsing                 3.1.1                    pypi_0    pypi
pyqt                      5.15.10          py38hd77b12b_0
pyqt5-sip                 12.13.0          py38h2bbff1b_0
pysocks                   1.7.1            py38haa95532_0
python                    3.8.18               h1aa4202_0
python-dateutil           2.8.2              pyhd3eb1b0_0
python-fastjsonschema     2.16.2           py38haa95532_0
python-json-logger        2.0.7            py38haa95532_0
pytz                      2023.3.post1     py38haa95532_0
pywavelets                1.4.1                    pypi_0    pypi
pywin32                   305              py38h2bbff1b_0
pywinpty                  2.0.10           py38h5da7b33_0
pyyaml                    6.0.1            py38h2bbff1b_0
pyzmq                     25.1.2           py38hd77b12b_0
qt-main                   5.15.2              h19c9488_10
qtconsole                 5.5.0            py38haa95532_0
qtpy                      2.4.1            py38haa95532_0
referencing               0.30.2           py38haa95532_0
requests                  2.31.0           py38haa95532_1
requests-oauthlib         1.3.1                    pypi_0    pypi
rfc3339-validator         0.1.4            py38haa95532_0
rfc3986-validator         0.1.1            py38haa95532_0
rpds-py                   0.10.6           py38h062c2fa_0
rsa                       4.9                      pypi_0    pypi
scikit-image              0.21.0                   pypi_0    pypi
scikit-learn              1.3.2                    pypi_0    pypi
scipy                     1.10.1                   pypi_0    pypi
segmentation-models       1.0.1                    pypi_0    pypi
send2trash                1.8.2            py38haa95532_0
setuptools                68.2.2           py38haa95532_0
sip                       6.7.12           py38hd77b12b_0
six                       1.16.0             pyhd3eb1b0_1
sniffio                   1.3.0            py38haa95532_0
soupsieve                 2.5              py38haa95532_0
sqlite                    3.41.2               h2bbff1b_0
stack_data                0.2.0              pyhd3eb1b0_0
tensorboard               2.9.1                    pypi_0    pypi
tensorboard-data-server   0.6.1                    pypi_0    pypi
tensorboard-plugin-wit    1.8.1                    pypi_0    pypi
tensorflow-estimator      2.9.0                    pypi_0    pypi
tensorflow-gpu            2.9.0                    pypi_0    pypi
tensorflow-io-gcs-filesystem 0.31.0                   pypi_0    pypi
termcolor                 2.4.0                    pypi_0    pypi
terminado                 0.17.1           py38haa95532_0
threadpoolctl             3.5.0                    pypi_0    pypi
tifffile                  2023.7.10                pypi_0    pypi
tinycss2                  1.2.1            py38haa95532_0
tomli                     2.0.1            py38haa95532_0
tornado                   6.3.3            py38h2bbff1b_0
traitlets                 5.7.1            py38haa95532_0
types-python-dateutil     2.9.0.20241206           pypi_0    pypi
typing-extensions         4.9.0            py38haa95532_1
typing_extensions         4.9.0            py38haa95532_1
uri-template              1.3.0                    pypi_0    pypi
urllib3                   2.1.0            py38haa95532_1
vc                        14.2                 h21ff451_1
vs2015_runtime            14.27.29016          h5e58377_2
wcwidth                   0.2.5              pyhd3eb1b0_0
webcolors                 24.8.0                   pypi_0    pypi
webencodings              0.5.1                    py38_1
websocket-client          0.58.0           py38haa95532_4
werkzeug                  3.0.1                    pypi_0    pypi
wheel                     0.41.2           py38haa95532_0
widgetsnbextension        4.0.5            py38haa95532_0
win_inet_pton             1.1.0            py38haa95532_0
winpty                    0.4.3                         4
wrapt                     1.16.0                   pypi_0    pypi
xz                        5.4.5                h8cc25b3_0
yaml                      0.2.5                he774522_0
zeromq                    4.3.5                hd77b12b_0
zipp                      3.17.0           py38haa95532_0
zlib                      1.2.13               h8cc25b3_0
zstd                      1.5.5                hd43e919_0
```

Linux: segnet-vgg.ipynb and segnet.ipynb is linux environment, related python packages are:

```
(base) wujieyu@lthpc:~$ conda activate tf
(tf) wujieyu@lthpc:~$ conda list
# packages in environment at /data/wujieyu/anaconda3/envs/tf:
#
# Name                    Version                   Build  Channel
_libgcc_mutex             0.1                        main  
_openmp_mutex             5.1                       1_gnu  
absl-py                   2.1.0            py39h06a4308_0  
anyio                     4.9.0                    pypi_0    pypi
aom                       3.6.0                h6a678d5_0  
argon2-cffi               23.1.0                   pypi_0    pypi
argon2-cffi-bindings      21.2.0                   pypi_0    pypi
arrow                     1.3.0                    pypi_0    pypi
asttokens                 3.0.0                    pypi_0    pypi
astunparse                1.6.3                      py_0  
async-lru                 2.0.5                    pypi_0    pypi
attrs                     25.3.0                   pypi_0    pypi
babel                     2.17.0                   pypi_0    pypi
beautifulsoup4            4.13.4                   pypi_0    pypi
blas                      1.0                         mkl  
bleach                    6.2.0                    pypi_0    pypi
brotli-python             1.0.9            py39h6a678d5_9  
bzip2                     1.0.8                h4bc722e_7    conda-forge
c-ares                    1.19.1               h5eee18b_0  
ca-certificates           2025.4.26            hbd8a1cb_0    conda-forge
cairo                     1.16.0               hb05425b_5  
certifi                   2025.4.26          pyhd8ed1ab_0    conda-forge
cffi                      1.17.1                   pypi_0    pypi
charset-normalizer        3.3.2              pyhd3eb1b0_0  
comm                      0.2.2                    pypi_0    pypi
contourpy                 1.3.0                    pypi_0    pypi
cuda-crt-tools            12.4.131             h06a4308_0  
cuda-cudart               12.4.127             h99ab3db_0  
cuda-cudart_linux-64      12.4.127             hd681fbe_0  
cuda-cupti                12.4.127             h6a678d5_1  
cuda-nvcc-tools           12.4.131             h99ab3db_0  
cuda-nvrtc                12.4.127             h99ab3db_1  
cuda-nvtx                 12.4.127             h6a678d5_1  
cuda-nvvm-tools           12.4.131             h6a678d5_0  
cuda-version              12.4                 hbda6634_3  
cudnn                     9.1.1.17               cuda12_1  
cycler                    0.12.1                   pypi_0    pypi
cyrus-sasl                2.1.28               h52b45da_1  
dav1d                     1.2.1                hd590300_0    conda-forge
dbus                      1.13.18              hb2f20db_0  
debugpy                   1.8.14                   pypi_0    pypi
decorator                 5.2.1                    pypi_0    pypi
defusedxml                0.7.1                    pypi_0    pypi
efficientnet              1.0.0                    pypi_0    pypi
eigen                     3.4.0                h4bd325d_0    conda-forge
exceptiongroup            1.2.2                    pypi_0    pypi
executing                 2.2.0                    pypi_0    pypi
expat                     2.7.0                h5888daf_0    conda-forge
fastjsonschema            2.21.1                   pypi_0    pypi
ffmpeg                    6.1.1                h2a67f75_3  
flatbuffers               24.3.25              h6a678d5_0  
fontconfig                2.14.1               h55d465d_3  
fonttools                 4.57.0                   pypi_0    pypi
fqdn                      1.5.1                    pypi_0    pypi
freetype                  2.10.4               h0708190_1    conda-forge
gast                      0.5.3              pyhd3eb1b0_0  
giflib                    5.2.2                h5eee18b_0  
glib                      2.78.4               h6a678d5_0  
glib-tools                2.78.4               h6a678d5_0  
google-pasta              0.2.0              pyhd3eb1b0_0  
graphite2                 1.3.14               h295c915_1  
grpcio                    1.62.2           py39h6a678d5_0  
gst-plugins-base          1.14.1               h6a678d5_1  
gstreamer                 1.14.1               h5eee18b_1  
h11                       0.16.0                   pypi_0    pypi
h5py                      3.12.1           py39h5842655_1  
harfbuzz                  10.2.0               hf296adc_0  
hdf5                      1.14.5               h2b7332f_2  
httpcore                  1.0.9                    pypi_0    pypi
httpx                     0.28.1                   pypi_0    pypi
icu                       73.1                 h6a678d5_0  
idna                      3.7              py39h06a4308_0  
image-classifiers         1.0.0                    pypi_0    pypi
imageio                   2.37.0                   pypi_0    pypi
importlib-metadata        8.5.0            py39h06a4308_0  
importlib-resources       6.5.2                    pypi_0    pypi
intel-openmp              2023.1.0         hdb19cb5_46306  
ipykernel                 6.29.5                   pypi_0    pypi
ipython                   8.18.1                   pypi_0    pypi
ipywidgets                8.1.7                    pypi_0    pypi
isoduration               20.11.0                  pypi_0    pypi
jedi                      0.19.2                   pypi_0    pypi
jinja2                    3.1.6                    pypi_0    pypi
joblib                    1.5.1                    pypi_0    pypi
jpeg                      9e                   h5eee18b_3  
json5                     0.12.0                   pypi_0    pypi
jsonpointer               3.0.0                    pypi_0    pypi
jsonschema                4.23.0                   pypi_0    pypi
jsonschema-specifications 2025.4.1                 pypi_0    pypi
jupyter                   1.1.1                    pypi_0    pypi
jupyter-client            8.6.3                    pypi_0    pypi
jupyter-console           6.6.3                    pypi_0    pypi
jupyter-core              5.7.2                    pypi_0    pypi
jupyter-events            0.12.0                   pypi_0    pypi
jupyter-lsp               2.2.5                    pypi_0    pypi
jupyter-server            2.15.0                   pypi_0    pypi
jupyter-server-terminals  0.5.3                    pypi_0    pypi
jupyterlab                4.4.2                    pypi_0    pypi
jupyterlab-pygments       0.3.0                    pypi_0    pypi
jupyterlab-server         2.27.3                   pypi_0    pypi
jupyterlab-widgets        3.0.15                   pypi_0    pypi
keras                     3.6.0            py39h06a4308_0  
keras-applications        1.0.8                    pypi_0    pypi
keras-unet                0.1.2                    pypi_0    pypi
kiwisolver                1.4.7                    pypi_0    pypi
krb5                      1.20.1               h143b758_1  
lame                      3.100             h166bdaf_1003    conda-forge
lazy-loader               0.4                      pypi_0    pypi
ld_impl_linux-64          2.40                 h12ee557_0  
leptonica                 1.82.0               h42c8aad_2  
lerc                      4.0.0                h0aef613_1    conda-forge
libabseil                 20240116.2      cxx17_h6a678d5_0  
libarchive                3.7.7                hfab0078_0  
libclang                  14.0.6          default_hc6dbbc7_2  
libclang13                14.0.6          default_he11475f_2  
libcublas                 12.4.5.8             h99ab3db_1  
libcufft                  11.2.1.3             h99ab3db_1  
libcups                   2.4.2                h2d74bed_1  
libcurand                 10.3.5.147           h99ab3db_1  
libcurl                   8.12.1               hc9e6f67_0  
libcusolver               11.6.1.9             h99ab3db_1  
libcusparse               12.3.1.170           h99ab3db_1  
libdeflate                1.22                 hb9d3cd8_0    conda-forge
libedit                   3.1.20230828         h5eee18b_0  
libev                     4.33                 h7f8727e_1  
libexpat                  2.7.0                h5888daf_0    conda-forge
libffi                    3.4.4                h6a678d5_1  
libgcc                    15.1.0               h767d61c_2    conda-forge
libgcc-ng                 15.1.0               h69a702a_2    conda-forge
libgfortran-ng            11.2.0               h00389a5_1  
libgfortran5              11.2.0               h1234567_1  
libglib                   2.78.4               hdc74915_0  
libgomp                   15.1.0               h767d61c_2    conda-forge
libgrpc                   1.62.2               h2d74bed_0  
libiconv                  1.18                 h4ce23a2_1    conda-forge
libllvm14                 14.0.6               hecde1de_4  
libnghttp2                1.57.0               h2d74bed_0  
libnvjitlink              12.4.127             h99ab3db_1  
libogg                    1.3.5                hd0c01bc_1    conda-forge
libopus                   1.5.2                hd0c01bc_0    conda-forge
libpng                    1.6.39               h5eee18b_0  
libpq                     17.4                 hdbd6064_0  
libprotobuf               4.25.3               he621ea3_0  
libssh2                   1.11.1               h251f7ec_0  
libstdcxx                 15.1.0               h8f9b012_2    conda-forge
libstdcxx-ng              11.2.0               h1234567_1  
libtheora                 1.1.1             h4ab18f5_1006    conda-forge
libtiff                   4.5.1                hffd6297_1  
libuuid                   1.41.5               h5eee18b_0  
libvorbis                 1.3.7                h9c3ff4c_0    conda-forge
libvpx                    1.13.1               h6a678d5_0  
libwebp                   1.3.2                h11a3e52_0  
libwebp-base              1.3.2                hd590300_1    conda-forge
libxcb                    1.17.0               h8a09558_0    conda-forge
libxkbcommon              1.9.2                h65c71a3_0    conda-forge
libxml2                   2.13.8               hfdd30dd_0  
lz4-c                     1.9.4                h6a678d5_1  
markdown                  3.8              py39h06a4308_0  
markdown-it-py            2.2.0            py39h06a4308_1  
markupsafe                3.0.2            py39h5eee18b_0  
matplotlib                3.9.4                    pypi_0    pypi
matplotlib-inline         0.1.7                    pypi_0    pypi
mdurl                     0.1.0            py39h06a4308_0  
mistune                   3.1.3                    pypi_0    pypi
mkl                       2023.1.0         h213fc3f_46344  
mkl-service               2.4.0            py39h5eee18b_2  
mkl_fft                   1.3.11           py39h5eee18b_0  
mkl_random                1.2.8            py39h1128e8f_0  
ml_dtypes                 0.4.1            py39hc74f9fe_0  
mysql                     8.4.0                h29a9f33_1  
namex                     0.0.7            py39h06a4308_0  
nbclient                  0.10.2                   pypi_0    pypi
nbconvert                 7.16.6                   pypi_0    pypi
nbformat                  5.10.4                   pypi_0    pypi
nccl                      2.21.5.1             ha515578_0  
ncurses                   6.4                  h6a678d5_0  
nest-asyncio              1.6.0                    pypi_0    pypi
networkx                  3.2.1                    pypi_0    pypi
notebook                  7.4.2                    pypi_0    pypi
notebook-shim             0.2.4                    pypi_0    pypi
numpy                     1.26.4           py39h5f9d8c6_0  
numpy-base                1.26.4           py39hb5e798b_0  
opencv                    4.10.0           py39h2484693_2  
openh264                  2.1.1                h780b84a_0    conda-forge
openjpeg                  2.5.2                he7f1fd0_0  
openldap                  2.6.4                h42fbc30_0  
openssl                   3.5.0                h7b32b05_1    conda-forge
opt_einsum                3.3.0              pyhd3eb1b0_1  
optree                    0.14.1           py39hdb19cb5_0  
overrides                 7.7.0                    pypi_0    pypi
packaging                 24.2             py39h06a4308_0  
pandocfilters             1.5.1                    pypi_0    pypi
parso                     0.8.4                    pypi_0    pypi
pcre2                     10.42                hebb0a14_1  
pexpect                   4.9.0                    pypi_0    pypi
pillow                    11.2.1                   pypi_0    pypi
pip                       25.1               pyhc872135_2  
pixman                    0.46.0               h29eaf8c_0    conda-forge
platformdirs              4.3.8                    pypi_0    pypi
prometheus-client         0.21.1                   pypi_0    pypi
prompt-toolkit            3.0.51                   pypi_0    pypi
protobuf                  4.25.3           py39he36ed58_1  
psutil                    7.0.0                    pypi_0    pypi
pthread-stubs             0.4               hb9d3cd8_1002    conda-forge
ptyprocess                0.7.0                    pypi_0    pypi
pure-eval                 0.2.3                    pypi_0    pypi
pycparser                 2.22                     pypi_0    pypi
pygments                  2.19.1           py39h06a4308_0  
pyparsing                 3.2.3                    pypi_0    pypi
pysocks                   1.7.1            py39h06a4308_0  
python                    3.9.21               he870216_1  
python-dateutil           2.9.0.post0              pypi_0    pypi
python-flatbuffers        24.3.25          py39h06a4308_0  
python-json-logger        3.3.0                    pypi_0    pypi
pyyaml                    6.0.2                    pypi_0    pypi
pyzmq                     26.4.0                   pypi_0    pypi
qt-main                   5.15.2              hb6262e9_12  
re2                       2022.04.01           h295c915_0  
readline                  8.2                  h5eee18b_0  
referencing               0.36.2                   pypi_0    pypi
requests                  2.32.3           py39h06a4308_1  
rfc3339-validator         0.1.4                    pypi_0    pypi
rfc3986-validator         0.1.1                    pypi_0    pypi
rich                      13.9.4           py39h06a4308_0  
rpds-py                   0.24.0                   pypi_0    pypi
scikit-image              0.24.0                   pypi_0    pypi
scikit-learn              1.6.1                    pypi_0    pypi
scipy                     1.13.1                   pypi_0    pypi
segmentation-models       1.0.1                    pypi_0    pypi
send2trash                1.8.3                    pypi_0    pypi
setuptools                78.1.1           py39h06a4308_0  
six                       1.17.0           py39h06a4308_0  
snappy                    1.2.1                h6a678d5_0  
sniffio                   1.3.1                    pypi_0    pypi
soupsieve                 2.7                      pypi_0    pypi
sqlite                    3.45.3               h5eee18b_0  
stack-data                0.6.3                    pypi_0    pypi
tbb                       2021.8.0             hdb19cb5_0  
tensorboard               2.17.0           py39h06a4308_0  
tensorboard-data-server   0.7.0            py39h52d8a92_1  
tensorflow                2.17.0          cuda124py39ha1f05a4_200  
tensorflow-base           2.17.0          cuda124py39h3b6feb8_200  
tensorflow-estimator      2.17.0          cuda124py39he5efd2c_200  
tensorflow-gpu            2.17.0          cuda124py39hd65659d_200  
termcolor                 2.1.0            py39h06a4308_0  
terminado                 0.18.1                   pypi_0    pypi
tesseract                 5.2.0                h6a678d5_2  
threadpoolctl             3.6.0                    pypi_0    pypi
tifffile                  2024.8.30                pypi_0    pypi
tinycss2                  1.4.0                    pypi_0    pypi
tk                        8.6.14               h39e8969_0  
tomli                     2.2.1                    pypi_0    pypi
tornado                   6.4.2                    pypi_0    pypi
traitlets                 5.14.3                   pypi_0    pypi
types-python-dateutil     2.9.0.20241206           pypi_0    pypi
typing-extensions         4.12.2           py39h06a4308_0  
typing_extensions         4.12.2           py39h06a4308_0  
tzdata                    2025b                h04d1e81_0  
uri-template              1.3.0                    pypi_0    pypi
urllib3                   2.3.0            py39h06a4308_0  
wcwidth                   0.2.13                   pypi_0    pypi
webcolors                 24.11.1                  pypi_0    pypi
webencodings              0.5.1                    pypi_0    pypi
websocket-client          1.8.0                    pypi_0    pypi
werkzeug                  3.1.3            py39h06a4308_0  
wheel                     0.45.1           py39h06a4308_0  
widgetsnbextension        4.0.14                   pypi_0    pypi
wrapt                     1.17.0           py39h5eee18b_0  
xkeyboard-config          2.44                 hb9d3cd8_0    conda-forge
xorg-libx11               1.8.12               h4f16b4b_0    conda-forge
xorg-libxau               1.0.12               hb9d3cd8_0    conda-forge
xorg-libxdmcp             1.1.5                hb9d3cd8_0    conda-forge
xz                        5.6.4                h5eee18b_1  
zipp                      3.21.0           py39h06a4308_0  
zlib                      1.2.13               h5eee18b_1  
zstd                      1.5.6                hc292b87_0  
```

