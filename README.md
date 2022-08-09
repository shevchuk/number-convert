# number-convert
Hexadecimal to decimal and vice versa at point.
The conversion isn't too smart so some formattings are not handled properly (e.g. 0xFF)

Usage:

`M-x number-convert/hex-to-dec-at-point RET`


    82297E -> 8530302
    FF -> 255

`M-x number-convert/dec-to-hex-at-point RET`

    255 -> FF
    256 -> 100


The following keybindings might be nice to use:

``` lisp
(global-set-key (kbd "C-c C-n d") 'number-convert/hex-to-dec-at-point)
(global-set-key (kbd "C-c C-n h") 'number-convert/dec-to-hex-at-point)
```
