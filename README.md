# kong-plugins-lua

Sharing some Kong plugins for lua.

## Overview



## Develop





## Distribution

* download plugins source by git

```
git clone git@github.com:mark0725/kong-plugins-lua.git
```

* Docker run

```
-v "$kong_plugins_lua_folder:/app/kong_plugins_lua" 
-e "KONG_LUA_PACKAGE_PATH=/app/kong_plugins_lua/?.lua;;"
-e "KONG_PLUGINS=bundled,plugin1,plugin2"
```

* environment

```
export KONG_LUA_PACKAGE_PATH=""/app/kong_plugins_lua/?.lua;;"
export KONG_PLUGINS="bundled,plugin1,plugin2"
```

* kong.conf

```
lua_package_path = /app/kong-plugins-lua/?.lua;;
plugins = bundled,plugin1,plugin2
```

> kong plugins doc: https://docs.konghq.com/gateway/latest/plugin-development/distribution/

## License

This project is licensed under the [MIT license](LICENSE).
