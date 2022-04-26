# sass

https://hub-mo.github.io/sass/


learned:

scss variables:

    ex :
    => $variableName: green;

    header {
        background: $variableName
    }


mixins:

    ex of creating a mixin: 
    @mixin Name {
        display: flex;
        justify-content: center;
    }

    ex of using a mixin:
    header {
        @include name();
    }

nesting:

    

    header {
    background: blue;
        display: flex;
        justify-content: center;
        button {
            background:green;
        }
    }

    instead of using : header button {...} you can nest the button inside the header styling.
    
    

extensions:

    .contact {
        @extend header;
    }

    this puts the same styling as header inside the contact class styling.

compiling sass with a VSCode extansion and via Terminal 
= sass --watch style/style.scss style/style.css( start watching) - stop (ctrl + C)


extra:
minifying style sheet:

    sass --watch --style=compressed style/style.scss style/style.min.css

checking the size of the style sheet via terminal = "ls -l"

