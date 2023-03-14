<template>
  <main>
    <div class="container">
      <div class="hero-img">
        <img class="img-main" src="./assets/bleu-2.jpg" alt="perfume bottle" />
      </div>
      <div class="description">
        <p class="subtitle">perfume</p>
        <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
        <p class="leading">
          A floral, solar and voluptuous interpretation composed by Olivier
          Polge, Perfumer-Creator for the House of CHANEL.
        </p>

        <div class="price">
          <h2 class="price-main">$149.99</h2>
          <p class="price-orig">$169.99</p>
        </div>

        <a href="#" class="btn-add">
          <svg
            class="btn-icon-add"
            width="15"
            height="16"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z"
              fill="#FFF"
            />
          </svg>
          Add to Cart
        </a>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: var(--cream);
  height: 100vh;
}

img {
  width: 100%;
}

h1,
h2 {
  font-family: "Fraunces", serif;
}

p {
  font-size: 0.9rem;
  color: var(--dark-grayish-blue);
}

.hero-img {
  margin-bottom: -4px; /*removing extra space bet container div*/
}

.img-main {
  border-radius: 0.5rem 0.5rem 0 0;
}

.subtitle {
  text-transform: uppercase;
  letter-spacing: 0.25rem;
  font-size: 0.75rem;
  padding-bottom: 1rem;
}

.title {
  padding-bottom: 0.75rem;
  line-height: 2rem;
}

.container {
  padding: 1.75rem 1rem;
}

.description {
  background-color: var(--white);
  padding: 1.5rem;
  border-radius: 0 0 0.5rem 0.5rem;
}

.leading {
  line-height: 1.25rem;
  padding-bottom: 1rem;
}

.price {
  display: flex;
  padding-bottom: 1rem;
}

.btn-add {
  background-color: var(--dark-cyan);
  color: var(--white);
  font-size: 0.85rem;
  font-weight: 700;
  border: none;
  text-decoration: none;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 0.5rem;
  padding: 1.1rem;
  width: 100%;
  max-width: 295px;
}

.btn-icon-add {
  position: relative;
  margin-right: 0.5rem;
}

.price-orig {
  text-decoration: line-through;
  align-self: center;
}

.price-main {
  font-size: 2rem;
  font-weight: 700;
  color: var(--dark-cyan);
  padding-right: 1rem;
  justify-items: ;
}

@media (width >= 768px) {
  main {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .container {
    display: flex;
  }

  .description {
    max-width: 280px;
    max-height: 384px;
    border-radius: 0 0.5rem 0.5rem 0;
  }

  .img-main {
    content: url("./assets/bleu-2.jpg");
    max-height: 620px;
    max-width: 256px; /* You must set a specified height */
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: cover;
    border-radius: 0.5rem 0 0 0.5rem;
  }
}
</style>
