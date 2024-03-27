Quuestion.1:- For the given index.html file. Perform the following task, without changing the index.html file.
#style.css
/*Question:B (a):- Use any of the css combinator selectors to target all the anchor tags and change the text color to red.*/
            nav a {color:red;
            }


            /* (b):- Target only the first <h2> tag and change the text and background color using the combinator selector*/
                nav > h2{
                    color:rgb(85, 14, 14);
                    background-color:rgb(235, 224, 224);
                }
                
            /* (c):- Also, select the first <p> tag and change the text color to red. */
                ul + p {
                    color: red;
                }


             /* Question:c (a):- Target the anchor tag with attribute "href" and change color to red and remove the text underline   */
             a [href] {
                color:red;
                text-decoration:none;
             }



             /* (b):- Target the anchor tag with the attribute of class name "active", change the text color, and provide the text style properties with underlining. */
           a [class="active"] {color:aqua;
                         text-decoration: underline;
             }


             /* (c):- Target the anchor tag with the attribute of the target whose value is "_self" and change the background color. */
             a [target="_self"] 
                {background-color:grey;

             }


             /* Question:D (a):- Target the last <p> tag and add "..." i.e. three dots after its value*/
                p:last child::after {
                    content:"..."

                }

            /* (b):- Target the list of bullet points and change the color of the bullet points without changing the list item's value. */
            li::marker {
                color:green;
            }


            /* (c):- Among the three <p> tags target the 2nd <p> tag, select the first letter of the second <p> tag, and change the color to red also increase the font size to 30px */
                p:nth-child(even)::first-letter {
                    color:red;
                    font-size:30px;
                }


Qestio.2:- For the given index.html file. Perform the following task, without changing the index.html file.
    :- Use the descendant combinator selector to remove list style type bullet points and text underlining of the menu list items.
    :- Use the child combinator to display the menu list item inline 
    :- Use the Ajacent sibling combinator selector to apply some margin between the menu lit items.

Answer:- 
#style.css
/* task one-use descendant combinator selector to remove list style bullet points --> */
    ul  li a {
    list-style:none;
    text-decoration:none;
}
/* task two - use child combinator to display the menu list item inline */
    ul > li {
        display: inline;
    }

    /* task three - se adjacent sibling combinator selector to apply some margin between the menu list item */
    li + li {
        margin: 10px;
    }

Question.3:-  Using any of the pseudo element selectors, add any random words after andd before the given HTML tag  index.html
Answer:- 
#style.css
h1:: after {
content:"selector"
}
h1::before {
content:"pseudo";
}


Question.4:- Illustrate one example of pseudo-class element selector hover example should inclde the following -
:- An example should be one HTMl button tag
:- When hovering the color should be changed and the shadow of the button should be added.
:- Proper padding space should be given.
:- The cursor style should also be changed to the pointer on hover

Annser:-  
#style.css

Button{
background-color: blue;
border:none;
margin-top:100px;
margi-left:100px;
padding:15px 30px;
color:white;
font-size:10px;
}
Button:hover{
Box-shadow:10px 5px 5px grey'
Cursor : Pointer;
}

