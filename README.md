# transmitor
# 删除之前创建的无效配置
rm -rf ~/.config/qt5ct/

# 强制使用xcb平台（确保大写XCB）
QT_QPA_PLATFORM=xcb colmap gui

# 创建新的环境变量配置
echo -e "export QT_QPA_PLATFORM=xcb\nexport __GLX_VENDOR_LIBRARY_NAME=nvidia" >> ~/.bashrc
source ~/.bashrc

# 运行COLMAP
colmap gui

# 检查插件是否存在
ls /usr/lib/x86_64-linux-gnu/qt5/plugins/platforms/  # 应看到libqxcb.so

# 如果缺失，重新安装Qt插件
sudo apt install --reinstall qtx11extras5 libqt5x11extras5-dev
