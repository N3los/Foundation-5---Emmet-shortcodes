# Foundation 5 - Emmet shortcodes
List of Emmet shortcodes for Foundation 5

Codes are mostly taken from F5 docs page and just "translated" to Emmet. With this u can make a fast prototype of your design in matter of minutes.


## Topbar navigation

.contain-to-grid.sticky>nav.top-bar[data-topbar data-options="sticky_on: large"]>ul.title-area>li.name>h1>a{Site name}^^li.toggle-topbar.menu-icon>a>span{Menu}^^^+section.top-bar-section>ul.right>li.active>a{Active Button}^li*5>a{Button}^li.has-dropdown>a{Dropdown Button}+ul.dropdown>li*5>a{Dropdown button $}.

## Orbit slider

ul.example-orbit[data-orbit]>li*3>img[src=http://lorempixel.com/1000/300/ alt=slider image $]+.orbit-caption{Slider caption $}

## Images

LoremPixel categories: abstract / animals / business / cats / city / food / nightlife / fashion / people / nature / sports / technics / transport

img[src=http://lorempixel.com/300/300/nature/$ alt=Image]*10

## F5 Gallery

ul.clearing-thumbs.small-block-grid-4img[data-clearing]>li*10>a.th[href="http://lorempixel.com/800/300/nature/"]>img[src="http://lorempixel.com/100/100/nature/" alt="Image"]

## Form

form>.row>.large-12.columns>label{Label:}>input:text^^^+.row>.large-4.columns*3>label{Label:}>input:text^^^.row>.large-12.columns>label{Label:}>select>option[value="$"]*5>{value $}^^^^^.row>(.large-6.columns>(label[for="radio$"]{Radio label $}+input:radio#radio$)*4)+(.large-6.columns>(label[for="check$"]{Checkbox label $}+input:checkbox#check$)*4)^.row>.large-12.columns>label{Textarea}>textarea