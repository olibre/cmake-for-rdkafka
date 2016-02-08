CMake encapsulation for the [librdkafka][1]
-------------------------------------------

The project [librdkafka][1] does not provide CMake.  
Therefore, to build it, you can use the provided script `./configure`.  
This project aims to provide a CMake encapsulation.

[1]: https://github.com/edenhill/librdkafka

Example to use this CMake encapsulation
----------------------------------------

```CMake
cmake_minimum_required(VERSION 2.8)
project(myProject)
add_executable(my.exe somefile.c)

include(some/path/rdkafka.cmake)                # Include the CMake encapsulation
target_link_libraries(my.exe rdkafka::rdkafka)  # Link to target rdkafka::rdkafka
```

License
-------

[CC0 1.0 Universal - Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, olibre (olibre@Lmap.org)
has waived all copyright and related or neighboring rights
to cmake-for-rdkafka (this README.md and CMake work).
This work is published in 2016 from France. 

Anybody can copy, modify, distribute and perform the work,
even for commercial purposes, all without asking permission.


