<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Me</title>
  <link rel="stylesheet" href="https://anjugopinath.github.io/styles/about.css">
  <style>
    /* General Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }

    .content {
      max-width: 1200px;
      margin: 0 auto;
      padding: 15px;
      box-sizing: border-box;
    }

    img {
      max-width: 100%;
      height: auto;
      display: block;
      margin: 0 auto;
    }

    p {
      text-align: justify;
      margin: 15px 0;
    }

    a {
      color: #007bff;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Responsive Layout */
    @media (max-width: 768px) {
      .content {
        padding: 10px;
      }

      img {
        margin-bottom: 15px;
      }
    }

    @media (max-width: 480px) {
      p {
        font-size: 14px;
      }
    }
  </style>
</head>
<body>
  <div class="content">
    <img src="https://anjugopinath.github.io/styles/AnjuGopinath.png" alt="Anju Gopinath">
    <p>Hi there!</p>
    <p>
      I am Anju, a Ph.D. student at Colorado State University. I am advised by 
      <a href="https://www.nikhilkrishnaswamy.com/">Dr. Nikhil Krishnaswamy</a> at the 
      <a href="https://www.signallab.ai/">SIGNAL</a> Lab and co-advised by 
      <a href="https://www.cs.colostate.edu/~draper/">Dr. Bruce Draper</a>. I specialize in Computer Vision and Machine Learning.
    </p>
    <p>
      I did my Master’s in Computer Science and Engineering at IIT Madras, India. Previously, I worked at Subex Ltd., Intel India Pvt. Ltd., and Oppo US Research Centre. My main research interests are hand grasps and 
      <a href="http://cs.brown.edu/courses/cs137/2017/readings/Gibson-AFF.pdf">affordances</a>. Among other things, this has applications in robots tasked to pick, transfer and place objects at desired locations in factories, or avatars interacting with objects in mixed reality environments.
    </p>
    <p>
      Feel free to email me regarding collaboration opportunities at anju [at] colostate [dot] edu.
    </p>
  </div>
</body>
</html>

 
<br />

{% include contact.html %}
