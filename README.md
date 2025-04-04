# Makefile for executing syzkaller with extended syscalls and pseudo-syscalls

 
Step 1: Copy example3.txt into the directory /syzkaller/sys/linux/
Command: cp example3.txt /syzkaller/sys/linux/

Step 2: Copy common_linux.h into the directory /syzkaller/executor/
Command: cp common_linux.h /syzkaller/executor/

Step 3: Copy syscalls_linux.go into the directory /syzkaller/pkg/host/
Command: cp syscalls_linux.go /syzkaller/pkg/host/

Step 4: Copy my.cfg into the directory /syzkaller/
Command: cp my.cfg /syzkaller/

Step 5: Change into the directory /syzkaller/
Command: cd /syzkaller/

Step 6: Execute: make generate
Command: make generate

Step 7: Execute: make
Command: make

Step 8: Execute: sudo ./bin/syz-manager -config my.cfg
Command: sudo ./bin/syz-manager -config my.cfg


