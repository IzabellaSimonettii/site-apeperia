# site-apeperia

Before componentizing 
Command in the mac to watch the changes 
   sass --waitch style.scss:style.css

   ---

Sass command 
   sass style.scss:style.css

Making a color darker!

$variable: darken (color, porcentage); - darken(#BADA55, 10)


Making a color lighter!

$variable: lightnen (color, porcentage); - lighten(#BADA55, 10)

or 

$variable: lightness (color); - lightness(#BADA55)



Use mixin when you have a patten value or just a value to imput in the call, otherwise you can use a placeholder. When you use lots of mixin in the CSS, the code is repeted in all of them so you have to mesure the impact of that in the code.

@mixin size($width, $height: $width) {
    width: $width;
    height: $height;
}

 to use ->  @include size(23, 9);


The placeholder make a group of places that need that settings and avoid the repetitions of the code, but is just a alternative of the mixin when we deal with fixed parameters "when you need to put a value in the call".
%placeholder {
    display: block;
    margin-left: auto;
    margin-right: auto;
}

@extend %placeholder;

