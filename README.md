# foo2zjs-zhcn-localize

## 项目名称
- 英文：foo2zjs Simplified Chinese Localization  
- 中文：foo2zjs 简体中文汉化工程

## 项目说明
针对开源激光打印机驱动 `foo2zjs` 制作完整的简体中文本地化，提供两种方案：增量汉化补丁、整合完成的全量汉化编译脚本，适配各类 Linux 发行版激光打印使用。

## 仓库内容
1. `foo2zjs-zh_CN-v1.0.patch`：增量汉化补丁文件  
2. `full-build/`：整合中文语言包的完整汉化源码目录  

## 使用方法

### 方式一：增量补丁（适合已有 foo2zjs 源码）
```bash
patch -p1 < foo2zjs-zh_CN-v1.0.patch
make clean && make
sudo make install
```

### 方式二：完整源码包（适合全新安装）
```bash
cd full-build/foo2zjs
make clean && make
sudo make install
```

## 已汉化内容（v1.0）
- 所有 `--help` 帮助信息（包括 `foo2zjs`、`foo2oak`、`foo2hp` 等全部命令）  
- 所有 wrapper 脚本的使用说明  

## 版本规划
- v1.0：帮助信息汉化  
- v2.0：运行时提示信息和常见错误信息汉化  
- v3.0：手册页（man）汉化  

## 开源协议
遵循原项目 GPLv2 协议开源
