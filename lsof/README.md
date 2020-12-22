# version
4.94.0

# build
```
LSOF_CC=/usr/bin/gcc LSOF_CFGF='-DHAS_STRFTIME -DHASNORPC_H -DGLIBCV'  ./Configure -n linux
make
gcc -o lsof -static dfile.o dmnt.o dnode.o dproc.o dsock.o dstore.o arg.o main.o misc.o node.o print.o proc.o store.o usage.o util.o -L./lib -llsof
```

