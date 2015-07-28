# nodemcu-mode

NodeMCU helper minor mode for Emacs.

This mode allows to communicate with [NodeMCU-firmware][nodemcu] in order to help Lua-scripts development.

[nodemcu]: https://github.com/nodemcu/nodemcu-firmware "NodeMCU-firmware"

## Features

* Communicating using serial device or telnet connection.
* Executing Lua code and evaluate Lua expressions on device.
* Listing uploading and removing files on/to/from device.
* Compiling Lua scripts after uploading to device.
* Some other useful commands.

## Bindings

| Key     | Command                   | Description                                      |
| ------- | ------------------------- | ------------------------------------------------ |
| C-x C-e | nodemcu-evaluate-at-point | Evaluate current line or marked region on device |
| C-c C-b | nodemcu-send-buffer       | Execute current buffer on device                 |
| C-c C-d | nodemcu-remove-file       | Remove file from device (with completion)        |
| C-c C-e | nodemcu-evaluate          | Evaluate some Lua-code on device                 |
| C-c C-h | nodemcu-get-heap          | Get heap size (node.heap())                      |
| C-c C-r | nodemcu-restart-node      | Restart node (node.restart())                    |
| C-c C-s | nodemcu-list-files        | List files on device file-system (file . size)   |
| C-c C-t | nodemcu-execute           | Execute some Lua-code on device                  |
| C-c C-u | nodemcu-upload-file       | Upload some local file local to device           |

## Hacking

You can activate Debugging IO using `nodemcu-debug-io` variable.
