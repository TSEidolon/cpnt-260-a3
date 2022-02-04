# CPNT-260 Assignment 3
### by: Edgar Caballero

<strong> Github Repo:</strong>
 - 

<strong>Github Pages: </strong>
  - 

<br>

## Reflection: (<em> CSS Style sheet in `css/style.css`</em>)
1. I was not able to make the Grid layout for the Gallery responsive. It only shrunk. I could not get help during lab time due to time constraints, so I tried to troubleshoot the issue by myself. Found several solutions but nothing changed. 
    - It would not condense into a single column once the screen size got smaller:
      - Tried `autofit` with `grid-auto-columns` and `grid-auto-rows`. 
        ```
        grid-auto-columns: repeat(auto-fit(8, 1fr));
        grid-auto-rows: repeat(auto-fit(8, 1fr));
        ```
        - It should've generated more rows as the screen got smaller due to the grid-auto command. It did not. Just using `grid-auto-rows: auto;` did not work either.
      - Media queries did not seem to work either.
    - Tried making the grid items into flex containers did not work either.
    ```
    display:flex;
    flex-direction: column;
    ```
      - Flex wrap breaks everything (did not use)
2. Had trouble with hover transitions to make the figcaption disappear when hovered.
    - It was due to the wrong “selector specificity”.
      - <strong>Problem</strong> was that I was using `figure img:hover figcaption {}`.
      - <strong>Fixed</strong> when I used `figure:hover figcaption {}`.

<br>

## Flare:
 - Shows figcaptions on images when hovered on.
 - `lines 90-107`

## Attributions
 - Hogwarts Letter by <a href="https://unsplash.com/photos/tS-jh0M6JoA" target="_blank">&copy;Tuyen Vo</a> 
 - Educational Decrees by <a href="https://unsplash.com/photos/cl8dqBQgRGY" target="_blank">&copy;Rhii Photography</a>
 - Dining Hall Tables by <a href="https://unsplash.com/photos/cAFAVm3VKZA" target="_blank">&copy;Rhii Photography</a>
 - Dumbledore's Office by <a href="https://unsplash.com/photos/lvqSlFAXsFA" target="_blank">&copy;Gabriel Kraus</a>
 - Great Hall by <a href="https://unsplash.com/photos/9ChvC9mBpCY" target="_blank">&copy;Mathew Schartz</a>
 - Potions Class by <a href="https://unsplash.com/photos/3X5ZhsDClY8" target="_blank">&copy;Gabriel Kraus</a>
 - White Owl by <a href="https://unsplash.com/photos/c1fFv08N7qE" target="_blank">&copy;Frida Lanenstrom</a>
 - Hogwarts Castle Sky by <a href="https://unsplash.com/photos/Ipv_MNTzcQI" target="_blank">&copy;Josipa Juras</a>
 - Hogwarts Lake by <a href="https://unsplash.com/photos/FdJmE0YibvQ" target="_blank">&copy;Gio Almonte</a>
 - The Golden Snitch by <a href="https://filmz.ru/photos/films/1199/#gallery-70" target="_blank">&copy;Filmz</a>