<template>
  <main>
    <div class="card-container">
      <img
        class="card-img"
        src="./assets/bleu-2.jpg"
        alt="bleu de chanel perfume bottle"
      />
      <div class="card-description">
        <p class="card-category">perfume</p>
        <h1 class="card-title">Gabrielle Essence Eau De Parfum</h1>
        <p class="card-lead-text">
          A Woody Aromatic fragrance interpretation composed by Olivier Polge,
          Perfumer-Creator for the House of CHANEL.
        </p>
        <div class="card-prices">
          <span class="price-new">$149.99</span>
          <span class="price-old" aria-hidden="true">$169.99</span>
        </div>
        <button class="card-btn-add" type="button">
          <svg
            class="card-btn-icon"
            width="16px"
            height="16px"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M14.383 10.388a2.397 2.397 0 0 0-1.518-2.222l1.494-5.593a.8.8 0 0 0-.144-.695.8.8 0 0 0-.631-.28H2.637L2.373.591A.8.8 0 0 0 1.598 0H0v1.598h.983l1.982 7.4a.8.8 0 0 0 .799.59h8.222a.8.8 0 0 1 0 1.599H1.598a.8.8 0 1 0 0 1.598h.943a2.397 2.397 0 1 0 4.507 0h1.885a2.397 2.397 0 1 0 4.331-.376 2.397 2.397 0 0 0 1.12-2.021ZM11.26 7.99H4.395L3.068 3.196h9.477L11.26 7.991Zm-6.465 6.392a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Zm6.393 0a.8.8 0 1 1 0-1.598.8.8 0 0 1 0 1.598Z"
              fill="#FFF"
            />
          </svg>
          Add to Cart
        </button>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  display: -ms-grid;
  display: grid;
  place-content: center;
  min-height: 100vh;
  background-color: var(--cream);
}

p {
  color: var(--cream);
}
.card-container {
  display: -ms-grid;
  display: grid;
  padding: 1rem;
  max-width: 26.5625rem;
  border-radius: 0.6rem;
}
.card-img {
  width: 100%;
  height: 15.375rem;
  -o-object-fit: cover;
  object-fit: cover;
  -o-object-position: center;
  object-position: center;
  border-radius: 0.6rem 0.6rem 0 0;
}

.card-description {
  background-color: var(--very-dark-blue);
  color: var(--white);
  padding: 1.5rem;
  border-radius: 0 0 0.6rem 0.6rem;
}

.card-category {
  text-transform: uppercase;
  font-size: 0.75rem;
  letter-spacing: 0.5rem;
  margin-left: 0.15rem;
  padding-bottom: 1rem;
}

.card-title {
  font-family: "Fraunces", serif;
  line-height: 2.25rem;
}

.card-lead-text {
  font-size: 0.85rem;
  padding: 0.75rem 0;
}

.card-prices {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 1.5rem;
  padding: 0.75rem 0;
}

.price-new {
  font-family: "Fraunces", serif;
  font-size: 2rem;
  color: var(--purple);
}

.price-old {
  text-decoration: line-through;
  font-size: 0.85rem;
}

button {
  all: unset;
}

.card-btn-add {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 0.65rem;
  border-radius: 0.5rem;
  width: 100%;
  height: 3rem;
  background-color: var(--pale-blue);
  -webkit-transition: ease-out 0.3s;
  -o-transition: ease-out 0.3s;
  transition: ease-out 0.3s;
}

.card-btn-add:hover {
  cursor: pointer;
  background-color: var(--purple);
}

@media (width>=48rem) {
  .card-container {
    -ms-grid-columns: 1fr 1fr;
    grid-template-columns: 1fr 1fr;
    max-width: 37.5rem;
    padding: 0;
    -webkit-box-shadow: 20px 31px 67px -17px rgba(92, 83, 92, 1);
    box-shadow: 20px 31px 67px -17px rgba(92, 83, 92, 1);
  }

  .card-img {
    height: 100%;
    border-radius: 0.6rem 0 0 0.6rem;
  }

  .card-category {
    padding-bottom: 0.65rem;
  }

  .card-description {
    padding: 2.2rem;
    border-radius: 0 0.6rem 0.6rem 0;
  }

  .card-title {
    padding: 0.4rem 0;
    font-size: 1.9rem;
    line-height: 2.1rem;
  }

  .card-lead-text {
    line-height: 1.5rem;
  }

  .card-prices {
    padding: 0 0 1.5rem;
  }

  .card-btn-add {
    height: 2.8rem;
    font-size: 0.85rem;
  }
}
</style>
