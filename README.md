# Foundation 5 - Emmet shortcodes
List of Emmet shortcodes for Foundation 5

Codes are mostly taken from F5 docs page and just "translated" to Emmet. With this u can make a fast prototype of your design in matter of minutes.

Lorem pixel is used for images, u can write down and number for desired dimensions of images


## Topbar navigation

http://foundation.zurb.com/docs/components/topbar.html

`.contain-to-grid.sticky>nav.top-bar[data-topbar data-options="sticky_on: large"]>ul.title-area>li.name>h1>a{Site name}^^li.toggle-topbar.menu-icon>a>span{Menu}^^^+section.top-bar-section>ul.right>li.active>a{Active Button}^li*5>a{Button}^li.has-dropdown>a{Dropdown Button}+ul.dropdown>li*5>a{Dropdown button $}`

## Orbit slider

http://foundation.zurb.com/docs/components/orbit.html

`ul.example-orbit[data-orbit]>li*3>img[src=http://lorempixel.com/1000/300/ alt=slider image $]+.orbit-caption{Slider caption $}`

## Images

LoremPixel categories: abstract / animals / business / cats / city / food / nightlife / fashion / people / nature / sports / technics / transport

`img[src=http://lorempixel.com/300/300/nature/$ alt=Image]*10`

## F5 Clearing (Lightbox)

http://foundation.zurb.com/docs/components/clearing.html

`ul.clearing-thumbs.small-block-grid-4img[data-clearing]>li*10>a.th[href="http://lorempixel.com/800/300/nature/"]>img[src="http://lorempixel.com/100/100/nature/" alt="Image"]`

## Form

http://foundation.zurb.com/docs/components/forms.html

`form>.row>.large-12.columns>label{Label:}>input:text^^^+.row>.large-4.columns*3>label{Label:}>input:text^^^.row>.large-12.columns>label{Label:}>select>option[value="$"]*5>{value $}^^^^^.row>(.large-6.columns>(label[for="radio$"]{Radio label $}+input:radio#radio$)*4)+(.large-6.columns>(label[for="check$"]{Checkbox label $}+input:checkbox#check$)*4)^.row>.large-12.columns>label{Textarea}>textarea`

## Accordion

http://foundation.zurb.com/docs/components/accordion.html

`ul.accordion[data-accordion]>li.accordion-navigation*5>a[href="#panel$a"]{Accordion $}+#panel$a.content>lorem20`

## Tabs

http://foundation.zurb.com/docs/components/tabs.html

`(ul.tabs[data-tab]>li.tab-title.active>a[href="#panel$"]{Tab $}^li.tab-title*4>a[href="#panel$"]{Tab $})+(.tabs-content>.content.active#panel$>p>lorem15^^.content#panel$*4>p>lorem15)`

If u want vertical tabs, just all "vertical" to first ul.tabs like this:  "ul.tabs.vertical"

## Block grid

http://foundation.zurb.com/docs/components/block_grid.html

`ul.small-block-grid-2.medium-block-grid-4.large-block-grid-6>li*6>{Your content}`

## Interchange

http://foundation.zurb.com/docs/components/interchange.html

### Images

img tag will generate src="" which u don't need so u can remove it

`img[data-interchange="[/path/to/default.jpg, (default)], [/path/to/bigger-image.jpg, (large)]"]`
`img[data-interchange="[/path/to/default.jpg, (only screen and (min-width: 1px))], [/path/to/bigger-image.jpg, (only screen and (min-width: 1280px))]"]`

### Content

'SOON' - Need to check all the options and write a good description


## Icon bar

http://foundation.zurb.com/docs/components/icon-bar.html

Icons are "Font Awesome" (http://fortawesome.github.io/Font-Awesome/) so the <i> class names are not from Foundation
Just change "home" part with something else (ex. envelope, phone, trash, close... check FontAwesome cheatsheet)

`.icon-bar.five-up>a[href="#"].item*4>i.fa.fa-home+label>{Label txt $}`


## Magellan 

**Sticky nav with scroll to section, can use for OnePage webs**

http://foundation.zurb.com/docs/components/magellan.html

The multiply number (*4 in this case) must be the same in both parts of the code

`(div[data-magellan-expedition="fixed"]>dl.sub-nav>dd[data-magellan-arrival="section-$"]*4>a[href="section-$"]>{Section $})+(.magellan-destinations>(h3[data-magellan-destination="section-$"]+a[name="section-$"]+section.magellan-content)*4)`


## Breadcrumbs

http://foundation.zurb.com/docs/components/breadcrumbs.html

`ul.breadcrumbs>li>a[href="#"]>{Home}^^+li.current>a[href="#"]>{Current}`


## Reveal Modal

http://foundation.zurb.com/docs/components/reveal.html

`(a[href="#" data-reveal-id="myModal"]>{Click Me For A Modal})+(#myModal.reveal-modal[data-reveal aria-labelledby="modalTitle" aria-hidden="true" role="dialog"]>(h2.modal-title>{Awesome modal})+(p.lead>{Some text})+(a.close-reveal-modal[aria-label="Close"]>{&#215;}))`


## Table

http://foundation.zurb.com/docs/components/tables.html

`table>(thead>tr>th*4>{Table header $})+(tbody*1>tr*4>td*4>{Table cell $})`
