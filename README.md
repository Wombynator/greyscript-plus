# greyscript-plus

Library to enhance GreyScript

# Overview

This project provides a robust and comprehensive set of functions for various use cases, including cryptography, event handling, logging mechanisms and general-purpose utilities.

# Modules and Functions

## Event
✔️ **event.on** Registers a function to be called when a specific event is triggered.<br>
✔️ **event.emit** Triggers all functions associated with a specific event.

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