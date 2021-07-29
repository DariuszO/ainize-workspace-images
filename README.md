# ainize-workspace-images
Docker images for Ainize Workspace

## Development Extension
* [Jupyter Notebook](https://jupyter.org/)
* [Visual Studio Code](https://github.com/cdr/code-server)
* [Terminal - ttyd](https://github.com/tsl0922/ttyd)

## Package List
```
Package                       Version
----------------------------- -------------------
absl-py                       0.13.0
argon2-cffi                   20.1.0
astunparse                    1.6.3
async-generator               1.10
attrs                         21.2.0
backcall                      0.2.0
backports.functools-lru-cache 1.6.4
beautifulsoup4                4.9.3
bleach                        3.3.1
brotlipy                      0.7.0
cached-property               1.5.2
cachetools                    4.2.2
certifi                       2021.5.30
cffi                          1.14.6
chardet                       4.0.0
charset-normalizer            2.0.0
conda                         4.10.3
conda-build                   3.21.4
conda-package-handling        1.7.3
cryptography                  3.4.7
cycler                        0.10.0
decorator                     5.0.9
defusedxml                    0.7.1
entrypoints                   0.3
filelock                      3.0.12
flatbuffers                   1.12
gast                          0.4.0
glob2                         0.7
google-auth                   1.34.0
google-auth-oauthlib          0.4.4
google-pasta                  0.2.0
grpcio                        1.34.1
h5py                          3.1.0
idna                          3.1
importlib-metadata            4.6.1
ipykernel                     5.5.5
ipython                       7.25.0
ipython-genutils              0.2.0
ipywidgets                    7.6.3
jedi                          0.18.0
Jinja2                        3.0.1
joblib                        1.0.1
jsonschema                    3.2.0
jupyter-client                6.1.12
jupyter-core                  4.7.1
jupyterlab-pygments           0.1.2
jupyterlab-widgets            1.0.0
keras-nightly                 2.5.0.dev2021032900
Keras-Preprocessing           1.1.2
kiwisolver                    1.3.1
libarchive-c                  3.1
Markdown                      3.3.4
MarkupSafe                    2.0.1
matplotlib                    3.2.2
matplotlib-inline             0.1.2
mistune                       0.8.4
nbclient                      0.5.3
nbconvert                     6.1.0
nbformat                      5.1.3
nest-asyncio                  1.5.1
notebook                      6.4.0
numpy                         1.19.5
oauthlib                      3.1.1
opt-einsum                    3.3.0
packaging                     21.0
pandas                        1.1.5
pandocfilters                 1.4.2
parso                         0.8.2
pexpect                       4.8.0
pickleshare                   0.7.5
Pillow                        8.3.1
pip                           21.2.1
pkginfo                       1.7.1
prometheus-client             0.11.0
prompt-toolkit                3.0.19
protobuf                      3.17.3
psutil                        5.8.0
ptyprocess                    0.7.0
pyasn1                        0.4.8
pyasn1-modules                0.2.8
pycosat                       0.6.3
pycparser                     2.20
Pygments                      2.9.0
pyOpenSSL                     20.0.1
pyparsing                     2.4.7
pyrsistent                    0.17.3
PySocks                       1.7.1
python-dateutil               2.8.2
pytz                          2021.1
PyYAML                        5.4.1
pyzmq                         22.1.0
requests                      2.26.0
requests-oauthlib             1.3.0
rsa                           4.7.2
ruamel-yaml-conda             0.15.80
scikit-learn                  0.22.2.post1
scipy                         1.4.1
seaborn                       0.11.1
Send2Trash                    1.7.1
setuptools                    49.6.0.post20210108
six                           1.15.0
soupsieve                     2.0.1
tensorboard                   2.5.0
tensorboard-data-server       0.6.1
tensorboard-plugin-wit        1.8.0
tensorflow                    2.5.0
tensorflow-estimator          2.5.0
termcolor                     1.1.0
terminado                     0.10.1
testpath                      0.5.0
torch                         1.9.0
torchaudio                    0.9.0
torchvision                   0.10.0
tornado                       6.1
tqdm                          4.61.2
traitlets                     5.0.5
typing-extensions             3.7.4.3
urllib3                       1.26.6
wcwidth                       0.2.5
webencodings                  0.5.1
Werkzeug                      2.0.1
wheel                         0.36.2
widgetsnbextension            3.5.1
wrapt                         1.12.1
zipp                          3.5.0
```

## How to Test Your Image
Build Docker Image
```bash
docker build -t <image-name> .
```
Run Docker 
```bash
docker run -d -p 8000:8000 -p 8010:8010 -p 8020:8020 <tage-name>
```

Run Docker with Password
```bash
docker run -d -p 8000:8000 -p 8010:8010 -p 8020:8020 -e PASSWORD=<password> <image-name>
```

Run Docker with Github Repo
```bash
docker run -d -p 8000:8000 -p 8010:8010 -p 8020:8020 -e GH_REPO=<github-repo> <image-name>
```

Run Docker with password and Github Repo
```bash
docker run -d -p 8000:8000 -p 8010:8010 -p 8020:8020 -e PASSWORD=<password> -e GH_REPO=<github-repo> <image-name>
```

Jupyter Notebook : http://server-address:8000/

Visual Studio Code : http://server-address:8010/

Terminal - ttyd : http://server-address:8020/