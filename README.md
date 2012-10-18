More.less brings you more to less.
Inspired by Compass and Twitter bootstrap.
More.less is a collection of css3 and cross-browser mixins and will ease your development a lot.
Give it a try I know you'll love it.


The goal is not to bloat your css but to ease your development.
No classes will be added to your css when you use More.less.

More.less will not supply you with any components, but will supply you with
 some solutions for lists, links, texts and more.

Animations
More.less includes all animate.css animations http://daneden.me/animate/
You should only import the animations that you are going to use,
because the keyframes will bloat your css.

The structure of the animations looks like this.
more/animation/bounce/(in|out)/bounce.less


Example usage of animations

    @import "more.less";                                 // Import more.less don't worry nothing will be added to your css
    @import "more/animation/bounce.less";               // A bounce animation


    .animated-ball {
        #animation > .init(1.5s);                    // Init the animation with it's speed
        #animation > .delay(1s);                    // Let's wait a while before the animation can start
        #animation > .infinite;                    // Please never stop, awesome animation
                                                  // A switch is used to separate
                                                 // In and out animations
        #animation > .bounce(in);               // This is the actual animation

        #shape > .circle(80px);               // Create a circle/ball
        #gradient > .horizontal;             // Let's put some color on the ball
        .box-shadow(-2px 3px 54px #8fa5ff); // Not everything fits in a namespace but it is cross-browser
    }
