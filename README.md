# ColorLog
A libary full with color functions and console log functions of course!

# Installation
You can install the library in two different ways.

### Option 1
  1. Download the file from github.
  2. Move to file to your work folder.
  3. Add the script to the HTML file
  
  **IMPORTANT: Make sure the ColorLog.js file is above your main JavaScript file in the markup!**
  
  Example:
  
  ```
  <script src="ColorLog.js"></script>
  <script src="main.js"></script>
  ```
  
### Option 2
  Use the CDN:
  http://www.cdn.daankorver.com/library/ColorLog/ColorLog.js
  
  And paste it in the script as following:
  
  ```<script src="http://www.cdn.daankorver.com/library/ColorLog/ColorLog.js"></script>```
  
  **IMPORTANT: The CDN is not online yet so this option becomes available soon!**
  
  **IMPORTANT: Make sure the CND Link is above your main JavaScript file in the markup!**
  
  Example:
  
  ```
  <script src="http://www.cdn.daankorver.com/library/ColorLog/ColorLog.js"></script>
  <script src="main.js"></script>
  ```

# Docs

These are the current functions in the library:

## log
```
cl.log(message, color, background-color, font-size);
```
### -Message
The ```message``` paramater expects a string. This is the string that outputs in the console.

### -Color
The ```color``` paramater expects a string. This will set the text color.

### -Background-color
The ```background-color``` paramater expects a string. This will set the background color.

### -Font-size
The ```color``` paramater expects a string. This will set the font size.

This function can be used to log things with different styles.
You can use this function as followed:
```
cl.log("Hello World!", "Green", "#000", "20px");
```
The output wil be the following:

![Screenshot](assets/output1.png)

## error

```
cl.error(string)
```
### -String
The ```String``` paramater expects a string. This is the string that outputs in the console.
This function can be used to log a custom error.
You can use this function as followed:
```
cl.error("Whoops, an error occured here");
```
The output will be the following:

![Screenshot](assets/output2.png)

## isColorName

```
cl.isColorName(color);
```
### -Color
The ```color``` paramater expects a string. This is the color that will be checked on name.

```
//Returns false
cl.isColorName("greens");

//Returns true
cl.isColorName("green");
```

## isColorHex

```
cl.isColorHex(color);
```
The ```color``` paramater expects a string. This is the color that will be checked on hex value.
This function returns true if the color is a color based on its hex value. if this is not the case, it returns false.

```
//Returns False
cl.isColorHex("#fffff");

//Returns True
Returns True("#ffffff");
```
