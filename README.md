xkb-bbokt
=========

Xkb custom layouts from http://forum.colemak.com/viewtopic.php?id=1438&amp;p=1


    cd /usr/share/X11/xkb/; \
    setxkbmap \
        -rules colemak \
        -model pc105awide-sl \
        -layout nocolemak,brcolemak \
        -variant cmk_ed_us,cmk_ed_us \
        -option lv5:caps_switch_lock,misc:extend,grp:ctrls_toggle \
        -print \
        | xkbcomp  -I$PWD - :0
