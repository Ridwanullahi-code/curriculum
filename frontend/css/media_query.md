# CSS Medial Query
## Learning Objectives

### Estimated time: 3h
## Description
Media queries are useful when you want to modify the layout or appearance of your site depending on specific characteristics such as the screen resolution of the device or the browser viewport width or height.

A media query is composed of:

An optional media type defining a broad category of devices to which the media query applies: all, print, or screen. This type is optional; it is assumed to be all if omitted
Any number of media feature expressions describing a specific characteristic of the user agent, output device, or environment. Examples are: hover, prefers-reduced-motion, and width
The common syntax for a CSS media query is as follows:

@media media type and (media feature expression) {
/* CSS rules */
}
The logical operators not, and, only, and or can be used to compose a complex media query.

For responsive design, min-width and max-width are the most commonly used media features. They enable styles to be based on the width of the viewport. For example, the following CSS code will apply styles only if the browser’s viewport width is equal to or less than 80em:

#### Extral Small devices such as large phones (less than or equal to 480px) 
`@media only screen and (max-width: 480px) {...}`
#### Small devices such as large phones (640px and up) 
`@media only screen and (max-width: 767px) {...}`
#### Medium devices such as tablets (768px and up)
`@media only screen and (min-width: 768px) {...}`
OR
`@media only screen and (min-width: 768px) and (max-width: 1023px)  {...}`

#### Large devices such as laptops (1024px and up)
`@media only screen and (min-width: 64em) {...}`

#### Largest devices such as desktops (1280px and up) 
`@media only screen and (min-width: 80em) {...}`