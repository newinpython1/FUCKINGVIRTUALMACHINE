doas cat > /etc/X11/xorg.conf << 'EOF'
Section "Device"
    Identifier "Card0"
    Driver "vesa"
EndSection
EOF
