More.less brings you more to less.
Inspired by Compass and Twitter bootstrap.
More.less is a collection of css3 and crossbrowser mixins and will ease your development a lot.
Give it a try I know you'll love it.

Example usage of animations

    @import "more/shape.less";                            // Used to create the shape of the ball
    @import "more/css3/animation.less";                  // Is required to use animations
    @import "more/animation/seekers/bounce.less";       // A bounce animation
    @import "more/css3/gradient.less";                 // Put some colors to the ball
    @import "more/css3/box-shadow.less";              // Crossbrowser box-shadow

    .ball {
        #animation > .init(1.5s);                  // Init the animation with it's speed
        #animation > .delay(1s);                  // Let's wait a while before the animation can start
        #animation > .iteration-count(infinite); // Please never stop bouncing awesome ball
        #animation > .bounce;                   // This is the actual animation

        #shape > .circle(80px);               // Create a circle/ball
        #gradient > .horizontal;             // Let's put some color on the ball
        .box-shadow(-2px 3px 54px #8fa5ff); // Not everything fits in a namespace
    }
