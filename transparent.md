# Testing transparency formula

https://www.viget.com/articles/equating-color-and-transparency/

background * (1 - opacity) + overlay * opacity = target

(204 - 255) / (0 - 255) = 0.2

Color * opcaity = new color
255 * .80 = 204

42 * .5 = 21
255 * .5 =

Red
255 * (.5 - 1) + 42 * .5 = target
255 * .5 + 42 * .5 = 148.5 round 149

Green
127.5 + 132 * .5 = 193.5 round 194

Blue
127.5 + 192 * .5 = 223.5 round 224

overlay color
rgba(42, 132, 192, 0.5)

Bg color
rgb(255, 255, 255)

resulting overlay color
rgb(154, 194, 224)

rgb(149, 194, 224)



---

background * (opacity - 1) + overlay * opacity = target

overlay
rgba(36, 39, 40, 0.7)

bg
rgb(183, 52, 52)

resulting
rgb(81, 43, 44)
actual
rgb(80, 43, 44)

r
183 * .3 + 36 * 0.7 = 80.1

g
52 * .3 + 39 * 0.7 = 43

b
52 * .3 + 40 * 0.7 = 44

---

background * (opacity - 1) + overlay * opacity = target

overlay
rgba(230, 237, 239, 0.5)
bg
rgb(227, 13, 13)
resulting
rgb(232, 138, 134)
actual
rgb(228.5, 125, 126)

r
227 * .5 + 230 * .5 = 228.5

g
13 * .5 + 237 * .5 = 125

b
13 * .5 + 239 * .5 = 126



----------------

overlay
rgba(255, 255, 255, 0.6)

bg
rgb(255, 0, 0)

results
rgb(255, 169, 164)

actual
rgb(255, 153, 153)

r
255 * .4 + 255 * .6 = 255

g
0 * .4 + 255 * .6 =  153

b
0 * .4 + 255 * .6 = 153
