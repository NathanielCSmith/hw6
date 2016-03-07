//creating a class to draw tha ball
//the whole top part is the class being built. line 39 on is calling the ballz


class Ball {
  int x;
  int y;
  int radius;
  int xspeed;
  int yspeed;

  Ball(int startx, int starty) {
    radius = 5;
    x = startx;
    y = starty;
    xspeed = 3;
    yspeed = 4;
  }

  void display() {
    ellipse(x, y, radius * 2, radius * 2);
    fill(0);
  }
  void move() {
    x = x + xspeed;
    y = y + yspeed;
  }

  void bounce() {
    if (x + radius >= width || x - radius <= 0) {
      xspeed = -xspeed;
    }
    if (y + radius >= height || y - radius <= 0) {
      yspeed = -yspeed;
    }
  }
}

Ball b = new Ball(15,25);
Ball c = new Ball(30,75);

  void setup() {
    size(500, 500);
  }

  void draw() {
    background(255);

    b.display();
    c.display();
    
    b.move();
    c.move();
    
    b.bounce();
    c.bounce();
  }
