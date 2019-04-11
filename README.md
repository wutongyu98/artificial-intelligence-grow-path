## 1. 人工智能的应用领域：自动驾驶、图像识别、机器人、智能音箱、虚拟现实眼镜

## 2. 人工智能的知识储备库：
 1. 数学基础：高等数学、离散数学、概率论与数理统计等；
 2. 基础科学：生物学、物理学、社会学等；
 3. 计算机科学：机器学习、深度学习、CNN、RNN、DNN等；
 4. 编程与框架：python、C++、Java、tensorflow、Caffe、ros编程等；
 5. 硬件：树莓派、传感器、控制器、制动器等。

## 3. Install tensorflow on ubuntu
### 1. currently tensorflow only support python version < 3.6. So we will need to install python3.6 first on ubuntu.

#### 1.1 sudo add-apt-repository ppa:jonathonf/python-3.6

#### 1.2 sudo apt-get update

#### 1.3 sudo apt-get install python3.6

#### 1.4 sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.5 1

#### 1.5 sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 2

#### 1.6 sudo update-alternatives --config python3

### 2. install pip3 that linked to python3.6

#### 2.1 python3.6 -m pip install --upgrade pip setuptools wheel

remarking: switch default python version can be done via adding these two lines in the .bashrc and then do source ~/.bashrc

remarking: "sudo apt-get install --reinstall python-minimal" can be used to correct the update error

alias python=python3.6

alias python3=python3.6

### 3. install needed 

#### 3.1 sudo apt update

#### 3.2 sudo apt install python3-dev python3-pip

#### 3.3 sudo pip3 install -U virtualenv  # system-wide install

### 4. create and activate a virtual environment 

#### 4.1 virtualenv --system-site-packages -p python3.6 ./venv 

#### 4.2 source ./venv1/bin/activate

### 5. install tensorflow in a virtual environment
#### 5.1  pip3 install --upgrade tensorflow




