Logic:

Display one image at a time.
Provide a way to navigate between images.
Highlight the current slide.
Step 2: Create the Basic Structure in HTML

WSA icon
Project title/name
Container for the image
Navigation buttons
Dot indicators for jumping to specific slides
Footer

>CSS

>step 3: JS 
Current slide index = 0
>create show and hide image - Logic
we need function for hidding all the images otherthan current image.

Function name showImag();
Step1: Retrieve all slides using document.getElementbyClassname("carouel-slide")

step 2: Loop through these slides and set display :none to hide them

step 3: Display the current slide using display: block

step 4: Retrieve all dots and remove active class from them

step 5: Add the dot-active class to the dot corresponding to the current slide

step 6: Handling  the Navigation
Logic: To move forward/Backward in the slide sequence
  -function changeSlide(n);
  Modify thslide
 CurrentSlideIndec by adding n.
  where , n is +1 for next 
>jump to specific slide when dot is clicked
function : CurrentSlide(n)
set CurrentSlideIndec to the clicked dots index

>Intial setup
call showslide(CurrentSlideIndec)