# termux-beautify
termux美化教程
echo "deb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main" > $PREFIX/etc/apt/sources.list
pkg update
pkg install git
git clone https://gh-proxy.org/https://github.com/Sugars0612/dotfiles
cd dotfiles
chmod +x ./bootstarp-termux.sh ./install-termux.she
yes Y | ./bootstarp-termux.sh && yes Y | ./install-termux.sh
