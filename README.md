WP Member Registration Form UI Manipulation with Simple JQuery Solution:

For the site Neuro Proteccion, JQuery was used to manipulate the theme based form provided by WP members plug in. The form is all based in dynamic php no html so in order to change the layout and structure of this form, JQuery was the most effective solution. 

If you visit http://neuroproteccion.com/registrate/ you will see a registration form built on Wordpress with a custom theme 
I changed to the style, design, and structure of how the client wanted this website to be. 

The customer required a registration form to log in to there account so the solution was to use the WP Members plug in which
provided the most effective solution in providing a registration form quickly for the client. 

The downfall however eventhough it is a great plug in, for this form however in order to change the layout of the design which is different from the standard structure the plug in provided, the form could only be changed with very complicated specific built in hooks which I thought in my opinion was not very clear and effective.

For this reason I decided to use the solution of manipulating the form structure and layout with JQuery. As you can see in the 
file provided, the file is the standard registration template I am using for the structure of the page with the JQuery code
included that first replaces the elements on the form to my like and then uses the JQuery method .wrapAll to achieve this
solution. 

- The file starts off with the wordpress codex to call the template in order to be used on the specific page. 

- Then grabs the other files the theme uses for the structure of the page: 

- Then the wrapper containers which are the div containers for the form followed by the WP Members short code to dynamically show the form with the short code provided by the WP Members plug in. 

- This form will be closed later on but showing the code piece by piece as to how I got this working. Then comes the actual JQuery code first to add a new class to the form and remove the old .form class which was not easy to target. 

 - After creating this new class and replacing the .form class, the classes .text and .div_text needed to be wrapped in another class which would be very tough to accomplish this with the complicated hooks the plug in provided. So for the purpose of having the form elements show up next to each other as opposed to full width which was different from the clients design, I created this jquery function with the method .wrapAll around these two classes which was exactly what I needed to do and thanks to JQuery, this would be much easier. 
  
- After that process was done, you have the ending closing div's of the wrapper containers holding the form followed by the wordpress get sidebar, and get footer syntax. 

             
