# AspNetTester

1.  Install Visual Studio: https://www.visualstudio.com/en-us/products/visual-studio-community-vs.aspx
2.  Install Web Essentials 2013: https://visualstudiogallery.msdn.microsoft.com/56633663-6799-41d7-9df7-0f2a504ca361
3.  Install SourceTree: http://sourcetreeapp.com/
4.  Create Github account and fork this repository: https://github.com/lepipele/AspNetTester
5.  Using SourceTree clone repository locally
6.  Cut PSD from landing_page.psd.zip into HTML and import it in Visual Studio Solution contained in Solution folder
7.  If you need help with ASP.NET implementation take a look at Solution\AspNetTester\Project_Readme.html
8.  While working keep commiting to your repository so work history can be reviewed. Few rules regarding commits:
    - Atomic, descriptive commits instead of one huge commit – so:
        - Feature 1 commit 
        - Feature 2 commit 
        - Feature 3 commit 
    - And not:
       - Feature 1, Feature 2, Feature 3 in single commit
    - Obviously “Feature 1,2,3” is bad description – be descriptive in your explanation of commit
    - Commit needs to be atomic in a sense: do not commit if what you did breaks build
9.  Once you are done with implementation email link to your GitHub repository

## Learning resources

This section aims to break down step 6 from main list. Your implementation of PSD should basically end up being:

1. Defining _Layout.cshtml - master page with common elements that will be used by each page
2. Linking needed .JS javascript files from _Layout.cshtml - if you are using frameworks like jQuery or AngularJs. Do not worry about bundling for now - we'll get to that later.
3. Linking needed .CSS files from _Layout.cshtml - plus if you are using SCSS and linking resulting CSS file.
4. Creating Controller with Actions for each partial page and implementing appropriate .cshtml files that use _Layout.cshtml defined in step 1
 
Easier said then done, right? Well, here are some links that should help you with learning:
- If you don't even know JavaScript/CSS, or want to refresh your knowledge, check out these tutorials:
    -   http://www.w3schools.com/js/default.asp
    -   http://www.w3schools.com/css/default.asp
- If you know CSS, but don't know SCSS and want to learn basics, visit: http://sass-lang.com/guide
    - To try out examples you'll need to follow steps 1 & 2 from main list and install Visual Studio & Web Essentials
- ASP.NET MVC learning - obviously this is huge topic. But for start you just need to get creation of .cshtml files / Razor under your belt. I.e. if you already have some experience with PHP this should be easy-peasy - instead of doing <?php echo "Hello World!"; ?> you'll be doing @Html.Raw("Hello World!"). Here is the list of links that should be helpful:
    -  http://www.asp.net/mvc/overview/getting-started/introduction/getting-started
    -  http://www.w3schools.com/aspnet/razor_intro.asp
    -  https://www.youtube.com/watch?v=pEfFySUIeBk
    -  If you are book reading type, any Amazon 5 star rated book on ASP.NET MVC will do, like this one: http://www.amazon.com/Professional-ASP-NET-MVC-Jon-Galloway/dp/1118794753