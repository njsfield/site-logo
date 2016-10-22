## Synopsis


A custom header component, comprised of a title, an svg logo, and CSS positioning to lock the logo and title into place.


## Work in Illustrator

After mind-mapping and sketching for half an hour, I was tempted to just give up then and there. Design is not my forte, though I hadn't touched Illustrator in several months and thought it would be a good exercise to relearn some key commands and tear up some anchor points.
<br>
Open sans was chosen as a standard clean sans-serif font, and I began by locking my name in place on the right side of the artboard, then secured many grid lines diagonal to the leg of the 'N'. I mirrored many of these vertically, to create a sort of diamond grid system. 
<br>
I then spent about 4 hours creating a flurry of abstract and completely pointless shapes that danced around the diamond grid lines (and nicely organized the shapes into layers, 'rain' 'clouds' 'dots' 'dashdots' 'legs' 'half-legs' etc), and finally spent a good half hour deleting about 70% of the shapes and keeping the neatest ones in.
<br>
At this point I decided it was time to give it a rest with illustrator and get to work putting it together in brackets.

## Work in Brackets

One day, I'll switch over to Atom. Until then, I'll swear by it for it's visual feedback when adjusting css rules. I created a header element with h1 tag, img and p tag (subheader), and used BEM style class-naming to build the module rules.
<br>
A tonne of contemplating went into deciding where the messiest positioning hacks would fall. Initially I tried keep the header container and h1/p tags clean and block stacked, and used psuedo elements to try and position the logo in a dirty way, this turned out to be just fine... but for some reason I really liked the cleanliness of just positioning the img nicely all the way to the left of the container, and letting everything else suffer.
<br>
The dirty hacks were burdoned on the header width, the h1's top padding and left padding. But the img was clean and nothing was collapsing.
<br>
Finally, the header containers font-size was set in relation to the viewport, and all elements in the block used ems in relation to keep it linear on all screen sizes. A media query was added to stop the growth in its tracks after 1000px viewport width. FIN.
