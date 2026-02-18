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
3. Carete `ArduinoIgnore.h` file, it should define all the stuff you want to trim off the DLMS.c library. Check `gxignore.h` for a full list of `#defines` for stuff you can turn on/off.

    > `ArduinoIgnore.h` is automatically included by the library, you don't need to manually include it.
    > `ArduinoIgnore.h` is used by the library files, it's required to build the project. You must cerate it even if it's going to be empty (sorry about that).

4. Include the library in your source files:

    ```c
    #include "gx_dlms_c.h"
    ```
5. Write your code, build or verify, and download it.

