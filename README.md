Simple palette management in p5js. Publishing all of my daily driver spaghettios for others to benchmark.

```js
let USER_PALETTES = {
    purple: ["#46244C", "#712B75", "#C74B50", "#D49B54"],
    rgb_example: [{ mode: "rgb", values: [255, 0, 0] }]
    hsb_example: [{ mode: "hsb", values: [255, 100, 0] }]
}

function setup() {
  initPalette(USER_PALETTES, USER_PALETTES.purple);

}

function draw() {
  	P.setPalette(C.palette)


    for (var i = 0; i < 10; i++) {
      fill(P.getI(i))
      rect(0, i * 20, 10, 10)
	}
}
```
