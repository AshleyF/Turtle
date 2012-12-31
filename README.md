# Turtle Graphics #

A very simple Turtle Graphics implementation using HTML5 canvas and JavaScript. Usage instructions are available on the web page (Default.htm). For example, this draws a “galaxy”:

> `0(1adf89r)180x`

Give it a try: http://brief.azurewebsites.net/archive/turtle/?(320dg0(1adf89r)720x1lc)1000x

There's also a YouTube demo here: http://www.youtube.com/watch?v=CVFcpoULWq4

It is driven by a tiny stack language allowing single-character commands to move the turtle and draw and do animations. Quotations are used to treat code as data (pushed to the stack); allowing repetition and definition of new commands.

> `h` Home - Reset x,y to 160,160

> `n` North - Reset bearing

> `g` Go - Sets x,y from stack `10,20g`

> `c` Clear - Clears canvas (useful for animation)

> `f` Forward - Draws forward n pixels `10f`

> `m` Move - Moves forward n pixels `10m`

> `l` Left - Turn bearing left n degrees `90l`

> `r` Right - Turn bearing right n degrees `90r`

> `x` Repeat - Repeats quotation n times `(100f90r)4x`

> `a` Add - Adds two numbers `4,2a`

> `-` Subtract - Subtracts two numbers `4,2-`

> `*` Multiply - Multiplies two numbers `4,2*`

> `v` Divide - Divides two numbers `4,2v`

> `j` Join - Prepends head onto quotation `10(f90r)c`

> `u` Unjoin - Separates head from tail `(10f90r)u`

> `d` Dup - Duplicates top stack value

> `w` Swap - Swaps top two stack values

> `o` Drop - Discards top stack value

> `i` Dip - Applies quote below next value `10,20(f)i`

Parenthesis surround quotations `(100f90r)`.

Digits [0123456789] build decimal numbers. Commas separate adjacent numbers.

Define unused characters by following quotation. `(90r)R` defines `R` as substitution for `90r`.

Canvas is 320x320. Turtle begins at 160,160 bearing North.
