# Mumonkan

This is my own minimalistic Ruby & Rails development oriented distrib of Vim editor.

![mumonkan.png](https://github.com/romanvbabenko/mumonkan/raw/master/mumonkan.png)

## Converts and unconverts hashrocket notation

    :Hashrockets   {foo: 'bar', boston: 'rocks'}        ==>   {:foo => 'bar', :boston => 'rocks'}
    :Bashrockets   {:foo => 'bar', :boston => 'rocks'}  ==>   {foo: 'bar', boston: 'rocks'}

another way

    :%s/\(\w*\): \([':]\)/:\1 => \2/g # Bashrockets => Hashrockets
    %s/:\([^=,'"]*\) =>/\1:/g # Hashrockets => Bashrockets

## Requirements

* Vim 7.0 or later
* Git (optional)
* RVM (optional)

