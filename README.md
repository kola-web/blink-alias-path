# blink-alias-path

support webpack alias path

![preview](/data/preview1.png)


# Features

1. support for alias path

# Quick Start

```lua
return {
  {
    "saghen/blink.cmp",
    dependencies = {
      "xieyonn/blink-cmp-dat-word",
    },
    opts = {
      sources = {
        default = { 'aliasPath' },
        providers = {
          aliasPath = {
            name = 'aliasPath',
            module = 'blink-alias-path',
            opts = {
              ignore_root_slash = false,
              path_mappings = {
                ['@'] = '${folder}/src',
                ['/'] = '${folder}/src/',
              },
            },
          },
        },
      },
    },
  },
}
```
