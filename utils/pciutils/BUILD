default_make &&

mkdir -p /usr/include/pci/ &&
install lib/{pci,header,types,config}.h /usr/include/pci/ &&
ln -sf /usr/lib/libpci.so.$(module_version pciutils) /usr/lib/libpci.so &&
bunzip2 $SOURCE_CACHE/$SOURCE2 -c > pci.ids &&
rm -f /usr/share/pci.ids* &&
install -m644 pci.ids /usr/share &&
install -D -m644 lib/libpci.pc /usr/lib/pkgconfig/libpci.pc &&

# the next line makes sure you will get a fresh pci id's db
# everytime you lin pciutils:
rm -f $SOURCE_CACHE/$SOURCE2
