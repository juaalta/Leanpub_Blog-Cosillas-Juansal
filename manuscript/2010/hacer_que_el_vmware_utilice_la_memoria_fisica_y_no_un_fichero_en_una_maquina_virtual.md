{:: encoding="utf-8" /}
## Hacer que el VMware utilice la memoria física y no un fichero en una máquina virtual {#2010_06}

Para conseguir esto hay que modificar el fichero .vmx de la máquina virutal y añadir/modificar las siguientes entradas:

```
mainMem.useNamedFile = "FALSE"
MemAllowAutoScaleDown = "FALSE"
MemTrimRate = "0"
sched.mem.pshare.enable = "FALSE"
```
