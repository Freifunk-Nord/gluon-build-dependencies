gluon-build-dependencies
========================

Dieses Repo enthällt alle Dateien die während des make Prozesses vom gluon make Script heruntergeladen werden müssen. Dies beugt Problemen
vor, die durch nicht erreichbare Server beim Kompilieren entstehen können.

Anwendung:
-------------------------------------
 
### # Repository clonen
 
    mkdir git-repo
    cd git-repo
    git clone https://github.com/Freifunk-Nord/gluon-build-dependencies
    git clone https://github.com/freifunk-gluon/gluon.git
    cd gluon
 
### # Ordnerstruktur anlegen
 
    mkdir openwrt
    for TARGET in ar71xx-generic ar71xx-mikrotik ar71xx-nand brcm2708-bcm2708 brcm2708-bcm2709 mpc85xx-generic ramips-mt7621 ramips-rt305x sunxi x86-64 x86-generic x86-kvm_guest x86-xen_domu; do
      mkdir -p build/$TARGET/openwrt
    done

### # Symlinks setzen

    ln -s ../gluon-build-dependencies/openwrt/dl openwrt/dl
    for f in build/*/openwrt/bin; do echo ln -s "../gluon-build-dependencies/$f" "$f"; done

