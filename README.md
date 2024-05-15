# greyscript-plus

Library to enhance GreyScript

# Overview

This project provides a robust and comprehensive set of functions for various use cases, including cryptography, event handling, logging mechanisms and general-purpose utilities.

# Table of Contents

- [**Functions**](#functions)
  - [Event](#event)
      - [`event.on`](#%EF%B8%8F-eventon-eventname-string-func-function-void)
      - [`event.emit`](#%EF%B8%8F-eventemit-eventname-string-void)
  - [Logger](#logger)
    - [`logger.info`](#%EF%B8%8F-eventon-eventname-string-func-function-void)

# Functions

## Event

### ✔️ `event.on(eventName: string, func: function): void`
Registers a callback function for a specific event.

#### Parameters:
- `eventName: string` - Name of the event.
- `func: function` - Callback function to be executed when the event occurs.

#### Example:
```lua
event.on("userLogin", @loginUserFunction)
```
*Registers `loginUserFunction` to be called when the `userLogin` event is emitted.*

---

### ✔️ `event.emit(eventName: string): void`
Triggers all callback functions associated with a specific event.

#### Parameters:
- `eventName: string` - Name of the event.

#### Example:
```lua
event.emit("userLogin")
```
*Triggers execution of all functions registered under the `userLogin` event.*

---

## Logger

### ✔️ `logger.info (source: string, message: string): null`
Logs an informational message.

#### Parameters:
- `source: string` - The source module or component that generated the log message.
- `message: string` - The informational message to log.

#### Example:
```lua
logger.info("main", "Info message...")
```
*Outputs*
![]()

---

✔️ **logger.info** Logs an informational message.<br>
✔️ **logger.debug** Logs a debug message.<br>
✔️ **logger.trace** Logs a trace message.<br>
✔️ **logger.warn** Logs a warning message.<br>
✔️ **logger.error** Logs an error message.<br>
✔️ **logger.fatal** Logs a fatal error message.

## Map
✔️ **map.add** Adds a key-value pair to a map.

## Number
✔️ **number.to_oct** Converts a number into its octal form.<br>
✔️ **number.to_bin** Converts a number into its binary form.<br>
✔️ **number.to_hex** Converts a number into its hexadecimal form.

## String
✔️ **string.bytes** Converts a string into an array of bytes.<br>
✔️ **string.encodeUtf8** Encodes a string to its UTF-8 representation.<br>
✔️ **string.decodeUtf8** Decodes a string from its UTF-8 representation.<br>
✔️ **string.encodeUrl** Encodes a string to Url format.<br>
✔️ **string.decodeUrl** Decodes a string from Url format.<br>
✔️ **string.encodeBase64** Encodes a string to Base 64.<br>
✔️ **string.decodeBase64** Decodes a string from Base 64.<br>
✔️ **string.to_oct** Converts the string representation of a number into its octal form.<br>
✔️ **string.to_bin** Converts the string representation of a number into its binary form.<br>
✔️ **string.to_hex** Converts the string representation of a number into its hexadecimal form.<br>
✔️ **string.to_int** Converts a string representation of a number into an integer.<br>
✔️ **string.zfill** Fills the string with leading zeros to reach a specified width.<br>
❌ **string.lfill** Fills the string with leading characters to reach a specified width.<br>
❌ **string.rfill** Fills the string with ending characters to reach a specified width.<br>
✔️ **string.reverse** Reverses the order of characters in a string.<br>
✔️ **string.isLower** Checks if the string is entirely in lowercase.<br>
✔️ **string.isUpper** Checks if the string is entirely in uppercase.<br>
✔️ **string.isIn** Checks if the current string is contained within the specified string.<br>
✔️ **string.isAlnum** Checks if the string consists only of alphanumeric characters.<br>
✔️ **string.isAlpha** Checks if the string consists only of alphabetic characters.<br>
✔️ **string.strip** Strips characters from both ends of a string.<br>
✔️ **string.lstrip** Strips characters from the beginning of a string.<br>
✔️ **string.rstrip** Strips characters from the end of a string.<br>
✔️ **string.removeTags** Removes TextMesh Pro tags from a string.<br>
✔️ **string.startsWith** Checks if a string starts with the specified substring.<br>
✔️ **string.endsWith** Checks if a string ends with the specified substring.<br>
✔️ **string.color** Applies a color to a string using both hexadecimal codes and named colors.<br>
✔️ **string.mark** Applies a highlight to a string using both hexadecimal codes and named colors.

## Colormap
- A global color map accessible via dot notation. For example, `print colorMap.red` would output the hexadecimal color code `#FF0000`.

Color | Code | Preview
--- | --- | ---
red | #FF0000 | <img src="https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF0000" alt="Badge" class="non-clickable">
maroon | #800000 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-800000)
brown | #856256 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-856256)
tomato | #FF5533 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF5533)
chocolate | #D2691E | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-D2691E)
orange | #FFAA00 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFAA00)
gold | #C3A200 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-C3A200)
yellow | #FFFF00 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFFF00)
light green | #90EE90 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-90EE90)
olive | #808000 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-808000)
green | #008000 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-008000)
alien | #55DD00 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-55DD00)
lime | #00FF00 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-00FF00)
cyan | #00FFFF | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-00FFFF)
turquoise | #40E0D0 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-40E0D0)
teal | #008080 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-008080)
light blue | #ADD8E6 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-ADD8E6)
deep sky blue | #55AAFF | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-55AAFF)
blue | #0000FF | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-0000FF)
slate blue | #6A5ACD | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-6A5ACD)
navy | #000080 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-000080)
midnight blue | #191970 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-191970)
indigo | #4B0082 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-4B0082)
purple | #800080 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-800080)
magenta | #FF00FF | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF00FF)
violet | #EE82EE | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-EE82EE)
orchid | #DD99CC | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-DD99CC)
salmon | #FA8072 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FA8072)
pink | #FFC0CB | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFC0CB)
black | #000000 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-000000)
gray | #808080 | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-808080)
silver | #A8ABAE | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-A8ABAE)
white | #FFFFFF | ![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFFFFF)