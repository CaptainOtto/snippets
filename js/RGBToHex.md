# RGB to hex snippet

The color we will convert and the result value: #4CAE50

![image](https://user-images.githubusercontent.com/16833945/180598827-9c0f5ca2-3562-4187-ab4b-1276d3366e68.png)


Converts said rgb value to hexadecimal value

``` js

/**
 * @brief Converts a rgb value to hexadecimal value
 * @param r red channel
 * @param g green channel
 * @param b blue channel
 * @returns hexadecimal value without alpha.
 */
const rgbToHex = (r, g, b) => {
  return "#" + ((r << 16) + (g << 8) + b).toString(16).padStart(6, '0');
};

```

``` js

hexValue = rgbToHex(76, 174, 80);
console.log(hexValue); // prints out #4cae50

```

