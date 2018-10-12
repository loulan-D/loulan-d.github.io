---
layout: post
title: "jupyter-notebook"
date: 2018-10-12 20:07:41 +0800
comments: true
categories: python

---

#### Jupyter notebook 安装conda环境

##### 安装:

```python
conda install ipykernel
```

##### 激活对应的conda环境:

```python
source activate environment_name
```

##### 将环境写入notebook 的kernel:

```python
python -m ipykernel install --user --name 环境名称  --display-name "Python （环境名称）"
```

##### 打开notebook

```python
jupyter notebook
```

-----

-----

#### 使用conda 创建 虚拟环境

```python
conda -V
conda list
conda env list   or  conda info -e       # 查看当前有那些虚拟环境
conda update conda

conda create -n env_name python=x.x      # 创建一个虚拟环境
source activate env_name
conda install -n env_name [package]
source deactivate
conda remove -n env_name -all
conda remove --name env_name package_name
```





