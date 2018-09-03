```
(gdb) bt
#0  dlsym_doit (a=a@entry=0x7fffffffddf0) at dlsym.c:47
#1  0x00007ffff7947c5c in __GI__dl_catch_exception (
    exception=exception@entry=0x7fffffffdd90, 
    operate=0x7ffff7bd3070 <dlsym_doit>, args=0x7fffffffddf0)
    at dl-error-skeleton.c:196
#2  0x00007ffff7947ccf in __GI__dl_catch_error (
    objname=0x7ffff7dd50d0 <last_result+16>, 
    errstring=0x7ffff7dd50d8 <last_result+24>, 
    mallocedp=0x7ffff7dd50c8 <last_result+8>, operate=<optimized out>, 
    args=<optimized out>) at dl-error-skeleton.c:215
#3  0x00007ffff7bd3595 in _dlerror_run (
    operate=operate@entry=0x7ffff7bd3070 <dlsym_doit>, 
    args=args@entry=0x7fffffffddf0) at dlerror.c:163
#4  0x00007ffff7bd30df in __dlsym (handle=<optimized out>, 
    name=<optimized out>) at dlsym.c:70
#5  0x0000555555554847 in main (argc=2, argv=0x7fffffffdf48) at main.c:14

```
