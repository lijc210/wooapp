# WSL2 ubuntu配置环境
sudo apt update
sudo apt install libwebkit2gtk-4.1-dev \
    build-essential \
    curl \
    wget \
    libssl-dev \
    libgtk-3-dev \
    libayatana-appindicator3-dev \
    librsvg2-dev

sudo apt install pkg-config \
  libdbus-1-dev \
  libgtk-3-dev \
  libsoup2.4-dev \
  libjavascriptcoregtk-4.0-dev \
  libwebkit2gtk-4.0-dev

# mac配置环境

# windwos配置环境


# 升级rust
rustup update
# 创建项目
cargo install create-tauri-app
cargo create-tauri-app

# 升级项目
cargo update
# 安装依赖
nvm use v16.20.0
pnpm install

# 启动方式一
pnpm tauri dev

# 启动方式二
cargo tauri dev

# 打包（默认项目dmg包与msi包2M多，二进制包5M多
pnpm tauri build

# 创建src-tauri（不用执行，create-tauri-app会自动创建）
cargo install tauri-cli
cargo tauri init


# 问题
在wsl2 ubuntu环境下，项目文件如果放在windows目录下，每次启动需要重复编译,而且慢，所以项目文件应该访问wsl2 ubuntu里面

#failed to bundle project: error running light.exe
package.productName 不能纯数字

# WebView2 Installation Options
https://tauri.app/zh-cn/v1/guides/building/windows/


# 推送到github
git remote add origin2 https://github.com/lijc210/woo-app.git
