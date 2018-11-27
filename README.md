# csportfolio

<details><summary>MyWebPage</summary>
      <p>This is a <a href="https://schlegelo.github.io/testPage/dogPage2/">website<a/> I created, using html, about my dog
      </p>
    </details>

<ul>
  <li> Lightning! <a href="https://schlegelo.github.io/lightning2/">Here<a/>
    <p> <p/>
  <li> Dice <a href="https://schlegelo.github.io/dice3/">Here<a/>
  <li> ChemoT <a href="https://schlegelo.github.io/chemotaxis4/">Here<a/>
  <li> Starfield <a href="https://schlegelo.github.io/starfield5/">Here<a/>
<ul/>
<br>
    

### Toughest code so far!
```Java
 void move() {
    x += (int)random(3)-1;
    y += (int)random(3)-1;
    
    float yDiff = mouseY - y;
    float xDiff = mouseX - x;       
    float theta = atan(yDiff / xDiff);
    //if(!collision){
    if(dist(x,y,mouseX,mouseY) < 300) {
      if(mouseX < x) {
        x -= (velocity * cos(theta));
        y -= (velocity * sin(theta));
      } else {
        x += velocity * cos(theta);
        y += velocity * sin(theta);    
      }
    }
    //}
  }
  ```
