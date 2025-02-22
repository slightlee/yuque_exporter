## 仓库说明

语*雀批量导出工具，可以自动将账户下所有知识库导出到本地，并按照知识库原有目录结构创建相应文件目录，同时文档将转换为Markdown文件。

本项目基于 [yuque_exporter](https://github.com/Jeandoom/yuque_exporter) ，在此基础上增加了自定义相关配置以及使用说明... 

## 使用说明

### 1、安装python环境

> 根据自己电脑环境安装即可

### 2、安装依赖

> 项目根目录执行

```shell
pip install -r requirements.txt
```

### 3、修改配置

> 复制`.env.sample`文件到当前目录并重新命名 `.env` , 修改文件内容 

```text
# cookie
yuque_cookie=lang=zh-cn; _yuque_session=xxxxxx==; yuque_ctoken=xxxxxxx; acw_tc=xxxxxxxxxx
# 取cookie中的yuque_ctoken的值
csrf_token=xxxxxxx
# 输出目录 可以自定义
output_directory=./exported/
```

### 4、执行脚本

> 项目根目录执行

```shell
python exporter.py
```

## 贡献

如果您愿意共享或改进代码，请随时提交请求（Pull Request）或创建问题（Issue）。欢迎您的贡献和反馈。

## 声明

此仓库目的是用来学习和技术交流，维护者不对仓库的滥用以及不当使用负责。任何违法行为与本仓库的维护者无关，使用者需自行承担法律责任。请使用仓库时自行遵守法律法规。谢谢您的理解和合作！
