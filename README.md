# _printf

 `_printf`: is a replica of c standar library function printf. This function writes under the control of a format to the stdout. 


## Prototype

`int _printf(const char *format, ...);`


### Usage

Once cloned over, the repository must contain the following files:

| File  	| Description   |
| ------------- | ------------- |
| _printf.c     | main file of the function         |
| main.h        | _printf header                    |
| func.c        | contains all the formats admitted.|
| get_func.c 	| calls the concerned function	    |
| pch.c    	| one byte printer      	    |

Example:

```
#include "main.h"

void main(void)
{
	_printf("String");
}
```

Once compiled...

Output:

```
$ ./a.out
String$
```


### Conversion Specifiers

__The conversion specifiers that__ `_printf` __accepts are:__

* __s:__ The `char *` argument given, will print the string (except the '\0' byte).
* __c:__ The `char ` argument given, will print the byte.
* __i__ & __d__: The `int`. argument given, will print the integer. 

Note that you can write `%%`, and you will obtain `%` as output.

### Return Value

Upon succeful excecution, `_printf` will return the number of bytes printed (excluded the '\0' byte). Upon a error output the return value will be `-1`.


## Authors

* Alejandro Martinez [Git Hub](https://github.com/alemao51092)
* Emanuel Trias [Git Hub](https://github.com/KrasniKot)
