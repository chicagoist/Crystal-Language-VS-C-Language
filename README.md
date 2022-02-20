## Crystal language vs. C language
compare Array with 1000 elements sorting


## Make speedTest.sh executable:
```$ chmod +x speedTest.sh```

## Compile C and Crystal with no optimizations:
Crystal:

```$ crystal build crystal.cr```

C:

```$ gcc c.c -o cNop -O0```

## Compile C and Crystal with optimizations:
Crystal:

```$ crystal build crystal.cr --release```

C:

```$ gcc c.c -o cOp -O3```


##
##

`C  No  optim:`

linux@thinkpad:$ `  ./speedTest.sh   ./cNop` 

Average: ``  real 0.382 user 0.379 sys 0.000``

`Crystal  No  optim:`

linux@thinkpad:$ `  ./speedTest.sh   ./crystalNop` 

Average: ``  real 5.083 user 5.045 sys 0.001``
#
#

`C  Optim:`
                                                                                                       
linux@thinkpad:$ `  ./speedTest.sh   ./cOp`                         

Average: ``  real 0.112 user 0.111 sys 0.000``
` `


`Crystal  Opt:`
                                                                                                       
linux@thinkpad:$ `  ./speedTest.sh   ./crystalOp`                         

Average: ``  real 0.219 user 0.217 sys 0.000``
                                                                                                       

