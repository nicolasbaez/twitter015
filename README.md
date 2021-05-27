# twitter015
#つぶやきProcessing void setup(){size(500,500);}float a,b,i,j,k,r=9,w=500;void _(float x,float y){stroke(255);line(x,0,x,y);for(i=0;i&lt;8;i++){a=x+r*cos(i);b=y+r*sin(i);line(x,y,a,b);line(a,b,a+random(2),b+9);}}void draw(){clear();for(j=0;j&lt;w;j+=54){_(j,k+noise(j+k)*6);}k+=0.5;}
