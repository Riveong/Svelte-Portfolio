<script>
    import { onMount } from 'svelte';
    let posts = [];
  
    onMount(async () => {
      const response = await fetch('http://localhost:8000/rss');
      const data = await response.json();
      const text = data.content;
      const parser = new DOMParser();
      const doc = parser.parseFromString(text, 'application/xml');
      posts = Array.from(doc.querySelectorAll('item'));
    });
  </script>
  
  {#each posts as post (post)}
    <article>
      <h2>{post.querySelector('title').textContent}</h2>
      <p>{post.querySelector('description').textContent}</p>
      <a href={post.querySelector('link').textContent}>Read more</a>
    </article>
  {/each}
  
  
  
    
  <style>
   
  </style>
  
    