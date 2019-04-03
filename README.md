## 1. 人工智能的应用领域：自动驾驶、图像识别、机器人、智能音箱、虚拟现实眼镜

## 2. 人工智能的知识储备库：
### 1. 数学基础：高等数学、离散数学、概率论与数理统计等；
### 2. 基础科学：生物学、物理学、社会学等；
### 3. 计算机科学：机器学习、深度学习、CNN、RNN、DNN等；
### 4. 编程与框架：python、C++、Java、tensorflow、Caffe、ros编程等；
### 5. 硬件：树莓派、传感器、控制器、制动器等。

## 3. Install tensorflow on ubuntu
### 1. currently tensorflow only support python version < 3.6. So we will need to install python3.6 first on ubuntu.
### 2. install pip3 that linked to python3.6
python3.6 -m pip install --upgrade pip setuptools wheel
### 3. install needed 
sudo apt update
sudo apt install python3-dev python3-pip
sudo pip3 install -U virtualenv  # system-wide install

### 3. create and activate a virtual environment 
2.1 virtualenv --system-site-packages -p python3.6 ./venv1 # this is to create a virtual environment that named venv1 and linked to python 3.6
2.2 source ./venv1/bin/activate

### 4. install tensorflow in a virtual environment
pip3 install --upgrade tensorflow




