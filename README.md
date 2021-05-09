# TCP Chat Room

Python implementation of a chat room using TCP protocol.

## Requirements

Plain Python 3, nothing more required. Version 3.8+ recommended.

## Usage

Run the server with `python server.py`. Add clients in other terminals with `python client.py`
and start chatting in the command line. If using multiple machines, change server address
accordingly.

On Windows, prefer the CMD as the Git-Bash console does not work well with background
threads.

## Features

### Messaging

Only broadcast messages supported: all other clients in the chat room receive your
messages.

### Commands

Supported commands:
* `/admin` -- become admin
* `/quit` -- quit the chat room
* `/exit` -- same as `/quit`
  
Supported admin commands:
* `/online` -- show online users list
* `/kick abc` -- kick user `abc`
* `/ban abc` -- kick and ban user `abc` (prevent reconnection)
* `/unban abc` -- unban user `abc` (remove from ban list)
* `/banned` -- show banned users list

