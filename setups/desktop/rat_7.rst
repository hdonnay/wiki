Stupid mouse needs a custom mapping in `xorg.conf`:

    Section "InputClass"
            Identifier "Mouse Remap"
            MatchProduct "Saitek Cyborg R.A.T.7 Mouse"
            MatchDevicePath "/dev/input/event*"
            Option "ButtonMapping" "1 2 3 4 5 6 7 2 9 10 11 12 0 0 0"
    EndSection
