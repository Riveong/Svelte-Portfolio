<script>
let cardInfo = {
  imageUrl: 'https://media.discordapp.net/attachments/1023598916857499680/1202244106215243786/48bb4759-8d22-481b-b09c-a4b6023acecf-removebg-preview.png?ex=65ccc013&is=65ba4b13&hm=72547bf8b48187236366c6532984577ba53a7c70d60cc24a8e449190c2839188&=&format=webp&quality=lossless',
  title: 'If I play D&D my OC would be based on my personality...',
  description: ['Race\n: Human', 'Class\n: Paladin (Oath of Glory) / Bard (College of Lore)', 'Alignment\n: Chaotic Good', 'Description\n: As a Paladin who has taken the Oath of Glory, I never leave my oath to achieve something and never run away from responsibility. I am committed to seeing a project through to its completion, no matter the challenges that arise. At the same time am multiclassing to bard, my Bardic abilities from the College of Lore translate well for being a good team member. Being good at teamwork, used to critique and giving critique are essential skills.']
};

</script>

<section>    
        <div class="card">
          <img src={cardInfo.imageUrl} alt="Card Image" class="card-image"/>
          <div class="card-text">
              <h2>{cardInfo.title}</h2>
            {#each cardInfo.description as item (item)}
                <p>{item}</p>
            {/each}
          </div>
</section>
<style>
        .card {
        display: flex;
        align-items: center;
        background-color: #000;
        padding: 10px;
        border-radius: 8px;
        box-shadow: 0 2px 4px rgba(0,0,0,0.2);
    }

    .card-image {
        max-width: 300px; /* Adjust as needed */
        height: auto; /* Adjust as needed */
        object-fit: cover;
        border-radius: 4px;
        margin-right: 15px;
    }

    .card-text {
        flex-grow: 1;
        color: white;
    }

    .card-text h2 {
        margin: 0 0 10px 0;
    }

    .card-text p {
        margin: 0;
    }
</style>