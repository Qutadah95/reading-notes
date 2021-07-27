## Transforms 

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

## Transform Syntax

div {


  -webkit-transform: scale(1.5);


     -moz-transform: scale(1.5);


       -o-transform: scale(1.5);


          transform: scale(1.5);

}

## 2D Transforms

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

* 2D Rotate

![](img/118.PNG)

* 2D Scale
![](img/119.PNG)

* 2D Translate

![](img/120.PNG)

* 2D Skew

![](img/121.PNG)

## Combining Transforms
![](img/122.PNG)

* 2D Cube Demo

![](img/123.PNG)

## Transitions & Animations
One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

## Transitions

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

* Transition Demo

![](img/124.PNG)

## Transitional Property
The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

### Transitional Properties

It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.
* background-color
* background-position
* border-color
* border-width
* border-spacing
* bottom
* clip
* color
* crop
* font-size
* font-weight
* height
* left
* letter-spacing
* line-height
* margin
* max-height
* max-width
* min-height
* min-width
* opacity
* outline-color
* outline-offset
* outline-width
* padding
* right
* text-indent
* text-shadow
* top
* vertical-align
* visibility
* width
* word-spacing
* z-index


## Transitional Button

![](img/125.PNG)

## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS

1. Fade in 
Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:

.fade


{


        opacity:0.5;


}


.fade:hover


{


        opacity:1;


}



2. Change color



.color:hover


{


        background:#53a7ea;



}


3. Grow & Shrink

.grow:hover


{


        -webkit-transform: scale(1.3);


        -ms-transform: scale(1.3);


        transform: scale(1.3);


}


.shrink:hover


{


        -webkit-transform: scale(0.8);


        -ms-transform: scale(0.8);


        transform: scale(0.8);


}
4. Rotate elements


.rotate:hover


{


        -webkit-transform: rotateZ(-30deg);


        -ms-transform: rotateZ(-30deg);


        transform: rotateZ(-30deg);


}


5. Square to circle


.circle:hover


{


        border-radius:50%;


}


6. 3D shadow


.threed:hover


{
        box-shadow:


                1px 1px #53a7ea,


                2px 2px #53a7ea,


                3px 3px #53a7ea;


        -webkit-transform: translateX(-3px);


        transform: translateX(-3px);


}
7. Swing


@-webkit-keyframes swing


{


    15%


    {


        -webkit-transform: translateX(5px);


        transform: translateX(5px);


    }


    30%


    {


        -webkit-transform: translateX(-5px);


       transform: translateX(-5px);


    } 


    50%


    {


        -webkit-transform: translateX(3px);


        transform: translateX(3px);


    }


    65%


    {


        -webkit-transform: translateX(-3px);


        transform: translateX(-3px);


    }


    80%


    {


        -webkit-transform: translateX(2px);


        transform: translateX(2px);


    }


    100%


    {


        -webkit-transform: translateX(0);


        transform: translateX(0);


    }


}




@keyframes swing


{


    15%


    {


        -webkit-transform: translateX(5px);


        transform: translateX(5px);


    }


    30%


    {


        -webkit-transform: translateX(-5px);


        transform: translateX(-5px);


    }


    50%


    {


        -webkit-transform: translateX(3px);


        transform: translateX(3px);


    }


    65%


    {


        -webkit-transform: translateX(-3px);


        transform: translateX(-3px);


    }


    80%


    {


        -webkit-transform: translateX(2px);


        transform: translateX(2px);


    }


    100%


    {


        -webkit-transform: translateX(0);


        transform: translateX(0);


    }


}



.swing:hover


{


        -webkit-animation: swing 1s ease;


        animation: swing 1s ease;


        -webkit-animation-iteration-count: 1;


        animation-iteration-count: 1;


}

8. Inset border

.border:hover


{

        box-shadow: inset 0 0 0 25px #53a7ea;


}











