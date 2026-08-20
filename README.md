# Termux 一键美化教程

> 让你的 Termux 终端从“黑白命令行”秒变“高颜值生产力工具”

本项目基于 [Sugars0612/dotfiles](https://github.com/Sugars0612/dotfiles) 配置，自动安装 Zsh、Oh My Zsh、Powerlevel10k 主题及常用插件，实现终端美化。
<img width="2560" height="1600" alt="1000278118" src="https://github.com/user-attachments/assets/64ee8025-634d-4eb9-958b-5b335f556392" />

---


## 前置要求
- Android 设备
- 已安装 Termux 应用

> Termux 安装建议：  
> - 官方推荐从 F-Droid 下载（兼容性最好）：[点此前往](https://f-droid.org/packages/com.termux/)  
> - 若无法访问 F-Droid，可使用我备好的安装包：📦 [夸克网盘下载](https://pan.quark.cn/s/e14865f858a1#/list/share) （请选择 `arm64-v8a` 版本）
> - 也可以用我给的release，[直接前往](https://github.com/XiaoBoMc/termux-beautify/releases/tag/termux%E4%B8%8B%E8%BD%BD%E5%9C%B0%E5%9D%80)
---

## 一键安装（所有命令集中在此）

复制以下整个代码块，粘贴到 Termux 终端中执行（建议逐条执行，也可一次性粘贴）：

```bash
# 1. 换用清华镜像源（加速国内下载）
echo "deb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main" > $PREFIX/etc/apt/sources.list

# 2. 更新软件包列表
pkg update

# 3. 安装 Git（用于克隆配置）
pkg install git

# 4. 克隆美化配置仓库（使用 gh-proxy 加速）
git clone https://gh-proxy.org/https://github.com/Sugars0612/dotfiles

# 5. 进入项目目录
cd dotfiles

# 6. 赋予脚本执行权限
chmod +x ./bootstarp-termux.sh ./install-termux.sh

# 7. 执行安装（自动确认所有提示）
yes Y | ./bootstarp-termux.sh && yes Y | ./install-termux.sh

#如安装失败，请再次运行yes Y | ./bootstarp-termux.sh && yes Y | ./install-termux.sh
```
安装好后，你会发现卡在一个页面不动了，这是新版本的一个bug，

不要犹豫，直接退出后台，否则后果自负（实际上就是卡死在那个

页面有概率让手机卡死，所以说最好快点退出，如果卡死了，

请点击下拉框菜单中的WIFI长按，就可以跳转到设置，然后再把termux关闭就行了）

然后重启termux
