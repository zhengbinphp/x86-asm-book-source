
ASMFILE=c05_mbr.asm

.PHONY: all clean

all:$(ASMFILE)
	nasm -f bin $(ASMFILE) -o mbr.bin
	VBoxManage convertfromraw mbr.bin myfile.vhd --format VHD --variant Fixed

clean:
	rm -rf *.vhd *.bin