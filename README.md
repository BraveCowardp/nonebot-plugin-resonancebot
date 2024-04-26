<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-resonancebot/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://github.com/A-kirami/nonebot-plugin-resonancebot/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# nonebot-plugin-resonancebot

_✨ 雷索纳斯优质行情提醒插件 ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/BraveCowardp/nonebot-plugin-resonancebot.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/nonebot-plugin-resonancebot">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-resonancebot.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">

</div>

雷索纳斯优质行情提醒助手，可以在检测到好行情时主动发送通知

<details>
<summary>配置发布工作流</summary>

模块库中自带了一个发布工作流, 你可以使用此工作流自动发布你的插件到 pypi

> [!IMPORTANT]
> 这个发布工作流需要 pyproject.toml 文件, 并且只支持 [PEP 621](https://peps.python.org/pep-0621/) 标准的 pyproject.toml 文件

1. 前往 https://pypi.org/manage/account/#api-tokens 并创建一个新的 API 令牌。创建成功后不要关闭页面，不然你将无法再次查看此令牌。
2. 在单独的浏览器选项卡或窗口中，打开 [Actions secrets and variables](./settings/secrets/actions) 页面。你也可以在 Settings - Secrets and variables - Actions 中找到此页面。
3. 点击 New repository secret 按钮，创建一个名为 `PYPI_API_TOKEN` 的新令牌，并从第一步复制粘贴令牌。

</details>

<details>
<summary>触发发布工作流</summary>
从本地推送任意 tag 即可触发。

创建 tag:

    git tag <tag_name>

推送本地所有 tag:

    git push origin --tags

</details>

## 📖 介绍

计划通过通过目前公开的api轮询行情，遇到好行情时发送通知

毕竟不会有人一直盯着行情，感觉这种很适合交给机器人去做，目前nb的插件商店还没有雷索纳斯相关的插件，所以想自己做一个

能力有限，不知道什么时候填坑

计划先做一个简单的推荐算法，做一个最基础的满足条件就推送的功能，发布到插件商店，验证可用性，后面再慢慢优化推荐算法和丰富推送的类型

欢迎提issues或者discussions

## 💿 安装

<details open>
<summary>使用 nb-cli 安装</summary>
在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装

    nb plugin install nonebot-plugin-resonancebot

</details>

<details>
<summary>使用包管理器安装</summary>
在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

<details>
<summary>pip</summary>

    pip install nonebot-plugin-resonancebot
</details>
<details>
<summary>pdm</summary>

    pdm add nonebot-plugin-resonancebot
</details>
<details>
<summary>poetry</summary>

    poetry add nonebot-plugin-resonancebot
</details>
<details>
<summary>conda</summary>

    conda install nonebot-plugin-resonancebot
</details>

打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入

    plugins = ["nonebot_plugin_resonancebot"]

</details>

## ⚙️ 配置

在 nonebot2 项目的`.env`文件中添加下表中的必填配置

| 配置项 | 必填 | 默认值 | 说明 |
|:-----:|:----:|:----:|:----:|
| 配置项1 | 是 | 无 | 配置说明 |
| 配置项2 | 否 | 无 | 配置说明 |

## 🎉 使用
### 指令表
| 指令 | 权限 | 需要@ | 范围 | 说明 |
|:-----:|:----:|:----:|:----:|:----:|
| 指令1 | 主人 | 否 | 私聊 | 指令说明 |
| 指令2 | 群员 | 是 | 群聊 | 指令说明 |
### 效果图
如果有效果图的话
