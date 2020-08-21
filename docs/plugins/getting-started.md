Developer Guideline

<br>

SpaceONE plugins help users collecting data from diverse cloud services: AWS, GCP, MS Azure, etc.

Developers can edit codes and even create new plugin.

## Initial Setting

### 1. python3.x

Python 2.7.10 version is installed on MAC OS by default. You should install Python 3.x version.

<br>

**Mac**

Using Homebrew

```bash
brew install python3
```

**Windows**

https://www.python.org/downloads/windows/

<br>

### 2. virtualenv

```bash
pip3 install virtualenv virtualenvwrapper
```

or you can use this too:

```bash
python3 -m pip install virtualenv virtualenvwrapper
```
<br>

## Edit the plugin

### 1. Clone

First, go to SpaceONE(https://github.com/spaceone-dev) and choose plugin repository you want to edit. Names of plugin repositories start with **'plugin-'

Click the 'Fork' button.

![](https://user-images.githubusercontent.com/41534832/90863701-7d1a5c80-e3ca-11ea-84cd-273254bf6a7b.png)

And clone your forked repository to local.



### 2. Project Setting

Check the directory.
```bash
plugin-***-****
├── bin
├── pkg
├── src
└── test
```

And go to Run > Edit Configuration. Click '+' button on the left side.
![](https://user-images.githubusercontent.com/41534832/90868678-1dc04a80-e3d2-11ea-951e-2c3230414ea6.png)

* Choose **Python** to add new configuration, and set 'Module name' as you want.

* Put `grpc spaceone.inventory` in **Parameters** for networking with other MicroServices.

* Set **Python interpreter** to Python 3.x you already installed.


Put this on terminal.(~/plugin-***-****)
```bash
virtualenv -p python3.8 venv
```

Check venv directory was created.

![](https://user-images.githubusercontent.com/41534832/90869977-f0749c00-e3d3-11ea-9814-934f5e7483c7.png)
