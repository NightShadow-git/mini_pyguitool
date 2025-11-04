# PyTool - Python GUI 工具集

一个功能丰富的 Python GUI 工具集，提供多种文本处理、编码解码和开发辅助功能。

## 功能特性

### 📝 文本处理
- **文本替换** - 支持普通替换和换行符处理
- **文本统计** - 统计字符数、数字、中英文、标点符号等
- **文本分割** - 按分隔符分割，支持去除空格和显示行号
- **多行文本处理** - 去重、排序和重复统计
- **文本合并** - 多行文本合并为单行
- **文本逆序** - 每行逆序或全部逆序
- **文本行定长** - 将长行按指定长度分割

### 🔄 编码/解码
- **Base64 编码/解码** - 支持多种 Base64 变体（Base16、Base32、Base64、Base85 等）
- **URL 编码/解码** - 标准 URL 编码处理
- **HTML 编码/解码** - HTML 实体编码转换

### 🌐 网络工具
- **Curl Converter** - 将 curl 命令转换为多种编程语言代码
  - 支持 50+ 种语言和框架（Python、JavaScript、Java、Go、PHP 等）

### 🔤 Unicode 工具
- **特殊符号库** - 数学符号、箭头、货币、表情符号等
- **字符信息查询** - 显示字符的 Unicode、十六进制、十进制编码和名称
- **字符范围生成** - 生成指定 Unicode 范围内的所有字符

## 环境要求

### 必需环境
- **Python 3.6+**
- **Node.js 12+**

### 依赖
- **curlconverter** - 用于 Curl Converter 功能

## 安装步骤

### 1. 安装 Python 依赖
```bash
# 确保已安装 tkinter（通常 Python 自带）
python -c "import tkinter; print('tkinter 可用')"
```

### 2. 安装 curlconverter

**全局安装：**
```bash
npm install -g curlconverter --registry https://mirrors.tuna.tsinghua.edu.cn/
```

**局部安装（推荐）：**
```bash
cd src
npm install curlconverter --registry https://mirrors.tuna.tsinghua.edu.cn/
```

## 使用方法

### 启动应用
```bash
python main.py
```

### 界面说明

应用采用标签页设计，主要分为三个部分：

1. **文本处理** - 各种文本操作工具
2. **编码/解码** - 编码转换工具  
3. **CurlConverter** - 网络命令转换工具

### 功能使用示例

#### Curl 命令转换
1. 打开 "CurlConverter" 标签页
2. 粘贴 curl 命令到输入框
3. 选择目标编程语言
4. 点击 "Convert" 按钮生成代码

#### Base64 编码
1. 打开 "编码/解码" → "base64"
2. 输入要编码的文本
3. 选择编码方式和字符编码
4. 点击 "输出" 获取结果

#### 文本统计
1. 打开 "文本处理" → "文本统计"
2. 粘贴文本内容
3. 点击 "统计" 查看详细统计信息

## 项目结构

```
.
├── main.py              # 主程序入口
├── README.md           # 项目说明
└── src/                # 资源目录
    ├── *.js           # 临时生成的 JS 文件
    └── node_modules/  # Node.js 依赖（局部安装时）
```

## 技术特点

- **跨平台** - 基于 Python tkinter，支持 Windows、macOS、Linux
- **模块化设计** - 功能独立，易于扩展
- **线程安全** - 使用锁机制确保多线程安全
- **用户友好** - 直观的 GUI 界面，操作简单

## 注意事项

- 确保 Node.js 已正确安装并添加到系统 PATH
- 局部安装 curlconverter 时，请确保 `src` 目录存在
- 部分功能需要网络连接（如在线符号库参考）

## 许可证

本项目仅供学习和个人使用。

## 支持与反馈

如有问题或建议，请检查：
1. Node.js 和 Python 环境配置
2. curlconverter 安装是否正确
3. 系统权限是否足够

享受使用 PyTool 带来的便利！ 🚀