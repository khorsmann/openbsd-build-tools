
user mod -G wsrc exampleuser
user mod -G wobj exampleuser

doas ./build_openbsd.py --build kernel --kernel GENERIC.MP --cvs_tag OPENBSD_6_3
doas ./build_openbsd.py --build userland --cvs_tag OPENBSD_6_3
doas ./build_openbsd.py --build release --cvs_tag OPENBSD_6_3
