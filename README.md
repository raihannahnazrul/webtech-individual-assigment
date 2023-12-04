# webtech-individual-assigment

<!--The javascript function that i add is scrolling button -->
  <style>
  
    #scrollToTopBtn {
      display: none;
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #333;
      color: #fff;
      padding: 10px;
      border: none;
      cursor: pointer;
    }

    #scrollToTopBtn:hover {
      background-color: #942424;
    }
  </style>
</head>
 
 
<body> 
 
 <script>
   // This function is to scroll from bottom to top smoothly
   function scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    }

    // scroll event listener is to show and hide the button when depending the way user scroll which is either scroll up or scroll down
    window.addEventListener('scroll', function () {
      const scrollToTopBtn = document.getElementById('scrollToTopBtn');
      if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
        scrollToTopBtn.style.display = 'block';
      } else {
        scrollToTopBtn.style.display = 'none';
      }
    });
    </script>
</body>


 // When the user clicks the button, the page will smoothly scroll to the top.

