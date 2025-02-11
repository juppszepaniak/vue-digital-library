<template>
  <div class="library-container">
    <div class="book-card">
      <div class="book-card-description"></div>
      <h3>Schuld und Sühne</h3>
      <p>Fjodor Dostojewski</p>
      <img
        src="https://images.thalia.media/-/BF750-750/a31a3c76d4264e09bdab6ad841cf41f8/schuld-und-suehne-taschenbuch-fjodor-m-dostojewski.jpeg"
        alt="Book Cover"
      />
    </div>
    <div class="book-card">
      <h3>David Copperfield</h3>
      <p>Charles Dickens</p>
      <img
        src="https://images.thalia.media/-/BF2000-2000/63fb92402c7f45c58227033b3b53195f/david-copperfield-gebundene-ausgabe-charles-dickens.jpeg"
        alt="Book Cover"
      />
    </div>
    <div class="book-card">
      <h3>Stolz und Vorurteil</h3>
      <p>Jane Austen</p>
      <img
        src="https://medien.umbreitkatalog.de/bildzentrale_original/978/315/020/4085.jpg"
        alt="Book Cover"
      />
    </div>
    <button class="btn add-book-card">+</button>
  </div>
</template>

<script>
export default {};
</script>

<style>
.library-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1rem;
  padding: 2rem;
}

.add-book-card {
  font-size: 5rem;
}
.book-card {
  background: var(--text-clr);
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 1rem;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.add-book-card {
  background: var(--text-clr);
  border: 1px solid var(--text-clr);
  border-radius: 8px;
  padding: 1rem;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.book-card img {
  max-width: 100%;
  max-height: 400px;
  border-radius: 4px;
  margin-top: 1rem;
}
.book-card h3 {
  margin-bottom: 0.5rem;
}
.book-card p {
  font-size: 0.9rem;
  color: var(--dark-text-clr);
}
</style>
