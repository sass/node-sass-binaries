node-sass-binaries
==================

This repository contains the native bindings that are published to NPM as part of [node-sass](https://github.com/andrew/node-sass).

## Building bindings for Windows

When compiling the bindings for Windows, make sure to remove every instance of the following line from the Visual Studio project file (build/binding.vcxproj)

```xml
<RuntimeTypeInfo>false</RuntimeTypeInfo>
```

This line is known to cause some incompatibility with libsass and node.js.

[More details about the node-gyp issue](https://github.com/TooTallNate/node-gyp/issues/335)

## Copyright

Copyright (c) 2013 Andrew Nesbitt. See [LICENSE](https://github.com/andrew/node-sass-binaries/blob/master/LICENSE) for details.
