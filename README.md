# ft_printf

## Table of Contents
- [Overview](#overview)
- [Requirements](#requirements)
- [Build](#build)
- [Usage](#usage)
    - [Example](#example)
- [Lisence](#lisence)

## Overview

`ft_printf` is subset implemention of the C `printf` function. Supported flags are:

- %c Prints single charater
- %s Prints a string
- %p Prints pointer in hex format
- %d Prints deciaml (base 10) number
- %i Prints an interger in base 10
- %u Prints an unsigned deciaml (base 10) number
- %x Prints a number in hex lowercase format
- %x Prints a number in hex uppercase format
- %% Prints a percent sign

## Requirements

This library have zero dependency, all you need is a C compiler and the `ar` archiver. The Included Makefile is configured to use `cc`. You can use your compile of choice.

## Build

To build The library, cd into `src` and run the following command

```sh
make
```

This will result in a `libftprintf.a` file which is a archive file containing all our object files. Which implements the library.

## Usage

To use `libftprintf` in your project include it in your src files list or as a argument to your C compiler.

### Example

This is a example compiling a `main.c` file using `libft.a` static library

```sh
gcc libft.a main.c -o main
```

main.c:

```c
#include "ft_printf.h"

void main() {
    char *str = "hello world";
    ft_printf("%s\n", str);
}
```


## Lisence

This project is licensed under MIT license. See the LICENSE file for details.
