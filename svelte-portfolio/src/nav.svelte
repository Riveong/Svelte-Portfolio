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
  