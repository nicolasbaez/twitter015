## twitter015 | #つぶやきProcessing 
https://twitter.com/nicolasbaez/status/1389413681935654915?s=20

![twitter](https://github.com/nicolasbaez/twitter015/blob/main/twitter015.gif)
```processing
void setup() {
  size(500, 500);
}
float a, b, i, j, k, r=9, w=500;
void _(float x, float y) {
  stroke(255);
  line(x, 0, x, y);
  for (i=0; i<8; i++) {
    a=x+r*cos(i);
    b=y+r*sin(i);
    line(x, y, a, b);
    line(a, b, a+random(2), b+9);
  }
}
void draw() {
  clear();
  for (j=0; j<w; j+=54) {
    _(j, k+noise(j+k)*6);
  }
  k+=0.5;
}
```
