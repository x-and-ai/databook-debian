# xandai/databook-debian

[Docker Hub Link](https://hub.docker.com/r/xandai/databook-debian)

[GitHub Link](https://github.com/x-and-ai/databook-debian)

## Description

This is a Docker image for using Jupyter for data analysis with Python 3 on Debian.

This image contains following packages:

NumPy (for low-level math operations)
pandas (for data manipulation)
scikit-learn (for evaluation metrics)
imageio (for read and write images)
Matplotlib (for data visualization)
Seaborn (for heatmaps)

## Tags and Versions

| tag        | numpy      | pandas     | scikit-learn | imageio    | matplotlib | seaborn    | jupyter    | python     | debian     |
|:----------:|:----------:|:----------:|:------------:|:----------:|:----------:|:----------:|:----------:|:----------:|:----------:|
| 1.0.0      | 1.16.2     | 0.24.1     | 0.20.3       | 2.5.0      | 3.0.3      | 0.9.0      | 1.0.0      | 3.5.3-1    | 9.8        |

## Usage

- Start notebook without token

``` sh
docker run --rm -it -p <localhostport>:8888 -v /absolute/path/to/notebook/dir:/home/jupyter/notebook xandai/databook-debian:1.0.0 jupyter notebook --NotebookApp.token=''
```

- Start notebook with token

``` sh
docker run --rm -it -p <localhostport>:8888 -v /absolute/path/to/notebook/dir:/home/jupyter/notebook xandai/databook-debian:1.0.0
```
