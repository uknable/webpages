FRONT-END JOURNEY TO THE STARS

github repo detailing my experience in learning front-end stuff.

Thursday 9th Feb

I'm one step closer to clearing the fog of this mystical language of making webpages. I learned about specificity and how its weight determines what style certain elements take on. My frustrations on replicating the youtube page is now behind me. I can't wait for the next feeling of confusion/anger/urgetothrowmymouseagainstthescreen!

	ID    > Class > Type
	1-0-0   0-1-0   0-0-1

When combining selectors they should be read from right to left. The selector farthest to the right is known as the 'key selector'.

	.hotdog p {
	  propertyzzz: valuezzz;
	}

The two selectors are seperated by a single space. The key selector is a type selector targetting paragraph elements and because this type selector is prequalified with a class selector of hotdog, the full combined selector will only select paragraph elements that reside within an element with a class attribute value of hotdog.
	Combining selectors will also cobine their specificity weights making our example have a total of 0-1-1.

====ANOTHER BIT OF INFO THAT WILL CURE CONFUSION====

BLOCK-LEVEL ELEMENTS occupy any available width, regardless of their content, and begin a new line.
INLINE-LEVEL ELEMENTS occupy only the width their content requires and line up on the same line, one after the other.

With the 'inline-block' value, an element will behave as a block-level element, accepting all box model properties. However, the element will be displayed in line with other elements, and it will not begin on a new line by default. 

EVERY ELEMENT on a PAGE is a RECTANGULAR BOX


WIDTH - Block level elements have a default width of 100%, consuming the entire horizontal space available. Inline and inline-block elements expand and contract horizontally to accommodate their content.
	Inline-level elements cannot have a fixed size, thus the width and height properties are only relevant to non-inline elements.
	Block and inline-block elements will accept the width and height properties and their corresponding values.

MARGIN - Vertical margins (top and bottom), are not accepted by inline-level elements. These vertical margins are, however, accepted by block-level and inline-block elements.

PADDING - works on all sides of an inline element.

The margin and padding properties are completely transparent and do not accept any colour values.

BOX-SIZING - The box model may be changed to support different calculations. CSS3 intoduced the 'box-sizing' property which allows us to change exactly how the box model works and how an elements size is calculated.
	This property accepts three values:
	1. content-box
	2. padding-box
	3. border-box 

1. content-box is the default value. Total width = width + padding + margin
2. Padding is included in the width. Total width = width + margin
3. Margin and padding is included. Total width = width
