doas cat > /etc/X11/xorg.conf << 'EOF'
Section "Device"
    Identifier "Card0"
    Driver "vesa"
EndSection

Section "Screen"
    Identifier "Screen0"
    Device "Card0"
    DefaultDepth 24
    SubSection "Display"
        Depth 24
        Modes "1024x768" "800x600"
    EndSubSection
EndSection

Section "Monitor"
    Identifier "Monitor0"
    Option "PreferredMode" "1024x768"
EndSection
EOF
