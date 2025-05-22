# transmitor
# 创建自定义Qt配置
mkdir -p ~/.config/qt5ct/
cat > ~/.config/qt5ct/qt5ct.conf <<EOF
[Platform]
OpenGL=desktop
EOF

# 运行COLMAP
QT_QPA_PLATFORM=qt5ct colmap gui

QT_DEBUG_PLUGINS=1 colmap gui
