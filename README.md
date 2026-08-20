# termux-beautify
termux美化教程


echo "deb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main" > $PREFIX/etc/apt/sources.list


pkg update


pkg install git


git clone https://gh-proxy.org/https://github.com/Sugars0612/dotfiles


cd dotfiles


chmod +x ./bootstarp-termux.sh ./install-termux.sh


yes Y | ./bootstarp-termux.sh && yes Y | ./install-termux.sh



至于termux，安装地址在这里：https://pan.quark.cn/s/e14865f858a1#/list/share


