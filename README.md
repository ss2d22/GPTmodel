# YungtingGPT

create a venv :

```
python -m venv yuGPT
```

activate the env :
for windows :

```
yuGPT\Scripts\activate
```

for mac:

intsall dependencies :

```
pip3 install matplotlib numpy pylzma ipykernel jupyter
```

install torch (if you have a nvidia gpu get te approprite command from torch website to install with cuda) :

```
pip3 install torch
```

create an environment to use as kernel for jupyter notebooks:

```
python -m ipykernel install --user --name=yuGPT --display-name "yungting-gpt"
```

start jupyter notebook :

```
jupyter notebook
```
