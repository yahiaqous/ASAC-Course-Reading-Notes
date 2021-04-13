# CSS Transforms, Transitions, and Animations




## CSS Transforms
The transform property comes in two different settings, **two-dimensional** and **three-dimensional**. Each of these come with their own individual properties and values

### 2D Transforms


|      **Property**      |                                              **Details**                                              |               **Example**               |
|------------------------|-------------------------------------------------------------------------------------------------------|-----------------------------------------|
| **2D Rotate**          | Rotate an element from 0 to 360 degrees                                                               | transform: rotate(20deg);               |
| **2D Scale**           | Change the appeared size of an element                                                                | transform: scale(.75); scale(.5, 1.15); |
| **2D Translate**       | Push and pull an element in different directions without interrupting the normal flow of the document | transform: translate(-10px, 25%);       |
| **2D Skew**            | Distort elements on the horizontal axis, vertical axis, or both                                       | transform: skew(5deg, -20deg);          |
| **Transform Origin**   | Change the default origin position from element center                                                | transform-origin: top left; 100% 100%;  |
| **Perspective**        | The vanishing point, that can be seen in three-dimensional drawings                                   | transform: perspective(200px);          |
| **Perspective Origin** | Change the default origin vanishing point position                                                    | perspective-origin: 0 0; 75% 75%;       |



### 3D Transforms


|   **Property**   |                    **Details**                     |        **Example**         |
|------------------|----------------------------------------------------|----------------------------|
| **3D Rotate**    | rotate an element around any axes x, y, z          | transform: rotateZ(45deg); |
| **3D Scale**     | Change the appeared size of an element on any axes | transform: scaleZ(1.75);   |
| **3D Translate** | Push and pull an element into any axes             | translateZ(-50px);         |




## CSS Transitions
alter the appearance and behavior of an element whenever a state change occurs, such as when it is *hovered over*, *focused on*, *active*, or *targeted*


|          **Property**          |                                               **Details**                                                |                   **Example**                   |
|--------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| **transition-property**        | Determines exactly what properties will be altered in conjunction with the other transitional properties | transition-property: background, border-radius; |
| **transition-duration**        | The duration in which a transition takes place                                                           | transition-duration: .2s,                       |
| **transition-timing-function** | Set the speed in which a transition will move                                                            | transition-timing-function: linear; ease-in;    |
| **transition-delay**           | Sets a time that determines how long a transition should be stalled before executing                     | transition-delay: 1s;                           |




### Simple CSS Transitions that will WoW Users


|    **Transition**    |                                                                   **Code**                                                                      |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| **Fade in**          | .fade{opacity:0.5;}  .fade:hover{opacity:1;}                                                                                                    |
| **Change color**     | .color:hover{background:#53a7ea;}                                                                                                               |
| **Rotate elements**  | .rotate:hover{webkit-transform: rotateZ(-30deg); -ms-transform: rotateZ(-30deg); transform: rotateZ(-30deg);}                                   |
| **Square to circle** | .circle:hover{border-radius:50%;}                                                                                                               |
| **3D shadow**        | .threed:hover{box-shadow: 1px 1px #53a7ea, 2px 2px #53a7ea, 3px 3px #53a7ea; -webkit-transform: translateX(-3px); transform: translateX(-3px);} |
| **Inset border**     | .border:hover{box-shadow: inset 0 0 0 25px #53a7ea;}                                                                                            |



* **Grow & Shrink**  
.grow:hover{-webkit-transform: scale(1.3); -ms-transform: scale(1.3); transform: scale(1.3);}  
.shrink:hover{-webkit-transform: scale(0.8); -ms-transform: scale(0.8); transform: scale(0.8);}

  
* **Swing**                
@-webkit-keyframes swing{15%{-webkit-transform: translateX(5px); transform: translateX(5px);}
    30%{-webkit-transform: translateX(-5px); transform: translateX(-5px);} 
    50%{-webkit-transform: translateX(3px); transform: translateX(3px);}
    65%{-webkit-transform: translateX(-3px); transform: translateX(-3px);}
    80%{-webkit-transform: translateX(2px); transform: translateX(2px);}
    100%{-webkit-transform: translateX(0); transform: translateX(0);}}               
@keyframes swing{15%{-webkit-transform: translateX(5px); transform: translateX(5px);}
    30%{-webkit-transform: translateX(-5px); transform: translateX(-5px);}
    50%{-webkit-transform: translateX(3px); transform: translateX(3px);}
    65%{-webkit-transform: translateX(-3px); transform: translateX(-3px);}
    80%{-webkit-transform: translateX(2px); transform: translateX(2px);}
    100%{-webkit-transform: translateX(0); transform: translateX(0);}}                      
.swing:hover{-webkit-animation: swing 1s ease; animation: swing 1s ease; -webkit-animation-iteration-count: 1; animation-iteration-count: 1;}






## CSS Animations
allow the appearance and behavior of an element to be altered in multiple keyframes


|                 **Property**                    |                                              **Details**                                              |                           **Example**                          |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| **Animations Keyframes**                        | Set multiple points at which an element should undergo a transition                                   | @keyframes test {0%{left: 0;} 100%{left: 488px;}}              |
| **animation-name**                              | After declaring keyframes for animation from the @keyframes rule                                      | animation-name: test;                                          |
| **Animation Duration, Timing Function & Delay** | After declaring the animation-name property on an element, animations behave similarly to transitions | animation-duration: 2s; animation timing-function: ease-in-out;|
| **animation-iteration-count**                   | Have an animation repeat itself numerous times                                                        | animation-iteration-count: infinite;                           |
| **animation-direction**                         | Declare the direction an animation completes                                                          | animation-direction: alternate;                                |
| **animation-play-state**                        | Allows an animation to be played or paused                                                            | animation-play-state: paused;                                  |
| **animation-fill-mode**                         | Identifies how an element should be styled either before, after, or before and after animation is run | animation-fill-mode: forwards;                                 |


