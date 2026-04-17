# Cartographer 2D 建图（含2D回环检测）

## 一、安装依赖库

### 1. 安装 stow
```bash
sudo apt install  -y
```

### 2. 安装 abseil-cpp
```bash
cd src/cartographer/scripts
sudo chmod +x ./install_abseil.sh
sudo ./install_abseil.sh
```

## 二、工作空间编译

### 正常编译
```bash
catkin_make_isolated --install --use-ninja
```

### 出现 Python 版本报错时编译
```bash
catkin_make_isolated --install --use-ninja -DPYTHON_EXECUTABLE=/usr/bin/python3
```