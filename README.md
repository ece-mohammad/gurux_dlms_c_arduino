# gx_dlms_c_arduino

Unofficial Gurux DLMS.c arduino library. 

## Introduction

Gurux provides open-source Gurux.DLMS.c, a platform independent, high performance, ANSI C component to implementation of DLMS/COSEM (Device Language Message Specification). This allows you to build applications (on PC, raspberry pi, micro-controllers) that act as either a DLMS Client (reading data from a smart meter) or a DLMS Server (emulating a meter).
Check out the official Gurux [DLMS.c repo](https://www.github.com/Gurux/GuruxDLMS.c) repository, and their [website](https://www.gurux.fi).

## Motivation

This is an un-official arduino library for the Gurux DLMS.c.

## Usage

1. Install library from Arduino IDE (1.5+)
2. Include the library in you code
3. Define your `gxignore.h` file, it should define all the stuff you want to trim off the DLMS.c library, and make sure to include it in your code before the library include

    ```c
    #include "gxignore.h"
    #include "gx_dlms_c.h"
    ```

