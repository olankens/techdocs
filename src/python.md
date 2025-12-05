<hr>

# PYTHON

### Create Local Conda Environment

```shell
conda create --prefix ./.venv python=3.11
conda activate ./.venv
which python
```

<hr>

### Create Named Conda Environment

```shell
conda create -n work python=3.11 -y
conda activate work
conda install <package_name> -y
```

<hr>

### Vanish Named Conda Environment

```shell
conda remove -n work --all -y
```

<hr>
