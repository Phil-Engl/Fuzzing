# For results, see report.pdf in this repository

 
# Step 1: Copy files into destined directories

cp example3.txt /syzkaller/sys/linux/

cp common_linux.h /syzkaller/executor/

cp syscalls_linux.go /syzkaller/pkg/host/

cp my.cfg /syzkaller/


# Step 2: Build files

cd /syzkaller/

make generate

make

# Step 3: Execute

sudo ./bin/syz-manager -config my.cfg
