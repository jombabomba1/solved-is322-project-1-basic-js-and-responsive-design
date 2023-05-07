Download Link: https://assignmentchef.com/product/solved-is322-project-1-basic-js-and-responsive-design
<br>
In this assignment you will be tasked with creating a simple E-Commerce site with a basic set of features. A landing page to advertise your site and some of your top selling products, a product list where the user can view all your products with filters and sorting, and a product page for viewing information on a specific product (only required for 3 person groups)




The <strong>instructions</strong> below give a step-by-step guide for creating each of the pages, as well as provide visual examples. You can however not follow them and just make sure your pages match all the <strong>requirements</strong>. Bootstrap CSS is allowed, but not any of it’s JavaScript

Components. Anything above and beyond the original requirements will be considered for extra credit.




This assignment only requires HTML, CSS, and JavaScript so it won’t be required to be fully functional, only using mock data to display products. There is no back-end component required for this assignment.




<h1>General Requirements</h1>

<ol>

 <li>All code must be in GitHub, and the website should be publicly accessible from at least one of your group members AFS web spaces. Both links will be required.</li>

 <li>All pages should be responsive, and can be easily viewed on the following resolutions, you do not need to specifically code for these resolutions, these are just the ones I will be testing:

  <ol>

   <li>1366px wide (Large Desktop)</li>

   <li>1024px wide (Small Desktop)</li>

   <li>768px wide (Tablet)</li>

   <li>411px wide (Phone)</li>

  </ol></li>

 <li>Not using Bootstrap at all and doing all the responsive work yourself will reward 20 points of extra credit on this project</li>

</ol>










<h1>Part 1: Landing Page (Required to Teams of 2+)</h1>




<h2>Description</h2>

Landing pages are typically the first page the user sees when they go to your site, it’s your index.html, your welcoming mat. As such it should give your potential customers a reason to stay, with information about your company/store as well as some examples of products and services you offer.




<h2>Requirements</h2>

<ol>

 <li>Some kind of Primary Navigation that allows your users to navigate to the product list and any other potential pages.</li>

 <li>A Carousel at the top of the page that displays various products or sales you have going on. Should change automatically every 3-5 seconds to display another. Should contain at least 3 slides.</li>

 <li>A blurb about your company on the bottom of the page (can use Lorem Ipsum text generator)</li>

 <li>A footer containing all of your fake companies’ information (Phone Number, Address, links to social media)

  <ol>

   <li>Horizontally on Desktop</li>

   <li>Vertically on Mobile</li>

  </ol></li>

</ol>

<h2>Instructions</h2>

<ol>

 <li>Create an <em>html</em> and <em>landing.js </em>files and add them to the product.</li>

 <li>Populate your <em>html </em>file with the basic HTML page structure. Make sure to include your <em>landing.js </em>file at the end of the body tag.</li>

 <li>Either make or include an existing CSS file within the HEAD tag using the LINK tag. (Also include bootstrap at this point if you so choose)</li>

 <li>Create a Navigation Menu to link to other pages of your site, you can make it yourself from scratch or use this (<u>https://getbootstrap.com/docs/4.3/components/navbar/</u>). Either way just make sure it works well on all tested resolutions. You only need 2 links, so collapsing isn’t necessary (will give extra credit for it though)</li>

 <li>Add a DIV tag at the top of the page containing 3 images. Create an <em>active </em>class for the image that sets the DISPLAY to BLOCK, while the default styling for the image will have a CSS DISPLAY property of NONE. This will make it so only image is displayed at a time.</li>

 <li>In your <em>js </em>JavaScript file, create a function that removes the active class from one slide and adds it to another. It should be able to keep track of the current slide with a variable declared outside of the function and be able to loop back to the first slide after it reaches the end.</li>

 <li>Use the setInterval Method</li>

</ol>

(<u>https://www.w3schools.com/jsref/met_win_setinterval.asp</u>) to call your function at regular intervals. (time is in milliseconds so 1 second = 1000ms)

<ol start="8">

 <li>Add Description of company that contains at least a title and 3 paragraphs (can use text generator)</li>

 <li>Add a footer on the bottom of the page that displays the text horizontally on desktop and vertically on mobile. Can use FLEXBOX, setting the CSS property FLEX-DIRECTION from row to column based on a media query.</li>

</ol>




<h2>Examples Desktop</h2>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<h2>Mobile</h2>




<h1>Part 2: Product List</h1>




<h2>Description</h2>

Your product list is where your customer can search for the exact product that meets their needs. To allow for this you should provide several filters and sorting options to let your users narrow down your vast inventory to the specific product they’re looking for (think Amazon).




<h2>Requirements</h2>

<ol>

 <li>A Filterable list of products. Each product item should contain an image, title, price and price. (NO TABLES)</li>

 <li>A set of filters to narrow down the list. Should have a least 2. Some suggestions <strong>IF </strong></li>

</ol>

<h2>GROUP OF 3 PEOPLE YOU’LL NEED 4 FILTERS. ADD META DATA TO YOUR DATABASE TO FILTER BY IF NECESSARY</h2>

<ol>

 <li>Price Range</li>

 <li>Meta data fields you don’t need to display (ex. Category, Screen Size, Department)</li>

 <li>The ability to sort the list by at least two fields. Recommended sorting options: Price (1-10)</li>

 <li>Title (A-Z)</li>

 <li>List should be able to be viewed comfortably on any of the previously stated resolutions</li>

</ol>




<h2>Instructions</h2>

<ol>

 <li>For the JavaScript portion of this assignment, the <em>AdvancedJS </em>repository from week 3 provides a lot of examples. Just as the <em>Media Queries </em>repository from week 2 will provide examples of CSS.</li>

 <li>Create a <em>html and productList.js </em>file and include them in your product.</li>

 <li>Populate your <em>html </em>file with the basic HTML page structure. Make sure to include your <em>productList.js </em>file at the end of the body tag.</li>

 <li>Either make or include an existing CSS file within the HEAD tag using the LINK tag. (Also include bootstrap at this point if you so choose)</li>

 <li>Create an area to contain your filters and add the relevant form inputs. Dropdowns or text inputs tend to work best.</li>

 <li>Add a div to you page with an ID, this will eventually be populated with your list data, but should be empty for the time being.</li>

 <li>In the <em>js </em>create a mockDatabase of JavaScript objects to render into your HTML.</li>

 <li>Create a <em>renderList </em>function similar to that of <em>AdvancedJS </em>and to render out your mockDatabase into your HTML. Some things to consider:

  <ol>

   <li>Make sure you clear out innerHTML first.</li>

   <li>Don’t use the mockDB variable directly, pass in a parameter. As we’ll be rendering different lists later.</li>

  </ol></li>

 <li>Hook up a sorting function via an event listener similar to that of Some things to keep in mind are strings and numbers need different strategies for sorting.</li>

 <li>Create 2 filters for your data based off the examples from Advanced JS. By listening to the change event on your DropDowns or Text Inputs you can get the value of it and use the Array.filter function to pass a new data set to your renderList function.</li>

 <li>Use media queries to position your filters on the side of the page for Desktop views, and the top of the page for mobile views. Examples of this can be found in the <em>Media Queries </em>Repository from week 2.</li>

 <li>Make sure your list always looks good on all screen resolutions I will be test, use the <em>Media </em></li>

</ol>

<em>Queries </em>Repository and the following examples for insight




<h2>Examples</h2>

<strong> </strong>

Desktop











































Tablet







Mobile













<h1>Part 3: Product Details (Only required for 3-person teams)</h1>




<h2>Description</h2>

After the user has sorted through your list and picked a product they might want to buy, they should be able to drill down and find out more information about it. That’s where the product details page comes in handy, it gives more information than the list view and also allows the user to focus on a single product as opposed to slipping they’re focus.




<h2>Requirements</h2>

<ol>

 <li>Page should declare a JavaScript Object somewhere before the main script contain the meta data for the page. Nothing should be hardcoded and instead pull it’s data from the JavaScript Object. This is so we can eventually replace it with an API call to properly display product data.</li>

 <li>Page should display all the basic Product information in a stylized way.

  <ol>

   <li>Product Title</li>

   <li>Price and a (fake) button to buy/add to cart</li>

   <li>Image that was displayed on list view.</li>

   <li>The brief description from the Product List</li>

  </ol></li>

 <li>Product should have a longer description stored in the JavaScript Object. This description can contain HTML tags (Can use Lorem Ipsum Text generator with some added HTML). When displayed on the page, the HTML tags should be rendered as expected. Each description should contain at least.

  <ol>

   <li>One Header Tag</li>

   <li>One Paragraph Tag</li>

   <li>One Strong Tag (for bold)</li>

  </ol></li>

</ol>




<h2>Instructions</h2>

<ol>

 <li>Follow Instructions 1-4 from previous pages. Just instead creating <em>html </em>and<em> productPage.js. </em></li>

 <li>Create a page that displays all of the information for a product. There are no real requirements other then make it look as good as possible and make sure all the required information is displayed.</li>

 <li>Within <em>js </em>copy and paste your mock database from the product list. Select a product from the array to set as the main product for this page. Ideally you’d be making a request to an API to get this product, but we don’t have that for now.</li>

 <li>For extra credit make it a random product from the array (generate a random number index using Math.random()) so I can check that it works for all your products.</li>

 <li>After getting the product from the array, get reference to and set the innerHTML of all the elements on your page that should normally contain data. Tip, setting an ID for each element you want to populate will make it easier.</li>

</ol>




<h2>Examples</h2>

<strong> </strong>

Desktop







Mobile













Important:




<ol>

 <li>Track changes to your code using GitHub</li>

 <li>Submit your AFS link and GitHub link to the app on Moodle Both Links are required, if you missed one of them, you get 20% off from full credit.</li>

 <li>10% off for every day late.</li>

 <li>You will receive a grade for the project as a whole, and an individual grade for your contributions.</li>

</ol>


