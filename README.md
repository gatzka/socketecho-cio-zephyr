# Meta project for building autobahn websocket test using cio on zephyr OS.

## Howto Build
```

west init -m git@github.com:gatzka/socketecho-cio-zephyr.git socketecho-cio-zephyr
cd socketecho-cio-zephyr
west update
west build -b native_posix socketecho-cio-zephyr/
```


