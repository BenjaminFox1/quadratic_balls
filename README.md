# Quadratic Balls

I wanted to begin documenting some basic ideas and concepts related to my Computer Science Degree and thought I'd begin with some quadratics.

A number of [random balls](https://benjaminfox1.github.io/quadratic_balls/) falling using a very basic quadratic equation.

<details><summary>Code Below</summary>
<p>
  
 ``` javascript

var circle;

function setup() {
  createCanvas(600, 600);
  
  circle = {
		x_pos: 50,
		y_pos: 10,
		size: random (50,100)
	};
}

function draw() {
  background(150);
  fill(255,100,100,150);

  ellipse(circle.x_pos,
    circle.y_pos,
    circle.size,
    circle.size)
  
  circle.x_pos=circle.x_pos+0.8;
  circle.y_pos = pow((0.07*circle.x_pos),2)

  fill(255,255,100,150);
  ellipse(circle.x_pos+50,
    circle.y_pos+20,
    circle.size+10,
    circle.size+10)

  circle.x_pos=circle.x_pos+0.4;
  circle.y_pos = pow((0.05*circle.x_pos),2)

  fill(255,100,255,150);
  ellipse(circle.x_pos+50,
    circle.y_pos+75,
    circle.size+20,
    circle.size+20)

  circle.x_pos=circle.x_pos+0.6;
  circle.y_pos = pow((0.08*circle.x_pos),2)

  fill(255,150,255,150);
  ellipse(circle.x_pos+150,
    circle.y_pos+75,
    circle.size+20,
    circle.size+20)

  circle.x_pos=circle.x_pos+0.6;
  circle.y_pos = pow((0.08*circle.x_pos),2)

  
  fill(200,200,100,150);
  ellipse(circle.x_pos+50,
    circle.y_pos+120,
    circle.size+50,
    circle.size+50)

  circle.x_pos=circle.x_pos+1;
  circle.y_pos = pow((0.1*circle.x_pos),2)
}
```

</p>
</details>
