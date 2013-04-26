Hacer resize de una imagen de sistema
=====================================

Para hacer resize debemos crear primero una nueva imagen vacia, con el nuevo tamano deseado

    dd bs=1M count=2500 if=/dev/zero of=ubuntu-new.img

Luego montarla como un dispositivo loop

    sudo losetup -f --show ubuntu-new.img

Montar la imagen original
  
    sudo losetup -f --show ubuntu.img

Copiar todo el contenido de la imagen pequeña a la nueva con mas tamaño

    sudo dd if=/dev/loop1 of=/dev/loop0

Hacemos un resize del limite de tamaño de la imagen, ya que lo hereda de la copia.

    sudo resize2fs ubuntu-new.img
    sudo e2fsck -f ubuntu-new.img 