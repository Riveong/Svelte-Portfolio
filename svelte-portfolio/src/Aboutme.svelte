<script>
  const interests = ["👨‍💻 Backend","💻 Sofware Development","📱 Android","🤖 Machine Learning","🎮 Game Development","🎨 UI Design","🔬 UX Research","🧾 RecSYS","🎮 Games","🎲 D&D","✍ Writing"]
</script>

<h1>About me</h1>
<header id="about" class="container" style="background-color: #1c1c1c ; color: white; ">
      <h2>Profile</h2>
      <p>Hiya my name is Ong Gabriel Riverine Susanto👋, I’m an undergraduate student at Sanata Dharma University <b>(last semester!)</b>, Bangkit 2023 Batch 1 Cloud Computing participant, Bangkit 2023 Batch 2 Mobile Dev Participant <b>(graduated with distinction)</b>.
        I am a lover of tech, tea and all its wonders. I marvel at the power of Back-end dev, UI/UX and the infinite possibilities it offers. I delight in learning new things and expanding my horizons. I cherish writing and art as forms of expression and creativity 🎨🖌️</p>
        
      
    
        <h2>Interest</h2>
        <div class="carousel">
          {#each interests as interest}
            <div class="item-container">
              <p>{interest}</p>
            </div>
          {/each}
        </div>
      
        <h2>Stacks</h2>
        <img alt="Node" src="https://img.shields.io/badge/JS-000000?style=for-the-badge&logo=javascript">
        <img alt="Node" src="https://img.shields.io/badge/Node-000000?style=for-the-badge&logo=node.js">
        <img alt="FastAPI" src="https://img.shields.io/badge/Kotlin-000000?style=for-the-badge&logo=Kotlin">
        <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-000000?style=for-the-badge&logo=FastAPI">
        <img alt="FastAPI" src="https://img.shields.io/badge/flask-000000?style=for-the-badge&logo=flask">
        <img alt="FastAPI" src="https://img.shields.io/badge/mysql-000000?style=for-the-badge&logo=mysql">
        <img alt="FastAPI" src="https://img.shields.io/badge/godot-000000?style=for-the-badge&logo=godot-engine">
        <img alt="FastAPI" src="https://img.shields.io/badge/fastify-000000?style=for-the-badge&logo=fastify">
        <img alt="FastAPI" src="https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python">
        <img alt="Svelte" src="https://img.shields.io/badge/Svelte-000000?style=for-the-badge&logo=svelte">
</header>
    
    <style>
      header {
        text-align: left;
        padding: 20px;
      }
      .carousel {
        display: flex;
        overflow-x: auto;
        scroll-behavior: smooth;
        -webkit-overflow-scrolling: touch;
        padding: 10px 0;
      }

      .item-container {
        flex: 0 0 auto;
        background-color: white;
        color: black;
        padding: 10px;
        margin-right: 10px;
        border-radius: 5px;
        box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        text-align: center;
      }

      .item-container p {
        margin: 0;
      }

    </style>