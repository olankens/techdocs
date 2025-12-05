<hr>

# PYTHON

### Create Local Conda Environment

```bash
conda create --prefix ./.venv python=3.11
conda activate ./.venv
which python
```

<hr>

### Create Named Conda Environment

```bash
conda create -n work python=3.11 -y
conda activate work
conda install <package_name> -y
```

<hr>

### Vanish Named Conda Environment

```bash
conda remove -n work --all -y
```

<hr>
