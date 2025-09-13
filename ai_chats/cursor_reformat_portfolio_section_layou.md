# Reformat portfolio section layout
_Exported on 9/13/2025 at 13:21:28 EDT from Cursor (1.5.11)_

---

**User**

please reformat the index.html file so that in the portfolio section,  we remove the three column format. instead, make it two columns, where the main body of each project appears above the skills used section in one column, and the image appears in the other column. alternate the images left to right.

---

**Cursor**

I'll help you reformat the portfolio section in your index.html file. Let me first read the current file to understand the structure and then make the requested changes.


Now I'll create a todo list to track the changes needed and then implement the reformatting:


Now I'll implement the reformatting. I'll start with the VoteKit section and work through each project, alternating the image placement as requested:


```html
<!DOCTYPE html>
<html lang="en">
<head>

     <title>Christopher Donnay</title>

     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="Tooplate">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/all.min.css">
     <link rel="stylesheet" href="css/owl.carousel.min.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/tooplate-ben-resume-style.css">
    
    <!-- Custom link styling for about and portfolio sections -->
    <style>
        #about a, #portfolio a {
            color: #3182ce !important;
            text-decoration: underline !important;
        }
        
        #about a:hover, #portfolio a:hover {
            color: #2b6cb0 !important;
            text-decoration: underline !important;
        }
    </style>
<!--
Tooplate 2120 Ben Resume
https://www.tooplate.com/view/2120-ben-resume
-->
</head>

<body data-spy="scroll" data-target="#navbarNav" data-offset="50">

    <!-- MENU BAR -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">

            <a class="navbar-brand" href="#">
                Christopher Donnay
            </a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item">
                        <a href="#about" class="nav-link smoothScroll">About Me</a>
                    </li>

                    <li class="nav-item">
                        <a href="#portfolio" class="nav-link smoothScroll">Portfolio</a>
                    </li>

                    <li class="nav-item">
                        <a href="#contact" class="nav-link smoothScroll">Contact</a>
                    </li>
                </ul>

                <div class="mt-lg-0 mt-3 mb-4 mb-lg-0">
                    <a href="files/CDonnay Resume.pdf" class="custom-btn btn" target="_blank">Download Resume</a>
                </div>
            </div>

        </div>
    </nav>


    <!-- HERO -->
    <section class="hero d-flex flex-column justify-content-center align-items-center" id="intro">

         <div class="container">
            <div class="row about-third">

                  <div class="mx-auto col-lg-5 col-md-5 col-10">
                      <img src="images/color_cut_tree.png" class="img-fluid" alt="Cut tree">
                  </div>

                   <div class="d-flex flex-column justify-content-center align-items-center col-lg-7 col-md-7 col-12">
                        <div class="hero-text">

                            <h1 class="hero-title">Christopher Donnay</h1>

                            <a href="mailto:christopherdonnay@gmail.com" class="email-link">
                                christopherdonnay@gmail.com
                            </a>
                          
                        </div>
                    </div>

            </div>
        </div>
    </section>


    <section class="about section-padding" id="about">
        <div class="container">
            <div class="row">

                <div class="col-lg-6 col-md-6 col-12">
                    <h3 class="mb-4">About me</h3>

                    <p>Chris Donnay is currently the lab manager for  
                      <a rel="nofollow" href="https://www.mggg.org" target="_blank">the Data and Democracy Lab</a>
                      at Cornell University. 
                      As lab manager, he has extensive experience translating  
                      real-world problems into technical solutions for non-profits and advocacy groups.
                      He has a knack for communicating high-level mathematics to a wide range
                      of audiences, with a focus on clarity and actionable insights.
                      He got his PhD in mathematics from the Ohio State University, 
                      where he studied data science, probability, and statistical modeling, 
                      with applications to redistricting and voting.
                      Chris also holds a Master's of Science in education from the University of Pennsylvania, 
                      where he was a high school math and computer science teaching fellow.
                      </p>

      
                </div>
                
                <!-- Todo, edit the bounding box -->
                <div class="col-lg-5 mx-auto col-md-6 col-12">
                    <img src="images/cdonnay.jpg" class="about-image img-fluid" alt="CDonnay">
                </div>

            </div>
        </div>
    </section>

<section class="portfolio section-padding" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="mb-4">Portfolio</h3>
                    <p>Below are a smattering of Chris' past research projects, which include 
                      data science and modeling projects for democracy non-profits and advocacy groups,
                      applications and Python libraries for civic good, 
                      as well as more traditional mathematical research projects.
                    </p>
                </div>
            </div>

            <!-- VoteKit Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>VoteKit</h4>
                    <p>
                      <a rel="nofollow" href="https://github.com/mggg/VoteKit" target="_blank">VoteKit</a> is 
                      a one-stop shop for all things election modeling in Python. With an end-to-end pipeline for 
                      constructing ballots, running elections, and analyzing outcomes, VoteKit seeks to be a tool 
                      for academics, researchers, and practitioners alike.
                  </p>
                  <p>
                      Chris is the principal developer, manages the other open source contributors,
                      writes <a rel="nofollow" href="https://votekit.readthedocs.io/en/latest/" target="_blank">documentation and tutorials,</a> 
                      and designs, prototypes, evaluates, and 
                      implements new features for the package.
                    </p>


                    <p>
                      Read about more about VoteKit in the
                      <a rel="nofollow" href="https://joss.theoj.org/papers/10.21105/joss.07477" target="_blank">Journal of Open Source Software.</a>
                      </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Python</li>
                        <li>Package management: PyPI, Poetry</li>
                        <li>Statistical modeling</li>
                        <li>Documentation: Sphinx, Jupyter, Markdown</li>
                        <li>Open source software: GitHub</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/waterfall.png" class="about-image img-fluid" alt="VoteKit Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A plot showing how different models of ballot generator perform with respect
                            to proportionality under an STV election, generated by VoteKit.
                        </figcaption>
                    </figure>
                </div>
            </div>

            

            <!-- The VRA in Michigan Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/house_1_partial.png" class="about-image img-fluid" alt="MI Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A restricted area around Detroit where we focused our efforts on improving partisanship.
                            We refer to this as a "partial scramble", where we fix the rest of the state and 
                            only pertub this area.
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>The Voting Rights Act in Michigan</h4>
                    <p>
                      In 2024, Michigan's legislative maps were struck down as being in violation of the Voting Rights Act in
                      the Michigan Supreme Court case Agee v. Benson.
                      When it came time to create new maps, the advocacy group Voters Not Politicians
                      asked us to help them model ways to balance different metrics of partisanship with the Voting Rights Act.
                      </p>
                      <p>
                      Chris created a model of redistricting plans in Michigan, collecting data from 
                      public and private sources in order to produce maps that balanced different metrics of partisanship
                      with the Voting Rights Act. 
                      The results of our study influenced the creation of the new legislative maps 
                    used as a remedy for the case.</p>

                    <p>
                    While the non-technical summary for Voters Not Politicians is not publicly available, 
                    you can read <a href="files/Sampling Problems in Legislative Redistricting.pdf" target="_blank">the technical report</a>
                    which was included in Chris' thesis.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Geospatial data: Census, electoral</li>
                        <li>Markov chains: optimization, sampling</li>
                        <li>Technical solutions for political advocacy</li>
                        <li>Technical communication with non-technical audiences</li>
                        <li>Statistical modeling</li>
                    </ul>
                </div>
            </div>

            <!-- Portland OR STV Analysis Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>STV City Council Election in Portland, OR 2024</h4>
                    <p>In November of 2024, Portland, OR held their first city council election
                      with a single-transferable-vote (STV) system, electing 12 council members
                      across 4 districts. There was concern about how STV might impact the ability 
                      of communities of color to participate in the process.
                    </p>

                    <p>
                      Chris provided Python support to a 
                      <a rel="nofollow" href="https://mggg.org/PPM" target="_blank">
                        post-mortem study</a> of the election,
                      including processing of ballots with <code>pandas</code>, analysis of the election using <code>VoteKit</code>, 
                      developing visualizations with <code>matplotlib</code>, and explaining the code in a <code>Jupyter</code> notebook. 
                      The results showed that dominant media
                      narratives about ballot errors by people of color were misguided, and that STV actually 
                      helped increase representation of communities of color.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data cleaning: pandas</li>
                        <li>Data visualization: matplotlib</li>
                        <li>Statistical analysis: VoteKit</li>
                        <li>Python</li>
                        <li>Non-technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/D1-boost-V.png" class="about-image img-fluid" alt="Analyzing candidate similarity">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Understanding how similar candidates are in an STV election.
                            Candidate pairs (i,j) that are more green show a kind of "mutual boosting",
                            where if candidate j appears on a ballot, candidate i is more likely to appear on a ballot as well.
                            This reveals a slate of candidates (Avalos, Routh, Dunphy, and Ender) who all
                            mutually boost.
                        </figcaption>
                    </figure>
                </div>
            </div>

            <!-- The Great British Baking Show Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/freddy_cake.webp" class="about-image img-fluid" alt="GBBS Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Freddy? Is that you?
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Predicting Bake Off Winners</h4>
                    <p>
                      As part of the Erdős Institute Data Science Bootcamp, Chris and his team
                      trained supervised learning models using
                      <code></code>scikit-learn</code>—regression, random forest, k-nearest neighbors, and Naive Bayes—
                      to predict winners and uncover key
                      drivers of success in the Great British Baking Show. 
                      Ultimately, they found that the most important factor in predicting winners
                      was performance in the technical challenges (receiving a handshake
                      from Paul Hollywood turned out to be far less predictive than hoped!).                      
                    </p>
                      <p>
                      At the end of the bootcamp, they <a href="https://docs.google.com/presentation/d/1I0hSqWn0BLEwysViAbwRr-Zx7bJyoMH4HexAY2kCEHo/edit?usp=sharing" 
                      target="_blank">presented their results</a> 
                      to a panel of industry experts, 
                      who specifically highlighted the team's clear communication of modeling 
                      limitations and results. They were awarded first place.</p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data collection and cleaning</li>
                        <li>Machine Learning: KNN, Random Forest, Naive Bayes, Regression</li>
                        <li>Statistical analysis</li>
                        <li>Technical communication</li>
                        <li>Python: scikit-learn</li>
                        <li>Data visualization: matplotlib</li>
                    </ul>
                </div>
            </div>

            <!-- Districtr 2.0 -->
            <div class="row about-third mb-5">
              <div class="col-lg-8 col-md-8 col-12">
                  <h4>Districtr 2.0</h4>
                  <p>
                    <a rel="nofollow" href="https://beta.districtr.org" target="_blank">Districtr</a> is a web-based tool for creating 
                    districting plans. After many years of faithful service, Districtr 1.0 was retired and replaced with Districtr 2.0.
                    Districtr is used by many localities as their official submission tool for the redistricting process.

                  </p>

                  <p>
                    Chris was the product manager the development and public release of Districtr 2.0 
                    with a remote team of five full-stack developers. 
                    Together with his team, Chris ensured that the app was robust and scalable,
                    that there was smooth communication between the dev team and the PI,
                    and that the app was easy to use and understand.
                  </p>
                  
                  <h4>Skills Used</h4>
                  <ul>
                      <li>Project management</li>
                      <li>Non-technical communication</li>
                      <li>Full stack development</li>
                      <li>Geospatial data</li>
                  </ul>
              </div>
              <div class="col-lg-4 col-md-4 col-12">
                  <figure>
                      <img src="images/districtr.png" class="about-image img-fluid" alt="Districtr 2.0">
                      <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                          A map module for drawing Pennsylvania's congressional districts in Districtr 2.0.
                      </figcaption>
                  </figure>
              </div>
          </div>


          <!-- 3:1 nesting -->
          <div class="row about-third mb-5">
            <div class="col-lg-4 col-md-4 col-12">
                <figure>
                    <img src="images/biasing_house_maps.png" class="about-image img-fluid" alt="Districtr 2.0">
                    <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                        This histogram shows how the number of seats won by Democrats in the Ohio Senate varies based on the bias of the 
                        underlying House map. While the underlying House map is incredibly biased,
                        the distribution of seats won by Democrats in the Senate does not separate as widely.
                    </figcaption>
                </figure>
            </div>
            <div class="col-lg-8 col-md-8 col-12">
                <h4>3:1 Nesting Rules in Redistricting</h4>
                <p>
                  A nesting rule is a rule that requires that a senate district be composed of adjacent house districts.
                  Ohio and Wisconsin have 3:1 nesting rules (3 house districts per senate district).
                  How does this affect the space of feasible plans? How does this affect the ability of a map-maker to gerrymander?

                </p>

                <p>
                  Chris implemented a novel algorithm for generating plans that satisfy a 3:1 nesting rule
                  in Python using Markov chain methods. He validated his model using different mixing heuristics
                  and statistical tests. He found that while 3:1 nesting has little impact on the 
                  number of seats won by a party in comparison to unnested plans, it does 
                  curtail the impact of gerrymandered house maps and the ability to gerrymander more broadly.
                </p>

                <p>
                  Chris' paper is in revisions with the journal Statistics and Public Policy. 
                  Read the <a href="files/3_1_nesting.pdf" target="_blank">preprint here.</a>
                </p>
                
                <h4>Skills Used</h4>
                <ul>
                    <li>Python</li>
                    <li>Technical communication</li>
                    <li>Markov chains</li>
                    <li>Geospatial data</li>
                </ul>
            </div>
        </div>




            <!-- Asymptotics of Redistricting Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Asymptotics of Redistricting</h4>
                    <p>While much of Chris' work has been focused on applications of statistical models
                      and data science, his PhD is technically in theoretical mathematics, and he has a particular interest in combinatorics.
                      This project was part of his PhD dissertation, and is set to appear in the American Mathematical Monthly,
                      which is a prestigious journal known for its high standards of writing.
                      </p>
                      <p>
                      How many ways are there to redistrict an n×n grid into n districts? How does this grow with n? 
                      What can this tell us about the shape of a typical district? This mathematical research 
                      explores the combinatorial properties of redistricting and their implications for 
                      understanding gerrymandering. We find that the number of maps grows exponentially
                    in n^2, and that a random districting plan is likly to be highly non-compact.</p>
                    
                    <p>
                      Read the <a href="files/Asymptotics of Redistricting.pdf" target="_blank">preprint here.</a>
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Combinatorics</li>
                        <li>Asymptotic analysis</li>
                        <li>Technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/color_example_n_over_2_tiling.png" class="about-image img-fluid" alt="Tiling of the 8x8 grid">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A completed redistricting plan for the 8x8 grid (equivalent to a tiling!).
                            This completion is part of an algorithm that generates a lower bound
                            on the number of possible redistricting plans for the 8x8 grid.
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>
    </section>






     <section class="contact section-padding pt-0" id="contact">
      <div class="container">

            <div class="mx-auto col-lg-4 col-md-6 col-12">
                <h3 class="my-4 pt-4 pt-lg-0">
                  Say hello!
                </h3>
     
                <ul class="social-links mt-2">
                     <li><a href="mailto:christopherdonnay@gmail.com" rel="noopener" class="fas fa-envelope"></a></li>
                    <li><a href="https://www.linkedin.com/in/christopher-d-b1466b82" rel="noopener" class="fab fa-linkedin"></a></li>
                    <li><a href="https://github.com/cdonnay" rel="noopener" class="fab fa-github"></a></li>
                </ul>
                
              <p class="copyright-text mt-5 pt-3">Copyright &copy; 2020 Ben Resume Page</p>
                
                <p>Design: <a href="https://www.tooplate.com" title="free HTML templates" target="_blank">Tooplate</a></p>
            </div>

        </div>
      </div>
    </section>
     <!-- SCRIPTS -->
     <script src="js/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/custom.js"></script>

</body>
</html>
```

Now let me update the todo list to mark the completed tasks:


Let me check for any linting errors in the updated file:


Perfect! I've successfully reformatted the portfolio section in your `index.html` file. Here's a summary of the changes I made:

## Changes Made:

1. **Converted from 3-column to 2-column layout**: Each project now uses `col-lg-8` and `col-lg-4` instead of three `col-lg-4` columns.

2. **Alternating image placement** as requested:
   - **VoteKit**: Content + skills (left), image (right)
   - **Michigan VRA**: Image (left), content + skills (right) 
   - **Portland STV**: Content + skills (left), image (right)
   - **Baking Show**: Image (left), content + skills (right)
   - **Districtr 2.0**: Content + skills (left), image (right)
   - **3:1 Nesting**: Image (left), content + skills (right)
   - **Asymptotics**: Content + skills (left), image (right)

3. **Combined content and skills**: The main project description and the "Skills Used" section are now in the same column, with the skills appearing below the main content.

4. **Maintained responsive design**: The layout will still work well on mobile devices with the existing Bootstrap classes.

The layout now provides a cleaner, more streamlined appearance with better visual balance between text content and images, while alternating the image placement to create visual interest as you scroll through the portfolio.

---

**User**

Please do the following:
- vertically center the images in their columns
- change the font of the skills used sections and image captions to match the body font
- change the captions of the figures to be right aligned
- change the figure bounding boxes to have sharp corners instead of rounded edges

---

**Cursor**

I'll help you make those styling changes. Let me first examine the current CSS file to understand the existing styles, then implement the requested changes.


Now I'll create a todo list and implement the requested styling changes:


Now I'll add the custom CSS styles to the existing style section in the HTML file to implement all the requested changes:


```html
<!DOCTYPE html>
<html lang="en">
<head>

     <title>Christopher Donnay</title>

     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="Tooplate">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/all.min.css">
     <link rel="stylesheet" href="css/owl.carousel.min.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/tooplate-ben-resume-style.css">
    
    <!-- Custom link styling for about and portfolio sections -->
    <style>
        #about a, #portfolio a {
            color: #3182ce !important;
            text-decoration: underline !important;
        }
        
        #about a:hover, #portfolio a:hover {
            color: #2b6cb0 !important;
            text-decoration: underline !important;
        }
        
        /* Portfolio section customizations */
        /* Vertically center images in their columns */
        #portfolio .col-lg-4 {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        /* Change skills used sections to match body font */
        #portfolio h4 {
            font-family: var(--base-font-family);
            font-weight: var(--font-weight-light);
            color: var(--dark-color);
        }
        
        #portfolio ul {
            font-family: var(--base-font-family);
            font-size: var(--p-font-size);
            font-weight: var(--font-weight-light);
            color: var(--p-color);
            letter-spacing: 0.3px;
            line-height: 2em;
        }
        
        /* Change image captions to match body font and right align */
        #portfolio figcaption {
            font-family: var(--base-font-family) !important;
            font-size: var(--p-font-size) !important;
            font-weight: var(--font-weight-light) !important;
            color: var(--p-color) !important;
            letter-spacing: 0.3px !important;
            line-height: 1.5em !important;
            text-align: right !important;
        }
        
        /* Remove rounded corners from images */
        #portfolio .about-image {
            border-radius: 0 !important;
        }
    </style>
<!--
Tooplate 2120 Ben Resume
https://www.tooplate.com/view/2120-ben-resume
-->
</head>

<body data-spy="scroll" data-target="#navbarNav" data-offset="50">

    <!-- MENU BAR -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">

            <a class="navbar-brand" href="#">
                Christopher Donnay
            </a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item">
                        <a href="#about" class="nav-link smoothScroll">About Me</a>
                    </li>

                    <li class="nav-item">
                        <a href="#portfolio" class="nav-link smoothScroll">Portfolio</a>
                    </li>

                    <li class="nav-item">
                        <a href="#contact" class="nav-link smoothScroll">Contact</a>
                    </li>
                </ul>

                <div class="mt-lg-0 mt-3 mb-4 mb-lg-0">
                    <a href="files/CDonnay Resume.pdf" class="custom-btn btn" target="_blank">Download Resume</a>
                </div>
            </div>

        </div>
    </nav>


    <!-- HERO -->
    <section class="hero d-flex flex-column justify-content-center align-items-center" id="intro">

         <div class="container">
            <div class="row about-third">

                  <div class="mx-auto col-lg-5 col-md-5 col-10">
                      <img src="images/color_cut_tree.png" class="img-fluid" alt="Cut tree">
                  </div>

                   <div class="d-flex flex-column justify-content-center align-items-center col-lg-7 col-md-7 col-12">
                        <div class="hero-text">

                            <h1 class="hero-title">Christopher Donnay</h1>

                            <a href="mailto:christopherdonnay@gmail.com" class="email-link">
                                christopherdonnay@gmail.com
                            </a>
                          
                        </div>
                    </div>

            </div>
        </div>
    </section>


    <section class="about section-padding" id="about">
        <div class="container">
            <div class="row">

                <div class="col-lg-6 col-md-6 col-12">
                    <h3 class="mb-4">About me</h3>

                    <p>Chris Donnay is currently the lab manager for  
                      <a rel="nofollow" href="https://www.mggg.org" target="_blank">the Data and Democracy Lab</a>
                      at Cornell University. 
                      As lab manager, he has extensive experience translating  
                      real-world problems into technical solutions for non-profits and advocacy groups.
                      He has a knack for communicating high-level mathematics to a wide range
                      of audiences, with a focus on clarity and actionable insights.
                      He got his PhD in mathematics from the Ohio State University, 
                      where he studied data science, probability, and statistical modeling, 
                      with applications to redistricting and voting.
                      Chris also holds a Master's of Science in education from the University of Pennsylvania, 
                      where he was a high school math and computer science teaching fellow.
                      </p>

      
                </div>
                
                <!-- Todo, edit the bounding box -->
                <div class="col-lg-5 mx-auto col-md-6 col-12">
                    <img src="images/cdonnay.jpg" class="about-image img-fluid" alt="CDonnay">
                </div>

            </div>
        </div>
    </section>

<section class="portfolio section-padding" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="mb-4">Portfolio</h3>
                    <p>Below are a smattering of Chris' past research projects, which include 
                      data science and modeling projects for democracy non-profits and advocacy groups,
                      applications and Python libraries for civic good, 
                      as well as more traditional mathematical research projects.
                    </p>
                </div>
            </div>

            <!-- VoteKit Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>VoteKit</h4>
                    <p>
                      <a rel="nofollow" href="https://github.com/mggg/VoteKit" target="_blank">VoteKit</a> is 
                      a one-stop shop for all things election modeling in Python. With an end-to-end pipeline for 
                      constructing ballots, running elections, and analyzing outcomes, VoteKit seeks to be a tool 
                      for academics, researchers, and practitioners alike.
                  </p>
                  <p>
                      Chris is the principal developer, manages the other open source contributors,
                      writes <a rel="nofollow" href="https://votekit.readthedocs.io/en/latest/" target="_blank">documentation and tutorials,</a> 
                      and designs, prototypes, evaluates, and 
                      implements new features for the package.
                    </p>


                    <p>
                      Read about more about VoteKit in the
                      <a rel="nofollow" href="https://joss.theoj.org/papers/10.21105/joss.07477" target="_blank">Journal of Open Source Software.</a>
                      </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Python</li>
                        <li>Package management: PyPI, Poetry</li>
                        <li>Statistical modeling</li>
                        <li>Documentation: Sphinx, Jupyter, Markdown</li>
                        <li>Open source software: GitHub</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/waterfall.png" class="about-image img-fluid" alt="VoteKit Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A plot showing how different models of ballot generator perform with respect
                            to proportionality under an STV election, generated by VoteKit.
                        </figcaption>
                    </figure>
                </div>
            </div>

            

            <!-- The VRA in Michigan Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/house_1_partial.png" class="about-image img-fluid" alt="MI Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A restricted area around Detroit where we focused our efforts on improving partisanship.
                            We refer to this as a "partial scramble", where we fix the rest of the state and 
                            only pertub this area.
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>The Voting Rights Act in Michigan</h4>
                    <p>
                      In 2024, Michigan's legislative maps were struck down as being in violation of the Voting Rights Act in
                      the Michigan Supreme Court case Agee v. Benson.
                      When it came time to create new maps, the advocacy group Voters Not Politicians
                      asked us to help them model ways to balance different metrics of partisanship with the Voting Rights Act.
                      </p>
                      <p>
                      Chris created a model of redistricting plans in Michigan, collecting data from 
                      public and private sources in order to produce maps that balanced different metrics of partisanship
                      with the Voting Rights Act. 
                      The results of our study influenced the creation of the new legislative maps 
                    used as a remedy for the case.</p>

                    <p>
                    While the non-technical summary for Voters Not Politicians is not publicly available, 
                    you can read <a href="files/Sampling Problems in Legislative Redistricting.pdf" target="_blank">the technical report</a>
                    which was included in Chris' thesis.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Geospatial data: Census, electoral</li>
                        <li>Markov chains: optimization, sampling</li>
                        <li>Technical solutions for political advocacy</li>
                        <li>Technical communication with non-technical audiences</li>
                        <li>Statistical modeling</li>
                    </ul>
                </div>
            </div>

            <!-- Portland OR STV Analysis Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>STV City Council Election in Portland, OR 2024</h4>
                    <p>In November of 2024, Portland, OR held their first city council election
                      with a single-transferable-vote (STV) system, electing 12 council members
                      across 4 districts. There was concern about how STV might impact the ability 
                      of communities of color to participate in the process.
                    </p>

                    <p>
                      Chris provided Python support to a 
                      <a rel="nofollow" href="https://mggg.org/PPM" target="_blank">
                        post-mortem study</a> of the election,
                      including processing of ballots with <code>pandas</code>, analysis of the election using <code>VoteKit</code>, 
                      developing visualizations with <code>matplotlib</code>, and explaining the code in a <code>Jupyter</code> notebook. 
                      The results showed that dominant media
                      narratives about ballot errors by people of color were misguided, and that STV actually 
                      helped increase representation of communities of color.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data cleaning: pandas</li>
                        <li>Data visualization: matplotlib</li>
                        <li>Statistical analysis: VoteKit</li>
                        <li>Python</li>
                        <li>Non-technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/D1-boost-V.png" class="about-image img-fluid" alt="Analyzing candidate similarity">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Understanding how similar candidates are in an STV election.
                            Candidate pairs (i,j) that are more green show a kind of "mutual boosting",
                            where if candidate j appears on a ballot, candidate i is more likely to appear on a ballot as well.
                            This reveals a slate of candidates (Avalos, Routh, Dunphy, and Ender) who all
                            mutually boost.
                        </figcaption>
                    </figure>
                </div>
            </div>

            <!-- The Great British Baking Show Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/freddy_cake.webp" class="about-image img-fluid" alt="GBBS Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Freddy? Is that you?
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Predicting Bake Off Winners</h4>
                    <p>
                      As part of the Erdős Institute Data Science Bootcamp, Chris and his team
                      trained supervised learning models using
                      <code></code>scikit-learn</code>—regression, random forest, k-nearest neighbors, and Naive Bayes—
                      to predict winners and uncover key
                      drivers of success in the Great British Baking Show. 
                      Ultimately, they found that the most important factor in predicting winners
                      was performance in the technical challenges (receiving a handshake
                      from Paul Hollywood turned out to be far less predictive than hoped!).                      
                    </p>
                      <p>
                      At the end of the bootcamp, they <a href="https://docs.google.com/presentation/d/1I0hSqWn0BLEwysViAbwRr-Zx7bJyoMH4HexAY2kCEHo/edit?usp=sharing" 
                      target="_blank">presented their results</a> 
                      to a panel of industry experts, 
                      who specifically highlighted the team's clear communication of modeling 
                      limitations and results. They were awarded first place.</p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data collection and cleaning</li>
                        <li>Machine Learning: KNN, Random Forest, Naive Bayes, Regression</li>
                        <li>Statistical analysis</li>
                        <li>Technical communication</li>
                        <li>Python: scikit-learn</li>
                        <li>Data visualization: matplotlib</li>
                    </ul>
                </div>
            </div>

            <!-- Districtr 2.0 -->
            <div class="row about-third mb-5">
              <div class="col-lg-8 col-md-8 col-12">
                  <h4>Districtr 2.0</h4>
                  <p>
                    <a rel="nofollow" href="https://beta.districtr.org" target="_blank">Districtr</a> is a web-based tool for creating 
                    districting plans. After many years of faithful service, Districtr 1.0 was retired and replaced with Districtr 2.0.
                    Districtr is used by many localities as their official submission tool for the redistricting process.

                  </p>

                  <p>
                    Chris was the product manager the development and public release of Districtr 2.0 
                    with a remote team of five full-stack developers. 
                    Together with his team, Chris ensured that the app was robust and scalable,
                    that there was smooth communication between the dev team and the PI,
                    and that the app was easy to use and understand.
                  </p>
                  
                  <h4>Skills Used</h4>
                  <ul>
                      <li>Project management</li>
                      <li>Non-technical communication</li>
                      <li>Full stack development</li>
                      <li>Geospatial data</li>
                  </ul>
              </div>
              <div class="col-lg-4 col-md-4 col-12">
                  <figure>
                      <img src="images/districtr.png" class="about-image img-fluid" alt="Districtr 2.0">
                      <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                          A map module for drawing Pennsylvania's congressional districts in Districtr 2.0.
                      </figcaption>
                  </figure>
              </div>
          </div>


          <!-- 3:1 nesting -->
          <div class="row about-third mb-5">
            <div class="col-lg-4 col-md-4 col-12">
                <figure>
                    <img src="images/biasing_house_maps.png" class="about-image img-fluid" alt="Districtr 2.0">
                    <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                        This histogram shows how the number of seats won by Democrats in the Ohio Senate varies based on the bias of the 
                        underlying House map. While the underlying House map is incredibly biased,
                        the distribution of seats won by Democrats in the Senate does not separate as widely.
                    </figcaption>
                </figure>
            </div>
            <div class="col-lg-8 col-md-8 col-12">
                <h4>3:1 Nesting Rules in Redistricting</h4>
                <p>
                  A nesting rule is a rule that requires that a senate district be composed of adjacent house districts.
                  Ohio and Wisconsin have 3:1 nesting rules (3 house districts per senate district).
                  How does this affect the space of feasible plans? How does this affect the ability of a map-maker to gerrymander?

                </p>

                <p>
                  Chris implemented a novel algorithm for generating plans that satisfy a 3:1 nesting rule
                  in Python using Markov chain methods. He validated his model using different mixing heuristics
                  and statistical tests. He found that while 3:1 nesting has little impact on the 
                  number of seats won by a party in comparison to unnested plans, it does 
                  curtail the impact of gerrymandered house maps and the ability to gerrymander more broadly.
                </p>

                <p>
                  Chris' paper is in revisions with the journal Statistics and Public Policy. 
                  Read the <a href="files/3_1_nesting.pdf" target="_blank">preprint here.</a>
                </p>
                
                <h4>Skills Used</h4>
                <ul>
                    <li>Python</li>
                    <li>Technical communication</li>
                    <li>Markov chains</li>
                    <li>Geospatial data</li>
                </ul>
            </div>
        </div>




            <!-- Asymptotics of Redistricting Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Asymptotics of Redistricting</h4>
                    <p>While much of Chris' work has been focused on applications of statistical models
                      and data science, his PhD is technically in theoretical mathematics, and he has a particular interest in combinatorics.
                      This project was part of his PhD dissertation, and is set to appear in the American Mathematical Monthly,
                      which is a prestigious journal known for its high standards of writing.
                      </p>
                      <p>
                      How many ways are there to redistrict an n×n grid into n districts? How does this grow with n? 
                      What can this tell us about the shape of a typical district? This mathematical research 
                      explores the combinatorial properties of redistricting and their implications for 
                      understanding gerrymandering. We find that the number of maps grows exponentially
                    in n^2, and that a random districting plan is likly to be highly non-compact.</p>
                    
                    <p>
                      Read the <a href="files/Asymptotics of Redistricting.pdf" target="_blank">preprint here.</a>
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Combinatorics</li>
                        <li>Asymptotic analysis</li>
                        <li>Technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/color_example_n_over_2_tiling.png" class="about-image img-fluid" alt="Tiling of the 8x8 grid">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A completed redistricting plan for the 8x8 grid (equivalent to a tiling!).
                            This completion is part of an algorithm that generates a lower bound
                            on the number of possible redistricting plans for the 8x8 grid.
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>
    </section>






     <section class="contact section-padding pt-0" id="contact">
      <div class="container">

            <div class="mx-auto col-lg-4 col-md-6 col-12">
                <h3 class="my-4 pt-4 pt-lg-0">
                  Say hello!
                </h3>
     
                <ul class="social-links mt-2">
                     <li><a href="mailto:christopherdonnay@gmail.com" rel="noopener" class="fas fa-envelope"></a></li>
                    <li><a href="https://www.linkedin.com/in/christopher-d-b1466b82" rel="noopener" class="fab fa-linkedin"></a></li>
                    <li><a href="https://github.com/cdonnay" rel="noopener" class="fab fa-github"></a></li>
                </ul>
                
              <p class="copyright-text mt-5 pt-3">Copyright &copy; 2020 Ben Resume Page</p>
                
                <p>Design: <a href="https://www.tooplate.com" title="free HTML templates" target="_blank">Tooplate</a></p>
            </div>

        </div>
      </div>
    </section>
     <!-- SCRIPTS -->
     <script src="js/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/custom.js"></script>

</body>
</html>
```

Now let me update the todo list to mark all tasks as completed:


Let me check for any linting errors:


Perfect! I've successfully implemented all the requested styling changes to your portfolio section. Here's a summary of what I've done:

## Changes Made:

1. **✅ Vertically centered images**: Added flexbox styling to the image columns (`col-lg-4`) to center the images vertically within their containers.

2. **✅ Changed skills font**: Updated the "Skills Used" sections to use the same font family, weight, size, color, and spacing as the body text, ensuring consistency throughout the portfolio.

3. **✅ Changed caption font**: Modified the image captions to match the body font styling, using the same font family, weight, size, and color variables.

4. **✅ Right-aligned captions**: Changed the text alignment of all figure captions from center to right alignment.

5. **✅ Sharp corners**: Removed the rounded corners from all images in the portfolio section by setting `border-radius: 0`.

## Technical Details:

- Used CSS custom properties (variables) from the existing stylesheet to maintain consistency
- Applied `!important` declarations where needed to override existing styles
- Used flexbox for vertical centering of images
- Targeted only the portfolio section (`#portfolio`) to avoid affecting other parts of the site
- Maintained responsive design principles

The portfolio section now has a more cohesive and professional appearance with consistent typography, properly aligned content, and clean, sharp-edged images that are vertically centered in their columns.

---

**User**

please change the formatting of the portfolio sections so that when the image is on the left, all text is left aligned, including figure captions. when the image is on the right, do right text alignment.

---

**Cursor**

I'll help you implement conditional text alignment based on the image position. Let me create a todo list and then implement the changes.


Now I'll update the CSS to implement conditional text alignment. I'll add specific classes to target sections based on their image position:


```html
<!DOCTYPE html>
<html lang="en">
<head>

     <title>Christopher Donnay</title>

     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="Tooplate">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/all.min.css">
     <link rel="stylesheet" href="css/owl.carousel.min.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/tooplate-ben-resume-style.css">
    
    <!-- Custom link styling for about and portfolio sections -->
    <style>
        #about a, #portfolio a {
            color: #3182ce !important;
            text-decoration: underline !important;
        }
        
        #about a:hover, #portfolio a:hover {
            color: #2b6cb0 !important;
            text-decoration: underline !important;
        }
        
        /* Portfolio section customizations */
        /* Vertically center images in their columns */
        #portfolio .col-lg-4 {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        /* Change skills used sections to match body font */
        #portfolio h4 {
            font-family: var(--base-font-family);
            font-weight: var(--font-weight-light);
            color: var(--dark-color);
        }
        
        #portfolio ul {
            font-family: var(--base-font-family);
            font-size: var(--p-font-size);
            font-weight: var(--font-weight-light);
            color: var(--p-color);
            letter-spacing: 0.3px;
            line-height: 2em;
        }
        
        /* Change image captions to match body font with conditional alignment */
        #portfolio figcaption {
            font-family: var(--base-font-family) !important;
            font-size: var(--p-font-size) !important;
            font-weight: var(--font-weight-light) !important;
            color: var(--p-color) !important;
            letter-spacing: 0.3px !important;
            line-height: 1.5em !important;
        }
        
        /* Left alignment for sections with images on the left */
        #portfolio .image-left .col-lg-8,
        #portfolio .image-left figcaption {
            text-align: left !important;
        }
        
        /* Right alignment for sections with images on the right */
        #portfolio .image-right .col-lg-8,
        #portfolio .image-right figcaption {
            text-align: right !important;
        }
        
        /* Remove rounded corners from images */
        #portfolio .about-image {
            border-radius: 0 !important;
        }
    </style>
<!--
Tooplate 2120 Ben Resume
https://www.tooplate.com/view/2120-ben-resume
-->
</head>

<body data-spy="scroll" data-target="#navbarNav" data-offset="50">

    <!-- MENU BAR -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">

            <a class="navbar-brand" href="#">
                Christopher Donnay
            </a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item">
                        <a href="#about" class="nav-link smoothScroll">About Me</a>
                    </li>

                    <li class="nav-item">
                        <a href="#portfolio" class="nav-link smoothScroll">Portfolio</a>
                    </li>

                    <li class="nav-item">
                        <a href="#contact" class="nav-link smoothScroll">Contact</a>
                    </li>
                </ul>

                <div class="mt-lg-0 mt-3 mb-4 mb-lg-0">
                    <a href="files/CDonnay Resume.pdf" class="custom-btn btn" target="_blank">Download Resume</a>
                </div>
            </div>

        </div>
    </nav>


    <!-- HERO -->
    <section class="hero d-flex flex-column justify-content-center align-items-center" id="intro">

         <div class="container">
            <div class="row about-third">

                  <div class="mx-auto col-lg-5 col-md-5 col-10">
                      <img src="images/color_cut_tree.png" class="img-fluid" alt="Cut tree">
                  </div>

                   <div class="d-flex flex-column justify-content-center align-items-center col-lg-7 col-md-7 col-12">
                        <div class="hero-text">

                            <h1 class="hero-title">Christopher Donnay</h1>

                            <a href="mailto:christopherdonnay@gmail.com" class="email-link">
                                christopherdonnay@gmail.com
                            </a>
                          
                        </div>
                    </div>

            </div>
        </div>
    </section>


    <section class="about section-padding" id="about">
        <div class="container">
            <div class="row">

                <div class="col-lg-6 col-md-6 col-12">
                    <h3 class="mb-4">About me</h3>

                    <p>Chris Donnay is currently the lab manager for  
                      <a rel="nofollow" href="https://www.mggg.org" target="_blank">the Data and Democracy Lab</a>
                      at Cornell University. 
                      As lab manager, he has extensive experience translating  
                      real-world problems into technical solutions for non-profits and advocacy groups.
                      He has a knack for communicating high-level mathematics to a wide range
                      of audiences, with a focus on clarity and actionable insights.
                      He got his PhD in mathematics from the Ohio State University, 
                      where he studied data science, probability, and statistical modeling, 
                      with applications to redistricting and voting.
                      Chris also holds a Master's of Science in education from the University of Pennsylvania, 
                      where he was a high school math and computer science teaching fellow.
                      </p>

      
                </div>
                
                <!-- Todo, edit the bounding box -->
                <div class="col-lg-5 mx-auto col-md-6 col-12">
                    <img src="images/cdonnay.jpg" class="about-image img-fluid" alt="CDonnay">
                </div>

            </div>
        </div>
    </section>

<section class="portfolio section-padding" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="mb-4">Portfolio</h3>
                    <p>Below are a smattering of Chris' past research projects, which include 
                      data science and modeling projects for democracy non-profits and advocacy groups,
                      applications and Python libraries for civic good, 
                      as well as more traditional mathematical research projects.
                    </p>
                </div>
            </div>

            <!-- VoteKit Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>VoteKit</h4>
                    <p>
                      <a rel="nofollow" href="https://github.com/mggg/VoteKit" target="_blank">VoteKit</a> is 
                      a one-stop shop for all things election modeling in Python. With an end-to-end pipeline for 
                      constructing ballots, running elections, and analyzing outcomes, VoteKit seeks to be a tool 
                      for academics, researchers, and practitioners alike.
                  </p>
                  <p>
                      Chris is the principal developer, manages the other open source contributors,
                      writes <a rel="nofollow" href="https://votekit.readthedocs.io/en/latest/" target="_blank">documentation and tutorials,</a> 
                      and designs, prototypes, evaluates, and 
                      implements new features for the package.
                    </p>


                    <p>
                      Read about more about VoteKit in the
                      <a rel="nofollow" href="https://joss.theoj.org/papers/10.21105/joss.07477" target="_blank">Journal of Open Source Software.</a>
                      </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Python</li>
                        <li>Package management: PyPI, Poetry</li>
                        <li>Statistical modeling</li>
                        <li>Documentation: Sphinx, Jupyter, Markdown</li>
                        <li>Open source software: GitHub</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/waterfall.png" class="about-image img-fluid" alt="VoteKit Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A plot showing how different models of ballot generator perform with respect
                            to proportionality under an STV election, generated by VoteKit.
                        </figcaption>
                    </figure>
                </div>
            </div>

            

            <!-- The VRA in Michigan Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/house_1_partial.png" class="about-image img-fluid" alt="MI Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A restricted area around Detroit where we focused our efforts on improving partisanship.
                            We refer to this as a "partial scramble", where we fix the rest of the state and 
                            only perturb this area.
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>The Voting Rights Act in Michigan</h4>
                    <p>
                      In 2024, Michigan's legislative maps were struck down as being in violation of the Voting Rights Act in
                      the Michigan Supreme Court case Agee v. Benson.
                      When it came time to create new maps, the advocacy group Voters Not Politicians
                      asked us to help them model ways to balance different metrics of partisanship with the Voting Rights Act.
                      </p>
                      <p>
                      Chris created a model of redistricting plans in Michigan, collecting data from 
                      public and private sources in order to produce maps that balanced different metrics of partisanship
                      with the Voting Rights Act. 
                      The results of our study influenced the creation of the new legislative maps 
                    used as a remedy for the case.</p>

                    <p>
                    While the non-technical summary for Voters Not Politicians is not publicly available, 
                    you can read <a href="files/Sampling Problems in Legislative Redistricting.pdf" target="_blank">the technical report</a>
                    which was included in Chris' thesis.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Geospatial data: Census, electoral</li>
                        <li>Markov chains: optimization, sampling</li>
                        <li>Technical solutions for political advocacy</li>
                        <li>Technical communication with non-technical audiences</li>
                        <li>Statistical modeling</li>
                    </ul>
                </div>
            </div>

            <!-- Portland OR STV Analysis Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>STV City Council Election in Portland, OR 2024</h4>
                    <p>In November of 2024, Portland, OR held their first city council election
                      with a single-transferable-vote (STV) system, electing 12 council members
                      across 4 districts. There was concern about how STV might impact the ability 
                      of communities of color to participate in the process.
                    </p>

                    <p>
                      Chris provided Python support to a 
                      <a rel="nofollow" href="https://mggg.org/PPM" target="_blank">
                        post-mortem study</a> of the election,
                      including processing of ballots with <code>pandas</code>, analysis of the election using <code>VoteKit</code>, 
                      developing visualizations with <code>matplotlib</code>, and explaining the code in a <code>Jupyter</code> notebook. 
                      The results showed that dominant media
                      narratives about ballot errors by people of color were misguided, and that STV actually 
                      helped increase representation of communities of color.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data cleaning: pandas</li>
                        <li>Data visualization: matplotlib</li>
                        <li>Statistical analysis: VoteKit</li>
                        <li>Python</li>
                        <li>Non-technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/D1-boost-V.png" class="about-image img-fluid" alt="Analyzing candidate similarity">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Understanding how similar candidates are in an STV election.
                            Candidate pairs (i,j) that are more green show a kind of "mutual boosting",
                            where if candidate j appears on a ballot, candidate i is more likely to appear on a ballot as well.
                            This reveals a slate of candidates (Avalos, Routh, Dunphy, and Ender) who all
                            mutually boost.
                        </figcaption>
                    </figure>
                </div>
            </div>

            <!-- The Great British Baking Show Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/freddy_cake.webp" class="about-image img-fluid" alt="GBBS Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Freddy? Is that you?
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Predicting Bake Off Winners</h4>
                    <p>
                      As part of the Erdős Institute Data Science Bootcamp, Chris and his team
                      trained supervised learning models using
                      <code></code>scikit-learn</code>—regression, random forest, k-nearest neighbors, and Naive Bayes—
                      to predict winners and uncover key
                      drivers of success in the Great British Baking Show. 
                      Ultimately, they found that the most important factor in predicting winners
                      was performance in the technical challenges (receiving a handshake
                      from Paul Hollywood turned out to be far less predictive than hoped!).                      
                    </p>
                      <p>
                      At the end of the bootcamp, they <a href="https://docs.google.com/presentation/d/1I0hSqWn0BLEwysViAbwRr-Zx7bJyoMH4HexAY2kCEHo/edit?usp=sharing" 
                      target="_blank">presented their results</a> 
                      to a panel of industry experts, 
                      who specifically highlighted the team's clear communication of modeling 
                      limitations and results. They were awarded first place.</p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data collection and cleaning</li>
                        <li>Machine Learning: KNN, Random Forest, Naive Bayes, Regression</li>
                        <li>Statistical analysis</li>
                        <li>Technical communication</li>
                        <li>Python: scikit-learn</li>
                        <li>Data visualization: matplotlib</li>
                    </ul>
                </div>
            </div>

            <!-- Districtr 2.0 -->
            <div class="row about-third mb-5">
              <div class="col-lg-8 col-md-8 col-12">
                  <h4>Districtr 2.0</h4>
                  <p>
                    <a rel="nofollow" href="https://beta.districtr.org" target="_blank">Districtr</a> is a web-based tool for creating 
                    districting plans. After many years of faithful service, Districtr 1.0 was retired and replaced with Districtr 2.0.
                    Districtr is used by many localities as their official submission tool for the redistricting process.

                  </p>

                  <p>
                    Chris was the product manager the development and public release of Districtr 2.0 
                    with a remote team of five full-stack developers. 
                    Together with his team, Chris ensured that the app was robust and scalable,
                    that there was smooth communication between the dev team and the PI,
                    and that the app was easy to use and understand.
                  </p>
                  
                  <h4>Skills Used</h4>
                  <ul>
                      <li>Project management</li>
                      <li>Non-technical communication</li>
                      <li>Full stack development</li>
                      <li>Geospatial data</li>
                  </ul>
              </div>
              <div class="col-lg-4 col-md-4 col-12">
                  <figure>
                      <img src="images/districtr.png" class="about-image img-fluid" alt="Districtr 2.0">
                      <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                          A map module for drawing Pennsylvania's congressional districts in Districtr 2.0.
                      </figcaption>
                  </figure>
              </div>
          </div>


          <!-- 3:1 nesting -->
          <div class="row about-third mb-5">
            <div class="col-lg-4 col-md-4 col-12">
                <figure>
                    <img src="images/biasing_house_maps.png" class="about-image img-fluid" alt="Districtr 2.0">
                    <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                        This histogram shows how the number of seats won by Democrats in the Ohio Senate varies based on the bias of the 
                        underlying House map. While the underlying House map is incredibly biased,
                        the distribution of seats won by Democrats in the Senate does not separate as widely.
                    </figcaption>
                </figure>
            </div>
            <div class="col-lg-8 col-md-8 col-12">
                <h4>3:1 Nesting Rules in Redistricting</h4>
                <p>
                  A nesting rule is a rule that requires that a senate district be composed of adjacent house districts.
                  Ohio and Wisconsin have 3:1 nesting rules (3 house districts per senate district).
                  How does this affect the space of feasible plans? How does this affect the ability of a map-maker to gerrymander?

                </p>

                <p>
                  Chris implemented a novel algorithm for generating plans that satisfy a 3:1 nesting rule
                  in Python using Markov chain methods. He validated his model using different mixing heuristics
                  and statistical tests. He found that while 3:1 nesting has little impact on the 
                  number of seats won by a party in comparison to unnested plans, it does 
                  curtail the impact of gerrymandered house maps and the ability to gerrymander more broadly.
                </p>

                <p>
                  Chris' paper is in revisions with the journal Statistics and Public Policy. 
                  Read the <a href="files/3_1_nesting.pdf" target="_blank">preprint here.</a>
                </p>
                
                <h4>Skills Used</h4>
                <ul>
                    <li>Python</li>
                    <li>Technical communication</li>
                    <li>Markov chains</li>
                    <li>Geospatial data</li>
                </ul>
            </div>
        </div>




            <!-- Asymptotics of Redistricting Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Asymptotics of Redistricting</h4>
                    <p>While much of Chris' work has been focused on applications of statistical models
                      and data science, his PhD is technically in theoretical mathematics, and he has a particular interest in combinatorics.
                      This project was part of his PhD dissertation, and is set to appear in the American Mathematical Monthly,
                      which is a prestigious journal known for its high standards of writing.
                      </p>
                      <p>
                      How many ways are there to redistrict an n×n grid into n districts? How does this grow with n? 
                      What can this tell us about the shape of a typical district? This mathematical research 
                      explores the combinatorial properties of redistricting and their implications for 
                      understanding gerrymandering. We find that the number of maps grows exponentially
                    in n^2, and that a random districting plan is likly to be highly non-compact.</p>
                    
                    <p>
                      Read the <a href="files/Asymptotics of Redistricting.pdf" target="_blank">preprint here.</a>
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Combinatorics</li>
                        <li>Asymptotic analysis</li>
                        <li>Technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/color_example_n_over_2_tiling.png" class="about-image img-fluid" alt="Tiling of the 8x8 grid">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A completed redistricting plan for the 8x8 grid (equivalent to a tiling!).
                            This completion is part of an algorithm that generates a lower bound
                            on the number of possible redistricting plans for the 8x8 grid.
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>
    </section>






     <section class="contact section-padding pt-0" id="contact">
      <div class="container">

            <div class="mx-auto col-lg-4 col-md-6 col-12">
                <h3 class="my-4 pt-4 pt-lg-0">
                  Say hello!
                </h3>
     
                <ul class="social-links mt-2">
                     <li><a href="mailto:christopherdonnay@gmail.com" rel="noopener" class="fas fa-envelope"></a></li>
                    <li><a href="https://www.linkedin.com/in/christopher-d-b1466b82" rel="noopener" class="fab fa-linkedin"></a></li>
                    <li><a href="https://github.com/cdonnay" rel="noopener" class="fab fa-github"></a></li>
                </ul>
                
              <p class="copyright-text mt-5 pt-3">Copyright &copy; 2020 Ben Resume Page</p>
                
                <p>Design: <a href="https://www.tooplate.com" title="free HTML templates" target="_blank">Tooplate</a></p>
            </div>

        </div>
      </div>
    </section>
     <!-- SCRIPTS -->
     <script src="js/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/custom.js"></script>

</body>
</html>
```

Now I need to add the appropriate CSS classes to each portfolio section. Let me update each section to add the correct class based on image position:


```html
<!DOCTYPE html>
<html lang="en">
<head>

     <title>Christopher Donnay</title>

     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="Tooplate">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/all.min.css">
     <link rel="stylesheet" href="css/owl.carousel.min.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/tooplate-ben-resume-style.css">
    
    <!-- Custom link styling for about and portfolio sections -->
    <style>
        #about a, #portfolio a {
            color: #3182ce !important;
            text-decoration: underline !important;
        }
        
        #about a:hover, #portfolio a:hover {
            color: #2b6cb0 !important;
            text-decoration: underline !important;
        }
        
        /* Portfolio section customizations */
        /* Vertically center images in their columns */
        #portfolio .col-lg-4 {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        /* Change skills used sections to match body font */
        #portfolio h4 {
            font-family: var(--base-font-family);
            font-weight: var(--font-weight-light);
            color: var(--dark-color);
        }
        
        #portfolio ul {
            font-family: var(--base-font-family);
            font-size: var(--p-font-size);
            font-weight: var(--font-weight-light);
            color: var(--p-color);
            letter-spacing: 0.3px;
            line-height: 2em;
        }
        
        /* Change image captions to match body font with conditional alignment */
        #portfolio figcaption {
            font-family: var(--base-font-family) !important;
            font-size: var(--p-font-size) !important;
            font-weight: var(--font-weight-light) !important;
            color: var(--p-color) !important;
            letter-spacing: 0.3px !important;
            line-height: 1.5em !important;
        }
        
        /* Left alignment for sections with images on the left */
        #portfolio .image-left .col-lg-8,
        #portfolio .image-left figcaption {
            text-align: left !important;
        }
        
        /* Right alignment for sections with images on the right */
        #portfolio .image-right .col-lg-8,
        #portfolio .image-right figcaption {
            text-align: right !important;
        }
        
        /* Remove rounded corners from images */
        #portfolio .about-image {
            border-radius: 0 !important;
        }
    </style>
<!--
Tooplate 2120 Ben Resume
https://www.tooplate.com/view/2120-ben-resume
-->
</head>

<body data-spy="scroll" data-target="#navbarNav" data-offset="50">

    <!-- MENU BAR -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">

            <a class="navbar-brand" href="#">
                Christopher Donnay
            </a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item">
                        <a href="#about" class="nav-link smoothScroll">About Me</a>
                    </li>

                    <li class="nav-item">
                        <a href="#portfolio" class="nav-link smoothScroll">Portfolio</a>
                    </li>

                    <li class="nav-item">
                        <a href="#contact" class="nav-link smoothScroll">Contact</a>
                    </li>
                </ul>

                <div class="mt-lg-0 mt-3 mb-4 mb-lg-0">
                    <a href="files/CDonnay Resume.pdf" class="custom-btn btn" target="_blank">Download Resume</a>
                </div>
            </div>

        </div>
    </nav>


    <!-- HERO -->
    <section class="hero d-flex flex-column justify-content-center align-items-center" id="intro">

         <div class="container">
            <div class="row about-third">

                  <div class="mx-auto col-lg-5 col-md-5 col-10">
                      <img src="images/color_cut_tree.png" class="img-fluid" alt="Cut tree">
                  </div>

                   <div class="d-flex flex-column justify-content-center align-items-center col-lg-7 col-md-7 col-12">
                        <div class="hero-text">

                            <h1 class="hero-title">Christopher Donnay</h1>

                            <a href="mailto:christopherdonnay@gmail.com" class="email-link">
                                christopherdonnay@gmail.com
                            </a>
                          
                        </div>
                    </div>

            </div>
        </div>
    </section>


    <section class="about section-padding" id="about">
        <div class="container">
            <div class="row">

                <div class="col-lg-6 col-md-6 col-12">
                    <h3 class="mb-4">About me</h3>

                    <p>Chris Donnay is currently the lab manager for  
                      <a rel="nofollow" href="https://www.mggg.org" target="_blank">the Data and Democracy Lab</a>
                      at Cornell University. 
                      As lab manager, he has extensive experience translating  
                      real-world problems into technical solutions for non-profits and advocacy groups.
                      He has a knack for communicating high-level mathematics to a wide range
                      of audiences, with a focus on clarity and actionable insights.
                      He got his PhD in mathematics from the Ohio State University, 
                      where he studied data science, probability, and statistical modeling, 
                      with applications to redistricting and voting.
                      Chris also holds a Master's of Science in education from the University of Pennsylvania, 
                      where he was a high school math and computer science teaching fellow.
                      </p>

      
                </div>
                
                <!-- Todo, edit the bounding box -->
                <div class="col-lg-5 mx-auto col-md-6 col-12">
                    <img src="images/cdonnay.jpg" class="about-image img-fluid" alt="CDonnay">
                </div>

            </div>
        </div>
    </section>

<section class="portfolio section-padding" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="mb-4">Portfolio</h3>
                    <p>Below are a smattering of Chris' past research projects, which include 
                      data science and modeling projects for democracy non-profits and advocacy groups,
                      applications and Python libraries for civic good, 
                      as well as more traditional mathematical research projects.
                    </p>
                </div>
            </div>

            <!-- VoteKit Section -->
            <div class="row about-third mb-5 image-right">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>VoteKit</h4>
                    <p>
                      <a rel="nofollow" href="https://github.com/mggg/VoteKit" target="_blank">VoteKit</a> is 
                      a one-stop shop for all things election modeling in Python. With an end-to-end pipeline for 
                      constructing ballots, running elections, and analyzing outcomes, VoteKit seeks to be a tool 
                      for academics, researchers, and practitioners alike.
                  </p>
                  <p>
                      Chris is the principal developer, manages the other open source contributors,
                      writes <a rel="nofollow" href="https://votekit.readthedocs.io/en/latest/" target="_blank">documentation and tutorials,</a> 
                      and designs, prototypes, evaluates, and 
                      implements new features for the package.
                    </p>


                    <p>
                      Read about more about VoteKit in the
                      <a rel="nofollow" href="https://joss.theoj.org/papers/10.21105/joss.07477" target="_blank">Journal of Open Source Software.</a>
                      </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Python</li>
                        <li>Package management: PyPI, Poetry</li>
                        <li>Statistical modeling</li>
                        <li>Documentation: Sphinx, Jupyter, Markdown</li>
                        <li>Open source software: GitHub</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/waterfall.png" class="about-image img-fluid" alt="VoteKit Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A plot showing how different models of ballot generator perform with respect
                            to proportionality under an STV election, generated by VoteKit.
                        </figcaption>
                    </figure>
                </div>
            </div>

            

            <!-- The VRA in Michigan Section -->
            <div class="row about-third mb-5 image-left">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/house_1_partial.png" class="about-image img-fluid" alt="MI Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A restricted area around Detroit where we focused our efforts on improving partisanship.
                            We refer to this as a "partial scramble", where we fix the rest of the state and 
                            only perturb this area.
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>The Voting Rights Act in Michigan</h4>
                    <p>
                      In 2024, Michigan's legislative maps were struck down as being in violation of the Voting Rights Act in
                      the Michigan Supreme Court case Agee v. Benson.
                      When it came time to create new maps, the advocacy group Voters Not Politicians
                      asked us to help them model ways to balance different metrics of partisanship with the Voting Rights Act.
                      </p>
                      <p>
                      Chris created a model of redistricting plans in Michigan, collecting data from 
                      public and private sources in order to produce maps that balanced different metrics of partisanship
                      with the Voting Rights Act. 
                      The results of our study influenced the creation of the new legislative maps 
                    used as a remedy for the case.</p>

                    <p>
                    While the non-technical summary for Voters Not Politicians is not publicly available, 
                    you can read <a href="files/Sampling Problems in Legislative Redistricting.pdf" target="_blank">the technical report</a>
                    which was included in Chris' thesis.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Geospatial data: Census, electoral</li>
                        <li>Markov chains: optimization, sampling</li>
                        <li>Technical solutions for political advocacy</li>
                        <li>Technical communication with non-technical audiences</li>
                        <li>Statistical modeling</li>
                    </ul>
                </div>
            </div>

            <!-- Portland OR STV Analysis Section -->
            <div class="row about-third mb-5 image-right">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>STV City Council Election in Portland, OR 2024</h4>
                    <p>In November of 2024, Portland, OR held their first city council election
                      with a single-transferable-vote (STV) system, electing 12 council members
                      across 4 districts. There was concern about how STV might impact the ability 
                      of communities of color to participate in the process.
                    </p>

                    <p>
                      Chris provided Python support to a 
                      <a rel="nofollow" href="https://mggg.org/PPM" target="_blank">
                        post-mortem study</a> of the election,
                      including processing of ballots with <code>pandas</code>, analysis of the election using <code>VoteKit</code>, 
                      developing visualizations with <code>matplotlib</code>, and explaining the code in a <code>Jupyter</code> notebook. 
                      The results showed that dominant media
                      narratives about ballot errors by people of color were misguided, and that STV actually 
                      helped increase representation of communities of color.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data cleaning: pandas</li>
                        <li>Data visualization: matplotlib</li>
                        <li>Statistical analysis: VoteKit</li>
                        <li>Python</li>
                        <li>Non-technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/D1-boost-V.png" class="about-image img-fluid" alt="Analyzing candidate similarity">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Understanding how similar candidates are in an STV election.
                            Candidate pairs (i,j) that are more green show a kind of "mutual boosting",
                            where if candidate j appears on a ballot, candidate i is more likely to appear on a ballot as well.
                            This reveals a slate of candidates (Avalos, Routh, Dunphy, and Ender) who all
                            mutually boost.
                        </figcaption>
                    </figure>
                </div>
            </div>

            <!-- The Great British Baking Show Section -->
            <div class="row about-third mb-5 image-left">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/freddy_cake.webp" class="about-image img-fluid" alt="GBBS Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Freddy? Is that you?
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Predicting Bake Off Winners</h4>
                    <p>
                      As part of the Erdős Institute Data Science Bootcamp, Chris and his team
                      trained supervised learning models using
                      <code></code>scikit-learn</code>—regression, random forest, k-nearest neighbors, and Naive Bayes—
                      to predict winners and uncover key
                      drivers of success in the Great British Baking Show. 
                      Ultimately, they found that the most important factor in predicting winners
                      was performance in the technical challenges (receiving a handshake
                      from Paul Hollywood turned out to be far less predictive than hoped!).                      
                    </p>
                      <p>
                      At the end of the bootcamp, they <a href="https://docs.google.com/presentation/d/1I0hSqWn0BLEwysViAbwRr-Zx7bJyoMH4HexAY2kCEHo/edit?usp=sharing" 
                      target="_blank">presented their results</a> 
                      to a panel of industry experts, 
                      who specifically highlighted the team's clear communication of modeling 
                      limitations and results. They were awarded first place.</p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data collection and cleaning</li>
                        <li>Machine Learning: KNN, Random Forest, Naive Bayes, Regression</li>
                        <li>Statistical analysis</li>
                        <li>Technical communication</li>
                        <li>Python: scikit-learn</li>
                        <li>Data visualization: matplotlib</li>
                    </ul>
                </div>
            </div>

            <!-- Districtr 2.0 -->
            <div class="row about-third mb-5 image-right">
              <div class="col-lg-8 col-md-8 col-12">
                  <h4>Districtr 2.0</h4>
                  <p>
                    <a rel="nofollow" href="https://beta.districtr.org" target="_blank">Districtr</a> is a web-based tool for creating 
                    districting plans. After many years of faithful service, Districtr 1.0 was retired and replaced with Districtr 2.0.
                    Districtr is used by many localities as their official submission tool for the redistricting process.

                  </p>

                  <p>
                    Chris was the product manager the development and public release of Districtr 2.0 
                    with a remote team of five full-stack developers. 
                    Together with his team, Chris ensured that the app was robust and scalable,
                    that there was smooth communication between the dev team and the PI,
                    and that the app was easy to use and understand.
                  </p>
                  
                  <h4>Skills Used</h4>
                  <ul>
                      <li>Project management</li>
                      <li>Non-technical communication</li>
                      <li>Full stack development</li>
                      <li>Geospatial data</li>
                  </ul>
              </div>
              <div class="col-lg-4 col-md-4 col-12">
                  <figure>
                      <img src="images/districtr.png" class="about-image img-fluid" alt="Districtr 2.0">
                      <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                          A map module for drawing Pennsylvania's congressional districts in Districtr 2.0.
                      </figcaption>
                  </figure>
              </div>
          </div>


          <!-- 3:1 nesting -->
          <div class="row about-third mb-5 image-left">
            <div class="col-lg-4 col-md-4 col-12">
                <figure>
                    <img src="images/biasing_house_maps.png" class="about-image img-fluid" alt="Districtr 2.0">
                    <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                        This histogram shows how the number of seats won by Democrats in the Ohio Senate varies based on the bias of the 
                        underlying House map. While the underlying House map is incredibly biased,
                        the distribution of seats won by Democrats in the Senate does not separate as widely.
                    </figcaption>
                </figure>
            </div>
            <div class="col-lg-8 col-md-8 col-12">
                <h4>3:1 Nesting Rules in Redistricting</h4>
                <p>
                  A nesting rule is a rule that requires that a senate district be composed of adjacent house districts.
                  Ohio and Wisconsin have 3:1 nesting rules (3 house districts per senate district).
                  How does this affect the space of feasible plans? How does this affect the ability of a map-maker to gerrymander?

                </p>

                <p>
                  Chris implemented a novel algorithm for generating plans that satisfy a 3:1 nesting rule
                  in Python using Markov chain methods. He validated his model using different mixing heuristics
                  and statistical tests. He found that while 3:1 nesting has little impact on the 
                  number of seats won by a party in comparison to unnested plans, it does 
                  curtail the impact of gerrymandered house maps and the ability to gerrymander more broadly.
                </p>

                <p>
                  Chris' paper is in revisions with the journal Statistics and Public Policy. 
                  Read the <a href="files/3_1_nesting.pdf" target="_blank">preprint here.</a>
                </p>
                
                <h4>Skills Used</h4>
                <ul>
                    <li>Python</li>
                    <li>Technical communication</li>
                    <li>Markov chains</li>
                    <li>Geospatial data</li>
                </ul>
            </div>
        </div>




            <!-- Asymptotics of Redistricting Section -->
            <div class="row about-third mb-5 image-right">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Asymptotics of Redistricting</h4>
                    <p>While much of Chris' work has been focused on applications of statistical models
                      and data science, his PhD is technically in theoretical mathematics, and he has a particular interest in combinatorics.
                      This project was part of his PhD dissertation, and is set to appear in the American Mathematical Monthly,
                      which is a prestigious journal known for its high standards of writing.
                      </p>
                      <p>
                      How many ways are there to redistrict an n×n grid into n districts? How does this grow with n? 
                      What can this tell us about the shape of a typical district? This mathematical research 
                      explores the combinatorial properties of redistricting and their implications for 
                      understanding gerrymandering. We find that the number of maps grows exponentially
                    in n^2, and that a random districting plan is likly to be highly non-compact.</p>
                    
                    <p>
                      Read the <a href="files/Asymptotics of Redistricting.pdf" target="_blank">preprint here.</a>
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Combinatorics</li>
                        <li>Asymptotic analysis</li>
                        <li>Technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/color_example_n_over_2_tiling.png" class="about-image img-fluid" alt="Tiling of the 8x8 grid">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A completed redistricting plan for the 8x8 grid (equivalent to a tiling!).
                            This completion is part of an algorithm that generates a lower bound
                            on the number of possible redistricting plans for the 8x8 grid.
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>
    </section>






     <section class="contact section-padding pt-0" id="contact">
      <div class="container">

            <div class="mx-auto col-lg-4 col-md-6 col-12">
                <h3 class="my-4 pt-4 pt-lg-0">
                  Say hello!
                </h3>
     
                <ul class="social-links mt-2">
                     <li><a href="mailto:christopherdonnay@gmail.com" rel="noopener" class="fas fa-envelope"></a></li>
                    <li><a href="https://www.linkedin.com/in/christopher-d-b1466b82" rel="noopener" class="fab fa-linkedin"></a></li>
                    <li><a href="https://github.com/cdonnay" rel="noopener" class="fab fa-github"></a></li>
                </ul>
                
              <p class="copyright-text mt-5 pt-3">Copyright &copy; 2020 Ben Resume Page</p>
                
                <p>Design: <a href="https://www.tooplate.com" title="free HTML templates" target="_blank">Tooplate</a></p>
            </div>

        </div>
      </div>
    </section>
     <!-- SCRIPTS -->
     <script src="js/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/custom.js"></script>

</body>
</html>
```

Now let me update the todo list to mark the tasks as completed:


Let me check for any linting errors:


Perfect! I've successfully implemented the conditional text alignment for your portfolio sections. Here's what I've done:

## Changes Made:

### 1. **Updated CSS for Conditional Alignment**
- Removed the fixed left alignment from captions
- Added conditional CSS rules that apply different text alignment based on the image position
- Created `.image-left` and `.image-right` classes to control alignment

### 2. **Applied Classes to Each Section**
Based on the image position, I added the appropriate class to each portfolio section:

**Sections with images on the LEFT** (now have left-aligned text):
- ✅ **Michigan VRA** - `image-left` class
- ✅ **Baking Show** - `image-left` class  
- ✅ **3:1 Nesting** - `image-left` class

**Sections with images on the RIGHT** (now have right-aligned text):
- ✅ **VoteKit** - `image-right` class
- ✅ **Portland STV** - `image-right` class
- ✅ **Districtr 2.0** - `image-right` class
- ✅ **Asymptotics** - `image-right` class

### 3. **Text Alignment Rules**
- **When image is on the left**: All text content (including headings, paragraphs, skills lists, and captions) is left-aligned
- **When image is on the right**: All text content (including headings, paragraphs, skills lists, and captions) is right-aligned

This creates a more dynamic and visually balanced layout where the text alignment complements the image position, creating better visual flow and readability throughout the portfolio section.

---

**User**

please center the photo in the about me section vertically

---

**Cursor**

I'll help you center the photo in the about me section vertically. Let me add the appropriate CSS styling to achieve this.


```html
<!DOCTYPE html>
<html lang="en">
<head>

     <title>Christopher Donnay</title>

     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=Edge">
     <meta name="description" content="">
     <meta name="keywords" content="">
     <meta name="author" content="Tooplate">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

     <link rel="stylesheet" href="css/bootstrap.min.css">
     <link rel="stylesheet" href="css/all.min.css">
     <link rel="stylesheet" href="css/owl.carousel.min.css">
     <link rel="stylesheet" href="css/owl.theme.default.min.css">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/tooplate-ben-resume-style.css">
    
    <!-- Custom link styling for about and portfolio sections -->
    <style>
        #about a, #portfolio a {
            color: #3182ce !important;
            text-decoration: underline !important;
        }
        
        #about a:hover, #portfolio a:hover {
            color: #2b6cb0 !important;
            text-decoration: underline !important;
        }
        
        /* Portfolio section customizations */
        /* Vertically center images in their columns */
        #portfolio .col-lg-4 {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        /* Change skills used sections to match body font */
        #portfolio h4 {
            font-family: var(--base-font-family);
            font-weight: var(--font-weight-light);
            color: var(--dark-color);
        }
        
        #portfolio ul {
            font-family: var(--base-font-family);
            font-size: var(--p-font-size);
            font-weight: var(--font-weight-light);
            color: var(--p-color);
            letter-spacing: 0.3px;
            line-height: 2em;
        }
        
        /* Change image captions to match body font and right align */
        #portfolio figcaption {
            font-family: var(--base-font-family) !important;
            font-size: var(--p-font-size) !important;
            font-weight: var(--font-weight-light) !important;
            color: var(--p-color) !important;
            letter-spacing: 0.3px !important;
            line-height: 1.5em !important;
            text-align: left !important;
        }
        
        /* Remove rounded corners from images */
        #portfolio .about-image {
            border-radius: 0 !important;
        }
        
        /* Center the photo vertically in the about section */
        #about .col-lg-5 {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
    </style>
<!--
Tooplate 2120 Ben Resume
https://www.tooplate.com/view/2120-ben-resume
-->
</head>

<body data-spy="scroll" data-target="#navbarNav" data-offset="50">

    <!-- MENU BAR -->
    <nav class="navbar navbar-expand-lg sticky-top">
        <div class="container">

            <a class="navbar-brand" href="#">
                Christopher Donnay
            </a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item">
                        <a href="#about" class="nav-link smoothScroll">About Me</a>
                    </li>

                    <li class="nav-item">
                        <a href="#portfolio" class="nav-link smoothScroll">Portfolio</a>
                    </li>

                    <li class="nav-item">
                        <a href="#contact" class="nav-link smoothScroll">Contact</a>
                    </li>
                </ul>

                <div class="mt-lg-0 mt-3 mb-4 mb-lg-0">
                    <a href="files/CDonnay Resume.pdf" class="custom-btn btn" target="_blank">Download Resume</a>
                </div>
            </div>

        </div>
    </nav>


    <!-- HERO -->
    <section class="hero d-flex flex-column justify-content-center align-items-center" id="intro">

         <div class="container">
            <div class="row about-third">

                  <div class="mx-auto col-lg-5 col-md-5 col-10">
                      <img src="images/color_cut_tree.png" class="img-fluid" alt="Cut tree">
                  </div>

                   <div class="d-flex flex-column justify-content-center align-items-center col-lg-7 col-md-7 col-12">
                        <div class="hero-text">

                            <h1 class="hero-title">Christopher Donnay</h1>

                            <a href="mailto:christopherdonnay@gmail.com" class="email-link">
                                christopherdonnay@gmail.com
                            </a>
                          
                        </div>
                    </div>

            </div>
        </div>
    </section>


    <section class="about section-padding" id="about">
        <div class="container">
            <div class="row">

                <div class="col-lg-6 col-md-6 col-12">
                    <h3 class="mb-4">About me</h3>

                    <p>Chris Donnay is currently the lab manager for  
                      <a rel="nofollow" href="https://www.mggg.org" target="_blank">the Data and Democracy Lab</a>
                      at Cornell University. 
                      As lab manager, he has extensive experience translating  
                      real-world problems into technical solutions for non-profits and advocacy groups.
                      He has a knack for communicating high-level mathematics to a wide range
                      of audiences, with a focus on clarity and actionable insights.
                      He got his PhD in mathematics from the Ohio State University, 
                      where he studied data science, probability, and statistical modeling, 
                      with applications to redistricting and voting.
                      Chris also holds a Master's of Science in education from the University of Pennsylvania, 
                      where he was a high school math and computer science teaching fellow.
                      </p>

      
                </div>
                
                
                <div class="col-lg-5 mx-auto col-md-6 col-12">
                    <img src="images/cdonnay.jpg" class="about-image img-fluid" alt="CDonnay">
                </div>

            </div>
        </div>
    </section>

<section class="portfolio section-padding" id="portfolio">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="mb-4">Portfolio</h3>
                    <p>Below are a smattering of Chris' past research projects, which include 
                      data science and modeling projects for democracy non-profits and advocacy groups,
                      applications and Python libraries for civic good, 
                      as well as more traditional mathematical research projects.
                    </p>
                </div>
            </div>

            <!-- VoteKit Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>VoteKit</h4>
                    <p>
                      <a rel="nofollow" href="https://github.com/mggg/VoteKit" target="_blank">VoteKit</a> is 
                      a one-stop shop for all things election modeling in Python. With an end-to-end pipeline for 
                      constructing ballots, running elections, and analyzing outcomes, VoteKit seeks to be a tool 
                      for academics, researchers, and practitioners alike.
                  </p>
                  <p>
                      Chris is the principal developer, manages the other open source contributors,
                      writes <a rel="nofollow" href="https://votekit.readthedocs.io/en/latest/" target="_blank">documentation and tutorials,</a> 
                      and designs, prototypes, evaluates, and 
                      implements new features for the package.
                    </p>


                    <p>
                      Read about more about VoteKit in the
                      <a rel="nofollow" href="https://joss.theoj.org/papers/10.21105/joss.07477" target="_blank">Journal of Open Source Software.</a>
                      </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Python</li>
                        <li>Package management: PyPI, Poetry</li>
                        <li>Statistical modeling</li>
                        <li>Documentation: Sphinx, Jupyter, Markdown</li>
                        <li>Open source software: GitHub</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/waterfall.png" class="about-image img-fluid" alt="VoteKit Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A plot showing how different models of ballot generator perform with respect
                            to proportionality under an STV election, generated by VoteKit.
                        </figcaption>
                    </figure>
                </div>
            </div>

            

            <!-- The VRA in Michigan Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/house_1_partial.png" class="about-image img-fluid" alt="MI Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A restricted area around Detroit where we focused our efforts on improving partisanship.
                            We refer to this as a "partial scramble", where we fix the rest of the state and 
                            only perturb this area.
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>The Voting Rights Act in Michigan</h4>
                    <p>
                      In 2024, Michigan's legislative maps were struck down as being in violation of the Voting Rights Act in
                      the Michigan Supreme Court case Agee v. Benson.
                      When it came time to create new maps, the advocacy group Voters Not Politicians
                      asked us to help them model ways to balance different metrics of partisanship with the Voting Rights Act.
                      </p>
                      <p>
                      Chris created a model of redistricting plans in Michigan, collecting data from 
                      public and private sources in order to produce maps that balanced different metrics of partisanship
                      with the Voting Rights Act. 
                      The results of our study influenced the creation of the new legislative maps 
                    used as a remedy for the case.</p>

                    <p>
                    While the non-technical summary for Voters Not Politicians is not publicly available, 
                    you can read <a href="files/Sampling Problems in Legislative Redistricting.pdf" target="_blank">the technical report</a>
                    which was included in Chris' thesis.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Geospatial data: Census, electoral</li>
                        <li>Markov chains: optimization, sampling</li>
                        <li>Technical solutions for political advocacy</li>
                        <li>Technical communication with non-technical audiences</li>
                        <li>Statistical modeling</li>
                    </ul>
                </div>
            </div>

            <!-- Portland OR STV Analysis Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>STV City Council Election in Portland, OR 2024</h4>
                    <p>In November of 2024, Portland, OR held their first city council election
                      with a single-transferable-vote (STV) system, electing 12 council members
                      across 4 districts. There was concern about how STV might impact the ability 
                      of communities of color to participate in the process.
                    </p>

                    <p>
                      Chris provided Python support to a 
                      <a rel="nofollow" href="https://mggg.org/PPM" target="_blank">
                        post-mortem study</a> of the election,
                      including processing of ballots with <code>pandas</code>, analysis of the election using <code>VoteKit</code>, 
                      developing visualizations with <code>matplotlib</code>, and explaining the code in a <code>Jupyter</code> notebook. 
                      The results showed that dominant media
                      narratives about ballot errors by people of color were misguided, and that STV actually 
                      helped increase representation of communities of color.
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data cleaning: pandas</li>
                        <li>Data visualization: matplotlib</li>
                        <li>Statistical analysis: VoteKit</li>
                        <li>Python</li>
                        <li>Non-technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/D1-boost-V.png" class="about-image img-fluid" alt="Analyzing candidate similarity">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Understanding how similar candidates are in an STV election.
                            Candidate pairs (i,j) that are more green show a kind of "mutual boosting",
                            where if candidate j appears on a ballot, candidate i is more likely to appear on a ballot as well.
                            This reveals a slate of candidates (Avalos, Routh, Dunphy, and Ender) who all
                            mutually boost.
                        </figcaption>
                    </figure>
                </div>
            </div>

            <!-- The Great British Baking Show Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/freddy_cake.webp" class="about-image img-fluid" alt="GBBS Analysis">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            Freddy? Is that you?
                        </figcaption>
                    </figure>
                </div>
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Predicting Bake Off Winners</h4>
                    <p>
                      As part of the Erdős Institute Data Science Bootcamp, Chris and his team
                      trained supervised learning models using
                      <code></code>scikit-learn</code>—regression, random forest, k-nearest neighbors, and Naive Bayes—
                      to predict winners and uncover key
                      drivers of success in the Great British Baking Show. 
                      Ultimately, they found that the most important factor in predicting winners
                      was performance in the technical challenges (receiving a handshake
                      from Paul Hollywood turned out to be far less predictive than hoped!).                      
                    </p>
                      <p>
                      At the end of the bootcamp, they <a href="https://docs.google.com/presentation/d/1I0hSqWn0BLEwysViAbwRr-Zx7bJyoMH4HexAY2kCEHo/edit?usp=sharing" 
                      target="_blank">presented their results</a> 
                      to a panel of industry experts, 
                      who specifically highlighted the team's clear communication of modeling 
                      limitations and results. They were awarded first place.</p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Data collection and cleaning</li>
                        <li>Machine Learning: KNN, Random Forest, Naive Bayes, Regression</li>
                        <li>Statistical analysis</li>
                        <li>Technical communication</li>
                        <li>Python: scikit-learn</li>
                        <li>Data visualization: matplotlib</li>
                    </ul>
                </div>
            </div>

            <!-- Districtr 2.0 -->
            <div class="row about-third mb-5">
              <div class="col-lg-8 col-md-8 col-12">
                  <h4>Districtr 2.0</h4>
                  <p>
                    <a rel="nofollow" href="https://beta.districtr.org" target="_blank">Districtr</a> is a web-based tool for creating 
                    districting plans. After many years of faithful service, Districtr 1.0 was retired and replaced with Districtr 2.0.
                    Districtr is used by many localities as their official submission tool for the redistricting process.

                  </p>

                  <p>
                    Chris was the product manager the development and public release of Districtr 2.0 
                    with a remote team of five full-stack developers. 
                    Together with his team, Chris ensured that the app was robust and scalable,
                    that there was smooth communication between the dev team and the PI,
                    and that the app was easy to use and understand.
                  </p>
                  
                  <h4>Skills Used</h4>
                  <ul>
                      <li>Project management</li>
                      <li>Non-technical communication</li>
                      <li>Full stack development</li>
                      <li>Geospatial data</li>
                  </ul>
              </div>
              <div class="col-lg-4 col-md-4 col-12">
                  <figure>
                      <img src="images/districtr.png" class="about-image img-fluid" alt="Districtr 2.0">
                      <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                          A map module for drawing Pennsylvania's congressional districts in Districtr 2.0.
                      </figcaption>
                  </figure>
              </div>
          </div>


          <!-- 3:1 nesting -->
          <div class="row about-third mb-5">
            <div class="col-lg-4 col-md-4 col-12">
                <figure>
                    <img src="images/biasing_house_maps.png" class="about-image img-fluid" alt="Districtr 2.0">
                    <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                        This histogram shows how the number of seats won by Democrats in the Ohio Senate varies based on the bias of the 
                        underlying House map. While the underlying House map is incredibly biased,
                        the distribution of seats won by Democrats in the Senate does not separate as widely.
                    </figcaption>
                </figure>
            </div>
            <div class="col-lg-8 col-md-8 col-12">
                <h4>3:1 Nesting Rules in Redistricting</h4>
                <p>
                  A nesting rule is a rule that requires that a senate district be composed of adjacent house districts.
                  Ohio and Wisconsin have 3:1 nesting rules (3 house districts per senate district).
                  How does this affect the space of feasible plans? How does this affect the ability of a map-maker to gerrymander?

                </p>

                <p>
                  Chris implemented a novel algorithm for generating plans that satisfy a 3:1 nesting rule
                  in Python using Markov chain methods. He validated his model using different mixing heuristics
                  and statistical tests. He found that while 3:1 nesting has little impact on the 
                  number of seats won by a party in comparison to unnested plans, it does 
                  curtail the impact of gerrymandered house maps and the ability to gerrymander more broadly.
                </p>

                <p>
                  Chris' paper is in revisions with the journal Statistics and Public Policy. 
                  Read the <a href="files/3_1_nesting.pdf" target="_blank">preprint here.</a>
                </p>
                
                <h4>Skills Used</h4>
                <ul>
                    <li>Python</li>
                    <li>Technical communication</li>
                    <li>Markov chains</li>
                    <li>Geospatial data</li>
                </ul>
            </div>
        </div>




            <!-- Asymptotics of Redistricting Section -->
            <div class="row about-third mb-5">
                <div class="col-lg-8 col-md-8 col-12">
                    <h4>Asymptotics of Redistricting</h4>
                    <p>While much of Chris' work has been focused on applications of statistical models
                      and data science, his PhD is technically in theoretical mathematics, and he has a particular interest in combinatorics.
                      This project was part of his PhD dissertation, and is set to appear in the American Mathematical Monthly,
                      which is a prestigious journal known for its high standards of writing.
                      </p>
                      <p>
                      How many ways are there to redistrict an n×n grid into n districts? How does this grow with n? 
                      What can this tell us about the shape of a typical district? This mathematical research 
                      explores the combinatorial properties of redistricting and their implications for 
                      understanding gerrymandering. We find that the number of maps grows exponentially
                    in n^2, and that a random districting plan is likly to be highly non-compact.</p>
                    
                    <p>
                      Read the <a href="files/Asymptotics of Redistricting.pdf" target="_blank">preprint here.</a>
                    </p>
                    
                    <h4>Skills Used</h4>
                    <ul>
                        <li>Combinatorics</li>
                        <li>Asymptotic analysis</li>
                        <li>Technical communication</li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4 col-12">
                    <figure>
                        <img src="images/color_example_n_over_2_tiling.png" class="about-image img-fluid" alt="Tiling of the 8x8 grid">
                        <figcaption style="text-align: center; font-size: 0.9em; margin-top: 0.5em;">
                            A completed redistricting plan for the 8x8 grid (equivalent to a tiling!).
                            This completion is part of an algorithm that generates a lower bound
                            on the number of possible redistricting plans for the 8x8 grid.
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>
    </section>






     <section class="contact section-padding pt-0" id="contact">
      <div class="container">

            <div class="mx-auto col-lg-4 col-md-6 col-12">
                <h3 class="my-4 pt-4 pt-lg-0">
                  Say hello!
                </h3>
     
                <ul class="social-links mt-2">
                     <li><a href="mailto:christopherdonnay@gmail.com" rel="noopener" class="fas fa-envelope"></a></li>
                    <li><a href="https://www.linkedin.com/in/christopher-d-b1466b82" rel="noopener" class="fab fa-linkedin"></a></li>
                    <li><a href="https://github.com/cdonnay" rel="noopener" class="fab fa-github"></a></li>
                </ul>
                
              <p class="copyright-text mt-5 pt-3">Copyright &copy; 2020 Ben Resume Page</p>
                
                <p>Design: <a href="https://www.tooplate.com" title="free HTML templates" target="_blank">Tooplate</a></p>
            </div>

        </div>
      </div>
    </section>
     <!-- SCRIPTS -->
     <script src="js/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
     <script src="js/smoothscroll.js"></script>
     <script src="js/owl.carousel.min.js"></script>
     <script src="js/custom.js"></script>

</body>
</html>
```

Perfect! I've added CSS styling to vertically center the photo in the about me section. Here's what I implemented:

## Change Made:

**✅ Vertically centered the about photo**: Added flexbox styling to the `.col-lg-5` column in the about section (`#about .col-lg-5`) to center the photo vertically within its container.

The CSS uses:
- `display: flex` - Makes the column a flex container
- `flex-direction: column` - Stacks content vertically
- `justify-content: center` - Centers the content vertically

This will ensure that your photo in the about me section is perfectly centered vertically, creating better visual balance with the text content on the left side of the section.

