# Writing a virus software development kit

These can come in handy when writing big projects, if you do not know what
they are used for, essentially we have a library that has a load of things to
help us, such as custom classes, structs, functions, etc.

## Getting started

First setup an appropriate testing environment and install the Visual Studio 2019 IDE along
with the visual C++ development kit.

You will need to make a new "blank" project and create a file structure looking like this..

```
Empty project
│   Source.cpp
│
└───SDK
    │   sdk.cpp
    └   sdk.hpp (or sdk.h)
```

Then once you complete this, open Source.cpp and include the sdk:

```c++
#include <iostream>
#include "SDK/sdk.hpp"

int main() { std::cout << "Hello world\r\n"; }
```

## Creating basic helper functions

This is your first step in making the SDK, it is the most simple too.

Open up `sdk.(h/hpp)` and create a function like this:

```c++
#include <iostream>

void warn(const char *string);
```

Then write some more code inside your function within `sdk.cpp`

```c++
#include "sdk.hpp"

void warn(const char *string) {
  std::cout << "\033[91m[!] \033[97m" << string << "\033[0m\r\n"; // Print red warning text
}
```

You can now use this function in the `Source.cpp` file!

## Notes

Try not to rely on guides when programming, it will help you in the long run and improve
your adaptability and problem-solving skills.
