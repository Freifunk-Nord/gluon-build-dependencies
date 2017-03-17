gluon-build-dependencies
========================

Dieses Repo enthällt alle Dateien die während des make Prozesses vom gluon make Script heruntergeladen werden müssen. Dies beugt Problemen
vor, die durch nicht erreichbare Server beim Kompilieren entstehen können.

Anwendung:
-------------------------------------
 
 ### Repository clonen
 
    mkdir git-repo
    cd git-repo
    git clone https://github.com/Freifunk-Nord/gluon-build-dependencies
    git clone https://github.com/freifunk-gluon/gluon.git
    cd gluon
 
 ### Ordnerstruktur anlegen
 
    mkdir openwrt
    mkdir build
    mkdir build/ar71xx-generic
    mkdir build/ar71xx-mikrotik
    mkdir build/ar71xx-nand
    mkdir build/brcm2708-bcm2708
    mkdir build/brcm2708-bcm2709
    mkdir build/mpc85xx-generic
    mkdir build/ramips-mt7621
    mkdir build/ramips-rt305x
    mkdir build/sunxi
    mkdir build/x86-64
    mkdir build/x86-generic
    mkdir build/x86-kvm_guest
    mkdir build/x86-xen_domu
    mkdir build/ar71xx-generic/openwrt
    mkdir build/ar71xx-mikrotik/openwrt
    mkdir build/ar71xx-nand/openwrt
    mkdir build/brcm2708-bcm2708/openwrt
    mkdir build/brcm2708-bcm2709/openwrt
    mkdir build/mpc85xx-generic/openwrt
    mkdir build/ramips-mt7621/openwrt
    mkdir build/ramips-rt305x/openwrt
    mkdir build/sunxi/openwrt
    mkdir build/x86-64/openwrt
    mkdir build/x86-generic/openwrt
    mkdir build/x86-kvm_guest/openwrt
    mkdir build/x86-xen_domu/openwrt
 
### Symlinks setzen

    ln -s ../gluon-build-dependencies/openwrt/dl openwrt/dl
    ln -s ../gluon-build-dependencies/build/ar71xx-generic/openwrt/bin build/ar71xx-generic/openwrt/bin
    ln -s ../gluon-build-dependencies/build/ar71xx-mikrotik/openwrt/bin build/ar71xx-mikrotik/openwrt/bin
    ln -s ../gluon-build-dependencies/build/ar71xx-nand/openwrt/bin build/ar71xx-nand/openwrt/bin
    ln -s ../gluon-build-dependencies/build/brcm2708-bcm2708/openwrt/bin build/brcm2708-bcm2708/openwrt/bin
    ln -s ../gluon-build-dependencies/build/brcm2708-bcm2709/openwrt/bin build/brcm2708-bcm2709/openwrt/bin
    ln -s ../gluon-build-dependencies/build/mpc85xx-generic/openwrt/bin build/mpc85xx-generic/openwrt/bin
    ln -s ../gluon-build-dependencies/build/ramips-mt7621/openwrt/bin build/ramips-mt7621/openwrt/bin
    ln -s ../gluon-build-dependencies/build/ramips-rt305x/openwrt/bin build/ramips-rt305x/openwrt/bin
    ln -s ../gluon-build-dependencies/build/sunxi/openwrt/bin build/sunxi/openwrt/bin
    ln -s ../gluon-build-dependencies/build/x86-64/openwrt/bin build/x86-64/openwrt/bin
    ln -s ../gluon-build-dependencies/build/x86-generic/openwrt/bin build/x86-generic/openwrt/bin
    ln -s ../gluon-build-dependencies/build/x86-kvm_guest/openwrt/bin build/x86-kvm_guest/openwrt/bin
    ln -s ../gluon-build-dependencies/build/x86-xen_domu/openwrt/bin build/x86-xen_domu/openwrt/bin
    
 
