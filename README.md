# Greyscript Plus Library for game [Grey Hack](https://store.steampowered.com/app/605230/Grey_Hack/)

Library to enhance the ingame language GreyScript ([documentation](https://documentation.greyscript.org/))

# Installation

## Option 1: Clone the Repository Using [Git](https://git-scm.com/downloads)
1. Open your terminal.
2. Clone the repository by running the following command:
```sh
git clone https://github.com/Wombynator/greyscript-plus.git
```
3. Navigate to the project directory:
```sh
cd greyscript-plus
```

## Option 2: Download the ZIP
1. Download the ZIP file from [this link](https://github.com/Wombynator/greyscript-plus/archive/refs/heads/main.zip).
2. Extract the downloaded ZIP file.
3. Navigate to the extracted directory.

## Usage
1. Import the library into your script using the relative path:
```lua
import_code("greyscript-plus/gsp.src")
```
2. You're now set up and ready to use the Greyscript Plus functions and tools in your project.

# Table of Contents

- [**Functions**](#functions)
  - [Event](#event)
      - [`event.on`](#%EF%B8%8F-eventon-eventname-string-func-function-void)
      - [`event.emit`](#%EF%B8%8F-eventemit-eventname-string-void)
  - [Logger](#logger)
    - [`logger.info`](#%EF%B8%8F-loggerinfo-source-string-message-string-null)
    - [`logger.debug`](#%EF%B8%8F-loggerdebug-source-string-message-string-null)
    - [`logger.trace`](#%EF%B8%8F-loggertrace-source-string-message-string-null)
    - [`logger.warn`](#%EF%B8%8F-loggerwarn-source-string-message-string-null)
    - [`logger.error`](#%EF%B8%8F-loggererror-source-string-message-string-null)
    - [`logger.fatal`](#%EF%B8%8F-loggerfatal-source-string-message-string-null)
  - [Map](#map)
    - [`map.add`](#%EF%B8%8F-mapadd-key-string-value-any-map)
  - [Number](#number)
    - [`number.toOct`]()
    - [`number.toBin`]()
    - [`number.toHex`]()
  - [String](#string)
    - [`string.bytes`]()
    - [`string.encodeUtf8`]()
    - [`string.decodeUtf8`]()
    - [`string.encodeUrl`]()
    - [`string.decodeUrl`]()
    - [`string.encodeBase64`]()
    - [`string.decodeBase64`]()
    - [`string.toOct`]()
    - [`string.toBin`]()
    - [`string.toHex`]()
    - [`string.toInt`]()
    - [`string.zfill`]()
    - [`string.reverse`]()
    - [`string.isLower`]()
    - [`string.isUpper`]()
    - [`string.isIn`]()
    - [`string.isAlnum`]()
    - [`string.isAlpha`]()
    - [`string.lstrip`]()
    - [`string.rstrip`]()
    - [`string.strip`]()
    - [`string.removeTags`]()
    - [`string.startsWith`]()
    - [`string.endsWith`]()
    - [`string.color`]()
    - [`string.mark`]()
  - [Globals](#globals)
    - [`__name__`]()
- [**Modules**](#modules)
  - [Colormap](#colormap)

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
✔️ **number.toOct** Converts a number into its octal form.<br>
✔️ **number.toBin** Converts a number into its binary form.<br>
✔️ **number.toHex** Converts a number into its hexadecimal form.

## String
✔️ **string.bytes** Converts a string into an array of bytes.<br>
✔️ **string.encodeUtf8** Encodes a string to its UTF-8 representation.<br>
✔️ **string.decodeUtf8** Decodes a string from its UTF-8 representation.<br>
✔️ **string.encodeUrl** Encodes a string to Url format.<br>
✔️ **string.decodeUrl** Decodes a string from Url format.<br>
✔️ **string.encodeBase64** Encodes a string to Base 64.<br>
✔️ **string.decodeBase64** Decodes a string from Base 64.<br>
✔️ **string.toOct** Converts the string representation of a number into its octal form.<br>
✔️ **string.toBin** Converts the string representation of a number into its binary form.<br>
✔️ **string.toHex** Converts the string representation of a number into its hexadecimal form.<br>
✔️ **string.toInt** Converts a string representation of a number into an integer.<br>
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

## Globals

### ✔️ `__name__ (): string`

# Modules

## Colormap
- A global color map accessible via dot notation. For example, `print colorMap.red` would output the hexadecimal color code `#FF0000`.

Color | Code | Preview
--- | --- | ---
red | #FF0000 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF0000)](https://www.colorhexa.com/FF0000)
maroon | #800000 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-800000)](https://www.colorhexa.com/800000)
brown | #856256 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-856256)](https://www.colorhexa.com/856256)
tomato | #FF5533 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF5533)](https://www.colorhexa.com/FF5533)
chocolate | #D2691E | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-D2691E)](https://www.colorhexa.com/D2691E)
orange | #FFAA00 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFAA00)](https://www.colorhexa.com/FFAA00)
gold | #C3A200 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-C3A200)](https://www.colorhexa.com/C3A200)
yellow | #FFFF00 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFFF00)](https://www.colorhexa.com/FFFF00)
light green | #90EE90 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-90EE90)](https://www.colorhexa.com/90EE90)
olive | #808000 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-808000)](https://www.colorhexa.com/808000)
green | #008000 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-008000)](https://www.colorhexa.com/008000)
alien | #55DD00 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-55DD00)](https://www.colorhexa.com/55DD00)
lime | #00FF00 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-00FF00)](https://www.colorhexa.com/00FF00)
cyan | #00FFFF | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-00FFFF)](https://www.colorhexa.com/00FFFF)
turquoise | #40E0D0 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-40E0D0)](https://www.colorhexa.com/40E0D0)
teal | #008080 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-008080)](https://www.colorhexa.com/008080)
light blue | #ADD8E6 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-ADD8E6)](https://www.colorhexa.com/ADD8E6)
deep sky blue | #55AAFF | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-55AAFF)](https://www.colorhexa.com/55AAFF)
blue | #0000FF | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-0000FF)](https://www.colorhexa.com/0000FF)
slate blue | #6A5ACD | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-6A5ACD)](https://www.colorhexa.com/6A5ACD)
navy | #000080 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-000080)](https://www.colorhexa.com/000080)
midnight blue | #191970 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-191970)](https://www.colorhexa.com/191970)
indigo | #4B0082 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-4B0082)](https://www.colorhexa.com/4B0082)
purple | #800080 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-800080)](https://www.colorhexa.com/800080)
magenta | #FF00FF | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FF00FF)](https://www.colorhexa.com/FF00FF)
violet | #EE82EE | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-EE82EE)](https://www.colorhexa.com/EE82EE)
orchid | #DD99CC | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-DD99CC)](https://www.colorhexa.com/DD99CC)
salmon | #FA8072 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FA8072)](https://www.colorhexa.com/FA8072)
pink | #FFC0CB | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFC0CB)](https://www.colorhexa.com/FFC0CB)
black | #000000 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-000000)](https://www.colorhexa.com/000000)
gray | #808080 | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-808080)](https://www.colorhexa.com/808080)
silver | #A8ABAE | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-A8ABAE)](https://www.colorhexa.com/A8ABAE)
white | #FFFFFF | [![](https://img.shields.io/badge/%E3%85%A4%E3%85%A4%E3%85%A4%E3%85%A4-FFFFFF)](https://www.colorhexa.com/FFFFFF)