# greyscript-plus

Library to enhance GreyScript

# Overview

This project provides a robust and comprehensive set of functions for various use cases, including cryptography, event handling, logging mechanisms and general-purpose utilities.

# Table of Contents

- [Event](#event)
    - [event.on](#%EF%B8%8F-eventon-eventname-string-func-function-void)
    - [event.emit](#%EF%B8%8F-eventemit-eventname-string-void)
- [Functions](#functions)
  - [Function1](#function1)
  - [Function2](#function2)
  - [Function3](#function3)
  - [Function4](#function4)
- [Contributing](#contributing)
- [License](#license)

# Modules and Functions

## Event
### ✔️ `event.on (eventName: string, func: function): void`
Registers a function to be called when a specific event is triggered.
### Description:
- This function allows registering one or more callback functions (`func`) to be executed when an event with the specified name (`eventName`) is emitted.
### Parameters:
- `eventName: string` The name of the event to which the function is to be registered.
- `func: function` The callback function to be executed when the event is emitted.
### Example:
```lua
event.on("userLogin", @loginUserFunction)
```
*Registers `loginUserFunction` to be called when `userLogin` event is emitted*

---
### ✔️ `event.emit (eventName: string): void`
### Description
- Triggers all functions associated with a specific event.
### Example
```lua
event.on("userLogin", @loginUserFunction)
```
*Registers `loginUserFunction` to be called when `userLogin` event is emitted*
✔️ **event.emit** 

## Logger
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
✔️ **string.encodeUtf8** Encodes a single character to its UTF-8 representation.<br>
✔️ **string.encodeUrl** Encodes a string to Url format.<br>
❌ **string.decodeUrl** Decodes a string from Url format.<br>
✔️ **string.encodeBase64** Encodes a string to Base 64.<br>
❌ **string.decodeBase64** Decodes a string from Base 64.<br>
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