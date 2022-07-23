# RGB to hex snippet

Converts said rgb value to hexadecimal value

``` cpp
/**
 * @brief Converts a rgb value to hexadecimal value
 * @param r red channel
 * @param g green channel
 * @param b blue channel
 * @returns hexadecimal value without alpha.
 */
 unsigned long rgbToHex(int r, int g, int b)
 {   
     return ((r & 0xff) << 16) + ((g & 0xff) << 8) + (b & 0xff);
 }

/**
 * @brief Converts a rgba value to hexadecimal value
 * @param r red channel
 * @param g green channel
 * @param b blue channel
 * @param a alpha channel
 * @returns hexadecimal value without alpha.
 */
unsigned long rgbaToHex(int r, int g, int b, int a)
{   
    return ((r & 0xff) << 24) + ((g & 0xff) << 16) + ((b & 0xff) << 8) + (a & 0xff);
}

```

``` cpp
unsigned long rgbValue = rgbToHex(76, 174, 80);
unsigned long rgbaValue = rgbToHex(76, 174, 80, 125);

printf(rgbValue);
printf(rgbaValue);

```
