# CSS-media-queries
This repository demonstrates how to make a simple website responsive and mobile-friendly using CSS Media Queries.

✅ Features
1.Responsive design for mobile, tablet, and desktop
2.Clean HTML and CSS structure
3.Uses media queries to adapt layout and styling
4.Example of flexible grid and navigation behavior
5.Includes meta viewport tag for scaling
Technologies Used:HTML,CSS,Media Queries
**html code**
<html>
    <head>
      <meta name="viewport" content="width=device-width,initial-scale=1.0">
            <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous" />
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
    <script src="https://kit.fontawesome.com/ac42c3b1f7.js" crossorigin="anonymous"></script>
    </head>
    <link rel="stylesheet" href="style.css">
    <body>
      <nav class="navbar navbar-expand-lg navbar-light bg-light " >
        <a class="navbar-brand" href="#travel" id="nav-bar">travel</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav">
            <a class="nav-link active" href="#home" id="navitem1">
              Home
              <span class="sr-only">(current)</span>
            </a>
            <a class="nav-link" href="#destination" id="navitem2">Destination</a>
            <a class="nav-link" href="#about us" id="navitem3">About us</a>
            <a class="nav-link" href="#contact us" id="navitem4">Contact us</a>
  
          </div>
        </div>
      </nav>
          <div class="bg-container d-flex justify-content-center flex-column">
            <div class="text-center">
              <h1 class="heading">Explore the World<br>
                 Without Limits</h1>
              <p class="para">Discover new places, meet new people, and create
                 memories that last forever.Your next adventure is just a step away.
                </p>
                <div class="buttons">
              <button class="button">explore now...</button>
            </div>
            </div>
          </div>
      
    
    </body>
</html>


**CSS CODE**
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");


.bg-container{
    background-image:url("https://media.istockphoto.com/id/619394704/photo/serene-young-man-watching-plane-before-departure.jpg?s=612x612&w=0&k=20&c=yhl90rjHEP75S9ndsjn1RM2BNPogQPcav-4QJLQrXsM=");
    height:100vh;
    background-size:cover;
}

#nav-bar{
    height:45px;
    font-weight: bold;
    font-size: large;
    font-family:"lucida handwriting";
    color:#a66817;    
}


#navitem1{
    color:#595248;
    font-family: "Lucida Sans";
}
#navitem2{
    color:#595248;
    font-family: "Lucida Sans";
}
#navitem3{
    color:#595248;
    font-family: "Lucida Sans";
}
#navitem4{
    color:#595248;
    font-family: "Lucida Sans";
}
.text-center{
     padding-left:10%;
     padding-bottom: 25%;
     margin-right: 5%;
}
.heading{
    font-size: 65px;
    font-family:  georgia;
    color: black;
    height:max-content; 
    text-align: end;
    
}

.para{
    font-family: "comic sans ms";
    font-size: 18px;
    color:#302d28;
    height:min-content;
    text-align:left;
    padding-left: 59%;
    
}
.buttons{
    text-align: end;
    padding-right: 15%;
}
.button{
    height:55px;
    width:150px;
    border-radius: 15px;
    color:black;
    font-size:18px ;
    font-family: 'comic sans ms';
    background-color: transparent;
    border-width: 2.8px;
    font-weight:500;
    
}



@media screen and (max-width: 768px ) {
    .text-center{
     padding-left:7%;
     padding-bottom: 15%;
     margin-right: 5%;
}
    .heading{
    font-size: 30px;
    font-weight: lighter;
    height:max-content;
    text-align: end;
    }
    .para{
        font-family: 'comic sans ms';
    font-size: 18px;
    color:black;
    height:min-content;
    text-align: end;
}
.buttons{
    text-align: end;
    padding:0%;
}
.button{
    height:45px;
    width:100px;
    border-radius: 15px;
    color:black;
    font-size:11px ;
    font-family: 'comic sans ms';
    background-color: transparent;
    border-width: 2.8px;
    font-weight:500;
    
}    
}



