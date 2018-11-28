# csportfolio


## Projects

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
      <p>I created a particle interface that my other classes inherited. The objects of these classes moved in patterns creating a        <a href="https://schlegelo.github.io/starfield5/">StarField<a/>. </p>
 </details>
<br>

### Project Reflection
      
      looking at my projects I am pleased with what I have done, but I think I could do better. Due to time constraints I was unable to do more with my projects than I accomplished. An example of this is my Chemotaxis; I was hoping to add collision and have the bacteria grow and multiply as they consumed particles. While I was unable to do this I still hope to add it sometime down the road. I would also like to make another website in the future. My mom used to make and sell and she is starting again, so I may make a website for her. My favorite project is definetly StarField as I was able to complete it and I am really pleased with how it turned out as I think it looks very appealing. Generally I would have to say these projects were pretty easy, though they certainly would have been harder had I added more things to them such as collision.

## Toughest code so far!
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
   I wouldn't say any of my code was particularily tough, but I dedcided to pick this snippet as I actually had to use math to solve my problem. My issue was I wanted my bacteria to move directly to the mouse and maintain a constant velocity. Since the mouse and bacteria form a right triangle due to the x and y, I used the difference in the x and y to find the angle, relative to the horizontal of the bacteria, the mouse was at. Then I used the angle and and the Hypothenuse (which was set as my desired speed) to find the necessary movement in the x and y to achieve the desired magnitude and direction 
