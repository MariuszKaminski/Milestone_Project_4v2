<h1 align="center">PROTEIN SHAKES N SNACKS<h1>

<p align="center">
    <a href="https://protein-shakes-n-snacks.herokuapp.com/">View the live project here.</a>
</p>

## This is a web based application designed for the sale of takaway shakes and protein snacks.

<h2 align="center"><img src="https://i.ibb.co/b7R6sqF/responsive-design.png"></h2>

-   ## User Experience (UX)

-   ### User stories

    -   #### First Time User Goals

        1. As a Guest, I want to easily easily navigate the web app.
        2. As a Guest, I want to be able to browse and search the menu.
        3. As a Guest, I want to be able to register with the website to speed up the purchase process.
    
    -   #### Returning Visitor Goals

        1. As a Registered User, I want to be able to log into my profile.
        2. As a Registered User, I want to be able to store some of my details on the site for faster checkout <br>
        and be able to see a history of my previous orders.
        3. As a Registered User, I want to receive a confirmation of my order with order details for reference.
    
    -   #### Frequent User Goals

        1. As a Staff Member, I want to be able to manage products, orders and users.        
        2. As a Staff Member, I want to the website to safely create and store orders in a database.
        3. As a Site Owner, I want only authorized staff members to have access to Django admin area <br>
        and be able to grant or withdraw authorization.
        

-   ### Design

    -   #### Color Scheme
        -   The application's two main colours are black and white for simple and maximum contrast and legibility.

    -   #### Typography
        -   The font of choice for the application is Roboto Google font with Sans-Serif as backup.

    -   #### Imagery
        -   The background image is used for aesthetic purposes and to ecourage user's interaction with the site. <br>
            The product page contains images of products up to four in a row.

-   ### Wireframes
    
    -   Homepage [View](/media/Homepage.png)

    -   Products [View](/media/Products_page.png)

    -   Product Details [View](/media/Product_details.png)

    -   Shopping Bag [View](/media/Shopping_bag.png)

    -   Checkout [View](/media/Checkout.png)
    
## Features

- Responsive on all device screen sizes as shown above - image obtained at [Am I Responsive?](https://ui.dev/amiresponsive)

- Interactive elements 
    - Actions involving login, registration, modifying shopping bag contents, purchases and editing product are confirmed with feedback messages [View](/static/img/feedback_message.png) 
    - Shopping bag provides on amount that needs to be spent to obtain free delivery [View](/static/img/low_stock_warning.png)

- CRUD functionalities available at Django admin page for authorized staff members and site owner (i.e Super User)

## Technologies

### Languages Used

-   [HTML5](https://en.wikipedia.org/wiki/HTML5)
-   [CSS3](https://en.wikipedia.org/wiki/Cascading_Style_Sheets)
    [JavaSript](https://en.wikipedia.org/wiki/JavaScript)
-   [Python](https://www.python.org/)

### Frameworks, Libraries & Programs Used

1. [AWS:](https://aws.amazon.com/)
    - Amazon Web Services is used for media and static files cloud storage.
1. [diagrams.net:](https://app.diagrams.net/)
    - Web based application diagrams.net is used to create wireframes during the design stage of the project.
1. [django](https://www.djangoproject.com/)
    - A python web framework used to create web app structue (views, templates and linking) and functionalities (authentication, admin).
1. [ElephantSQL](https://www.elephantsql.com/)
    - ElephantSQL is used to create an external database that can be used by the web app deployed at Heroku.
1. [Font Awesome:](http://fontawesome.com/)
    - Font Awesome was used on all pages throughout the website to add icons for aesthetic and UX purposes.
1. [Git:](https://git-scm.com/)
    - Git was used for version control by utilizing the Gitpod terminal to commit to Git and Push to GitHub.
1. [GitHub:](https://github.com/)
    - GitHub is used to store the projects code after being pushed from Git.
1. [Heroku:](https://www.heroku.com/)
    - Heroku is cloud application platform used to host the web app for online access.


## Testing

The W3C Markup Validator and W3C CSS Validator Services were used to validate every page of the project to ensure there were no syntax errors in the project.

-   [W3C Markup Validator](https://validator.w3.org/) - [Results](media/html_markup_validation_versults.PNG) <br>
    Please note that even though the html validatation shows errors, these are all related to the use of Flask values in curly brackets and Jinga templating language expressions which are essential for the app's functioning.
-   [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input) - [Results](media/CSS_validation_results.PNG)
-   Efforts were made to assure compliance of the Python code with the [PEP8 Style Guide](https://peps.python.org/pep-0008/) in terms of layout, line length, indentation, blank lines, etc.

### Testing User Stories from User Experience (UX) Section

    #### First Time User Goals

    1. As a Guest I can access all the main functionalities (i.g product page, login/registration, bag) with one click.
    2. As a Guest, I can easily find the items I'm interested in by using the search box or form drop down menus.
    3. As a Guest, I can register as a site user.

-   #### Returning Visitor Goals

    1. As a Registered User, I can log into my profile using my username and an email address.
    2. As a Registered User, I can acces my profile and save my delivery, payment and personal details at the site for faster checkout <br>
    as well as view my previous orders' history.
    3. As a Guest/Registered User, I receive a confirmation of my order with order details for reference both on the website and by email.

-   #### Frequent User Goals

    1. As a Staff Member, I can manage products, orders and users through Django admin area.        
    2. As a Staff Member, I can rely on webhooks sent by Stripe as a redundant method of creating and storing orders in a database.
    3. As a Site Owner, I can grant authorization to staff members and withdrwa it through Django admin area. <br> 
    Unauthorized users are not unable to access Django admin area.

### Further Testing
-   Black box testing schedule. [View](https://docs.google.com/document/d/1Jl3OG22ZebmyAGIBUtjNv4lRYiGg8pyabqFY4PEP0jc/edit?usp=sharing)
-   The website was tested on Google Chrome, Internet Explorer and Microsoft Edge.
-   The website was viewed on a variety of devices such as Desktop, Laptop and Android phone.
-   Testing included checking that all pages were linking correctly.

### Known Bugs

-   Webhooks in Stripe showing webhook delivery 505 error for payment.intent.succes.
-   Html markup validation throws 'Duplicate ID' error.
-   The website fails to sent out an order confirmation email.

## Deployment

-   The app files have been manually deployed from a GitHub repository to a newly created Heroku app. The following commands have been executed in a Gitpod bash terminal:<br>
    1.  heroku login -i
    2.  heroku create app_name_here
    3.  git push heroku main

## Credits

### Code
-   The code has been largely based on [Code Institute's](https://codeinstitute.net/) 'Boutique Ado' tutorial in 'Full Stack Frameworks with Django' section by [Tim Nelson](https://github.com/TravelTimN).

### Content
-   Chocolate Protein Shake description and nutritional values [Chelsea's Messy Arpron](https://www.chelseasmessyapron.com/triple-chocolate-chunk-brownie-protein-shake/)
-   Coffee Protein Shake description and nutritional values [Love & Zest](https://www.loveandzest.com/coffee-lovers-protein-shake/)
-   Cookies and Cream Protein Shake descritption and nutritional values [The Seasoned Mom](https://www.theseasonedmom.com/cookies-and-cream-protein-shake/)
-   Strawberry and Banana Protein Shake descritption and nutritional values [The Protein Chef](https://theproteinchef.co/strawberry-banana-protein-shake-recipe/)
-   Peanut Butter Protein Shake descritption and nutritional values [eating bird food](https://www.eatingbirdfood.com/peanut-butter-protein-shake/)
-   Protein Packed Skinny Frozen Mocha description and nutritional values [Nutrition Starring YOU](https://nutritionstarringyou.com/protein-packed-skinny-frozen-mocha/)
-   Salted Caramel Mocha Protein Frapé descripion and nuritional values [The Seasoned Mom](https://www.theseasonedmom.com/salted-caramel-mocha-protein-shake/)
-   Vanilla Frapé descripion and nuritional values [foodfanatic](https://www.foodfanatic.com/recipes/healthy-homemade-vanilla-frappuccino-recipe/)
-   Reign Peach Fizz descripion and nuritional values [musclefood](https://www.musclefood.com/reign-peach-fizz.html)
-   Moose Juice Berry description and nutritional values [musclemoose](https://musclemoose.co.uk/product/berry/)
-   Protein Dynamix BCAA Amino Energy descripion and nuritional values [musclefinessewholesale](https://musclefinessewholesale.com/protein-dynamix-bcaa-amino-energy-12-x-500ml.html)
-   Chocolate Chip Salted Caramel Protein Bar description and nutritional values [musclefood](https://www.musclefood.com/chocolate-chip-salted-caramel-grenader-carb-killatm-bar-12-x-60g.html)
-   The Big Protein Flapjack - Peanut Butter description and nutritional values [musclefood](https://www.musclefood.com/the-big-protein-flapjack-peanut-butter-24.html)
-   Cheese And Onion Protein Crisps description and nutritional values [Shake That Weight](https://www.shakethatweight.co.uk/shop/fitness/protein-crisps/cheese-onion-crisps)
-   Banana Protein Pancakes description and nutritional values [Healthy Fitness Meals](https://healthyfitnessmeals.com/banana-protein-pancakes/)
-   Peanut Butter Blueberry Protein Cookies description and nutritional values [Hayl's Kitchen](https://www.haylskitchen.com/pb-blueberry-protein-cookies/)
-   All remaining content was written by the developer.

### Media
-   Background image for the app is a free stock photo by Kindel Media at [Pexel](https://www.pexels.com/pl-pl/zdjecie/koktajl-sloj-odswiezenie-zimne-napoje-8181548/)
-   Chocolate Protein Shake image [Chelsea's Messy Arpron](https://www.chelseasmessyapron.com/wp-content/uploads/2013/10/Chocolate-Protein-Shake-1.jpg)
-   Coffee Protein Shake image [Love & Zest](https://www.loveandzest.com/wp-content/uploads/2019/02/Coffee-Protein-Shake-Web-Ready-8-640x960.jpg)
-   Cookies and Cream Protein Shake image [The Seasoned Mom](https://www.theseasonedmom.com/wp-content/uploads/2018/12/Cookies-and-Cream-Protein-Shake-8a.jpg)
-   Strawberry Banana Protein Shake image [The Protein Chef](https://media.theproteinchef.co/wp-content/uploads/2021/08/Strawberry-Banana-Protein-Shake-Recipe-683x1024.jpg)
-   Peanut Butter Protein Shake image [eating bird food](https://www.eatingbirdfood.com/wp-content/uploads/2021/07/peanut-butter-protein-shake-in-cup-633x950.jpg)
-   Protein Packed Skinny Frozen Mocha image [Nutrition Starring YOU](https://www.simplyhappyfoodie.com/wp-content/uploads/2019/07/iced-coffee-protein-shake-1b.jpg)
-   Salted Caramel Mocha Protein Frapé [The Seasoned Mom](https://www.theseasonedmom.com/wp-content/uploads/2015/03/Salted-Caramel-Mocha-Protein-Shake-17.jpg)
-   Vanila Frapé image [foodfanatic](https://food-fanatic-res.cloudinary.com/iu/s--Qr4q1aJB--/t_xlarge_p/cs_srgb,f_auto,fl_strip_profile.lossy,q_auto:420/v1502748400/healthy-homemade-vanilla-frappuccino-pic.jpg)
-   Reign Peach Fizz image [musclefood](https://d3rxe6nylop6k3.cloudfront.net/catalog/product/cache/1/image/530x/9df78eab33525d08d6e5fb8d27136e95/m/o/monster-reign-peach-fizz-500ml-mf_dr391_sample_1.jpg)
-   Moose Juice Berry image [musclemoose](https://musclemoose.co.uk/wp-content/uploads/2021/04/MooseJuice_Berry-Flavour-Can_Single-600x849.png)
-   Protein Dynamix BCAA Amino Energy image [musclefinessewholesale](https://musclefinessewholesale.com/media/catalog/product/cache/21d694c873907d78b2b1c9b0cbd4c5fc/t/r/tropical_energy_drink.jpg)
-   Chocolate Chip Salted Caramel Protein Bar image [musclefood](https://d3rxe6nylop6k3.cloudfront.net/catalog/product/cache/1/image/530x/9df78eab33525d08d6e5fb8d27136e95/g/r/grenade-chocolate-chip-salted-caramel-carb-killa-bar-60g-mf_sn1168_box_4.jpg)
-   The Big Protein Flapjack - Peanut Butter image [musclefood](https://d3rxe6nylop6k3.cloudfront.net/catalog/product/cache/1/image/530x/9df78eab33525d08d6e5fb8d27136e95/m/u/muscle-moose-big-protein-flapjack-peanut-butter-100g-mf_sn1503-x24.jpg)
-   Cheese And Onion Protein Crisps image [Shake That Weight](https://www.shakethatweight.co.uk/wp-content/uploads/2020/11/EP-Cheese-Onion-Protein-Crisps_WO-1024x1024.jpg)
-   Banana Protein Pancakes image [Healthy Fitness Meals](https://healthyfitnessmeals.com/wp-content/uploads/2018/06/banana-protein-pancakes-3.jpg)
-   Peanut Butter Blueberry Protein Cookies description and nutritional values [Hayl's Kitchen](https://i0.wp.com/www.haylskitchen.com/wp-content/uploads/2022/08/Peanut-Butter-Blueberry-Protein-Cookies-2.jpg)
### Acknowledgements
-   Also many thanks to my Harlow College tutor Patrick Justus Phd who provided me with input on black box testing.