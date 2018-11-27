# csportfolio

<details><summary>MyWebPage</summary>
      <p>This is a <a href="https://schlegelo.github.io/testPage/dogPage2/">Website<a/> I created, using html, about my dog. </p>
 </details>
<br>
    
 <details><summary>Lightning</summary>
      <p>I used the random and line methods along with a loop to create <a href="https://schlegelo.github.io/lightning2/">Lightning<a/>.        </p>
  </details>
 <br>
       
 <details><summary>Dice</summary>
      <p>I created <a href="https://schlegelo.github.io/dice3/">Dice<a/> objects that stored a random value from 1 to 6 and used a              nested for loop to make a grid of them.</p>
  </details>
 <br>

<details><summary>Chemotaxis</summary>
      <p>I created Bacteria objects that follow the mouse mimicing the <a href="https://schlegelo.github.io/chemotaxis4/">Chemotaxis<a/>        of actual cells. </p>
 </details>
<br>

<details><summary>StarField</summary>
      <p>I created a particle interface that thet my other classes inherited. The objects of these classes moved in patterns creating a        <a href="https://schlegelo.github.io/starfield5/">StarField<a/>. </p>
 </details>
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
