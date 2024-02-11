<script>
    function scrollToSection(sectionId) {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
      }
    }
  </script>
  
  <nav>   
    <ul>
      <li><button on:click={() => scrollToSection('about')}>About Me</button></li>
      <li><button on:click={() => scrollToSection('projects')}>Projects</button></li>
      <li><button on:click={() => scrollToSection('blog')}>Blog</button></li>
    </ul>
  </nav>
  <a href="https://www.youtube.com/channel/UC5s3FdG5mlgcQ9XofSF8p6w"><img alt="YouTube Channel Subscribers" src="https://img.shields.io/youtube/channel/subscribers/UC5s3FdG5mlgcQ9XofSF8p6w?style=for-the-badge&logo=Youtube&logoColor=red"></a>
  <a href="https://www.linkedin.com/in/ong-gabriel-riverine-susanto-8994b2266/"><img alt="Linked In" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="https://github.com/Riveong"><img alt="Github" src="https://img.shields.io/badge/Github-000000?style=for-the-badge&logo=github&logoColor=white"></a>
  
  <style>
    nav {
      background-color: #1c1c1c;
      text-align: end; /* Align to end */
      padding: 10px;
    }
  
    nav ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      justify-content: flex-end; /* Align items to the end */
    }
    a {
      display: flex;
      justify-content: flex-end;
    }
  
    nav li {
      margin-left: 20px; /* Space between menu items */
    }
  
    button {
      background: none;
      border: none;
      color: white;
      cursor: pointer;
      font-size: 16px;
      transition: color 0.3s;
    }
  
    button:hover {
      color: lightblue; /* Color on hover */
    }
    
  </style>
  