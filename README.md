# html_slider_2

An html slider that takes in external or internal html "slides" and displays them as iframes. CSS animation controlled via javascript applies a smooth transition from one slide to the next in either direction. 

---
## Algorithm - abstract
The slider uses html slides input as iframes. Currently, 2 basic (and frankly ugly) slides are hardcoded into the slider html, though they can be referenced by directory if the user desires via var "htmlfiles" in script location (true or false). Since this is only hardcoded to be useable with 2 slides at the moment, container in total contains 3 slides in order from left to right: Slide 2 (invisible, to left), Slide 1 (visible), Slide 2 (invisible, to right). The fact that Slide 2 is preloaded in either direction makes animation a lot smoother than if it was instantiated during or just before animation (trust me). Animation css class is added to a pseudo-container inside the main container that visually shifts all elements in any direction. After animation, the original slide html is replaced on both sides of the current slide: Slide 1 (invisible, to left), Slide 2 (visible), Slide 3 (invisible, to right).
