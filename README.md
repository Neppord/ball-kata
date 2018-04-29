# Ball Kata

Create a 2D bouncing ball in the browser using javascript.

```
 ________________________________
|       /\                       |
|      o  o                      |
|     /                          |
|    o                           |
|                                |
|                                |
|                                |
|                                |
|                                |
|                                |
|                                |
|________________________________|
```

Start feedbackloop:
```
$ npm install
$ npm start
```

and then open `http://localhost:8080/index.html` in a web-browser. It will reload the page when you save the file.

Some example constraints:

 * The ball should:
    * start at a random position (but not inside a wall)
    * have a random speed:
        * not faster then its 2 times its radius per second
        * and not less then its radius per second
        * in a random direction.
    * have a radius of 25 px (or points)
    * have the color blue
    * bounce on all walls 4:
        * loosing *no* momentum
        * deflect perfectly
        * at the edge of the ball (not the center)
 * The wall should:
    * have the color black
    * cover a area that is 640 x 480 px (or points)
 * The frame rate should:
    * be as high possible.
    * not dependent on ball speed.
    * use `requestAnimationFrame` if applicable.

Methods to try out:
 * Test Driven Design: BDD, Mockist-approach, or Classic
 * State:
    * global
    * OO-Global
        Grouped but still global via `Singelton` or other
    * OO-Encapsulated
        Using scopes and module pattern to hide state, or this and hide the object itself.
    * Immutable:
        never mutate the state only generate new state passing it through function calls.
         By hand or one of the state patterns: Applicative, Monadic
 * Physics:
    * Time discrete
    * Event based
 * Render:
    * 2D canvas element
    * SVG
    * Divs (hint: border-radius 50% )
    * Web-gl, flat or 3d, but still 2d physics.