# Python Cheatsheet

Cheatsheet for Python3

## Lists

|         Command         |            Explanation             |
| :---------------------: | :--------------------------------: |
|       `list = []`       |            create list             |
|       `list[i:j]`       |           return susbet            |
|       `list[-1]`        |        return last element         |
|       `list[:-1]`       | return all except for last element |
|     `list[i] = val`     |      assign value to element       |
| `list[i:j] = otherlist` |   replace subset with other list   |
|     `del list[i:j]`     |           delete subset            |
|   `list.append(item)`   |        append item to list         |

## General

### Basics

print: print(VAR|"STRING")

### Loops

if-loop

```python
if STATEMENT:
    action
```

### Scripting

| Description |      Syntax       |
| :---------: | :---------------: |
| User Input  | `input("TEXT: ")` |
| Exit Script |     `exit()`      |

## Useful Modules

- HTTP Server: `python3 -m http.server 80`
- SMTP Server: `python3 -m smtpd -n -c DebuggingServer localhost:25`

## Syntax

Sockets

```python
import socket

s = socket.socket
s.connect
```
