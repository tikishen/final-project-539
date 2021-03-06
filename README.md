# final-project-539

## Basic Requirements
### Responsive Design
The responsive design trigger when screen width are 950px or less, 750px or less, and 750px or less plus landscape orientation. <br>
- **950px wide or less** : Change on padding and font size of navigation bar, flex size of container for About, Contact page. <br>
- **750px wide or less**: Change on padding and font size of navigation bar, flex layout of container for About, Contact page (Columns of picture and text stack on top of each other instead of next to each other). <br>
- **750px wide or less and landscape**: Change on padding and font size of navigation bar, flex size of container for About, Contact page, the size of light box container.<br>

### Grid and Flex Box
- **Footer:**<br>
Flex is used to create a container to justify the content and text align center.<br>

- **Home Page:**<br>
Flex is used as a container to put author name and position title. Flex used here for vertical and center layout (flex-direction: column;). <br>

- **About Page:**<br>
Flex is used to create a row container (.container-row {display: -webkit-flex;}), and two column containers that sits next to each other. The picture container also has a page-content to make its position center.<br>

- **Contact Page:**<br>
This page used the same row container and page container as About Page. The logic and layout of column containers that sits next to each other are as same as the About Page, except change on background-color. <br>

- **Foodie Blog**:<br>
Grid is used here to create two grid boxes that are sit next to each other, and has 20px row gap with other grid boxes. <br>

### JS and jQuery (excluding advanced js and jquery)
- **JS is used for Contact Page.**<br>
When clicking submit form, the js is triggered to check if the name and email text area has been filled. If not, it raises error message. If yes, the form could be submitted.<br>

 - **jQuery is used for Foodie Blog Page.**<br>
The heart-like icon was dark grey initially. When clicking the icon, it became to red, triggling style in ".like" class.<br>

### Each page must validate on w3 and aXe
Yes, except w3 errors on lightbox, but it was acceptable for the previous assignment.

### What I have changed after demo?
The navigation can clearly display the current page, implemeted by bootstrap nav-tabs and active classes.


## Extras
### Accessibility

#### Color:
1. Is color alone used to convey important information? <br>
View the page in gray-scale. All the information are still understandable and all page functions can perform. <br>
2. Is the color contrast of text readable by people with low-vision? <br>
aXe does not detect any issues related to color contrast. <br>

#### Images:
3. Do all images have alternative text? <br>
aXe does not detect any issues related to missing alt text. <br>
4. Does the alternative text make sense? <br>
Yes, they all make sense, and describe the certain area is used for image.<br>
5. If the image is a link, does the alternative text clearly identify the link destination? <br>
There is no image that is a link.<br>
6. Are all CSS background images either pure decoration or have alternative text? <br>
When hiding the background image, users still have access to all information and functionality. And it has passed aXe background image check.<br>
7. Is any text embedded in images? <br>
There is no text embedded in images.<br>

#### Keyboard
8. Does the tab order make sense? <br>
When tabbing through the page using only keyboard, the navigation order is logical and intuitive. Each page can also be reached using a Jump to Content option with the first tab on the page.
9. Can you always see where the keyboard focus is? <br>
Yes, the keyboard focus only work for navigation, button and input.
10. Does the user have access to the full functionality of the page or application using a keyboard alone? <br>
Users can fully interact with every interactive aspect of a web page using keyboard alone (no mouse). All information or functionality can be triggered with a mouse accessible and operable with a keyboard alone.

#### Form Fields
11. Do all form felds have appropriate labels? <br>
Yes. aXe does not detect any issues related to labels. 

#### Screen Reader
12. Is all content and functionality available to a screen reader? <br>
By using VoiceOver, users have access to all information and features on the page, and complete all tasks independently.

### Advanced JS or jQuery
#### Carousel
**Implementation is on the Foodie Blog Page**<br>
By importing css and js files from an online carousel implementation called Slick `http://kenwheeler.github.io/slick/`, I established my own carousel. One of challenges I faced was color contrast issue. After a close scrutiny, I found some imported carousel elements have a transparent background color. Therefore, I wrote classes to override the background color of the imported carousel elements. The concept to learn for this implementation is how to adjust color contrast and override the class elements.

#### Lightbox
**Implementation is on the Gallery Page**<br>
Implementation of Lightbox is also imported from an online material `https://lokeshdhakar.com/projects/lightbox2/`. The new concepts are the differences of data-lightbox, data-title and data-alt, which is also the challenge I met. At the beginning, I assigned data-lightbox of each image into different texts mistakenly, so the lightbox did not work. Writing each attribute with correct text/value requires complete understanding of the instructions.

#### Modals
**Implementation is on the Contact Page by clicking the phone icon/number**<br>
Modal is written by bootstrap. The new concepts to learn are bootstrap, telephone protocol as well as CSS cursor property. Taking example of the last concept. When hovering the phone icon/number, the mouse cursor default display trigger for indicating the link. The challenge for this implementation is bootstrap since we did not learn much bootstrap in class.

### Advanced proficiency with Bootstrap
- Implementation of navigation bar is written by bootstrap 3<br>
- Modal is written upon bootstrap 3 <br>
Challenge of writing bootstrap is due to unfamiliar with bootstrap. Therefore, I read official document to know available classes of bootstrap that could be used for my site.


