<script>
  let projects = [];

  fetch('data/projects.json')
    .then(response => response.json())
    .then(data => {
      projects = data.projects;
    });
</script>

<h1>Projects</h1>
<div id="projects"class="cards-container" style="background-color: #1c1c1c ;">
  <div>
    <h2>20+ Projects</h2>
    <p class="intro">Over 20+ projects have been finished,
    <br>here are the most notable projects
    <br> for more projects you can check my github</p>
    <a href="https://github.com/Riveong" class="btn">Github</a>
  </div>
  {#each projects as project}
    <div class="card">
      <h3>{project.Title}</h3>
      <p>{project.Description}</p>
      <span class="tag">{project.tag}</span>
      <a href="{project.link}" target="_blank">View Project</a>
    </div>
  {/each}
</div>

  
<style>
  .cards-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
  }

  .card {
    background-color: white;
    color: black;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    margin: 10px;
    padding: 20px;
    width: 300px; /* Adjust width as needed */
  }

  .card h3 {
    margin-top: 0;
  }

  .card .tag {
    display: inline-block;
    background-color: #e0e0e0;
    border-radius: 5px;
    padding: 5px 10px;
    margin-top: 10px;
  }

  .card a {
    display: inline-block;
    margin-top: 15px;
    color: blue;
    text-decoration: none;
  }

  h2{
    color: #fff;
  }

  p.intro{
    color: #fff;
  }

  .btn {
    -webkit-border-radius: 10;
    -moz-border-radius: 10;
    border-radius: 10px;
    font-family: Arial;
    color: #ffffff;
    background-color: transparent;
    font-size: 15px;
    padding: 10px 20px 10px 20px;
    border: solid #ffffff 2px;
    text-decoration: none;
  }

</style>

  