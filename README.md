﻿# testGPT

#### create a venv :

```
python -m venv yuGPT
```

#### activate the env :

##### for windows :

```
yuGPT\Scripts\activate
```

##### for mac/linux:

```
source yuGPT/bin/activate
```

#### intsall dependencies :

```
pip3 install matplotlib numpy pylzma ipykernel jupyter
```

#### install torch :

(if you have a nvidia gpu get te approprite command from torch website to install with cuda : https://pytorch.org/get-started/locally/)

```
pip3 install torch
```

#### create an environment to use as kernel for jupyter notebooks:

```
python -m ipykernel install --user --name=yuGPT --display-name "yungting-gpt"
```

#### If you want to have the jupyter notebook running on a pc while you acess it from your laptop :

##### i) generate cinfug file for jupyter notebook :

```
jupyter notebook --generate-config
```

##### ii) edit the config

paste the following two lines in the generated config

e.g. if you have vscode with the path set :

```
code C:\Users\Srira\.jupyter\jupyter_server_config.json
```

replace the C:/... with your path to the config which was shown when you ran the generate config command

these two lines :

```
c.NotebookApp.allow_origin = '*' #allow all origins

c.NotebookApp.ip = '0.0.0.0' # listen on all IPs
```

if the port you are using for jupyter notebook is blocked you will have to enable the port

##### iii) (optional) set a password so that when you use access notebooks a password needs to be entered

```
jupyter notebook password
```

now you can connect by your_pc_ip:portofjupyternotebook on other devices
http://xxx.xxx.xxx.xxx:8888/login

after running the notebook using the command below

#### start jupyter notebook :

```
jupyter notebook
```
