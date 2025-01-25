<template>
  <div id="contactContainer">
    <h2>Enquiries</h2>
    <form action="https://formspree.io/f/xknykdjb" method="POST">
      <label for="name">
        <!-- <p class="formHeader">Your Name:</p> -->
        <input type="text" name="name" placeholder="YOUR NAME?" required />
      </label>
      <label for="number">
        <!-- <p class="formHeader">Your Email:</p> -->
        <input type="tel" name="telephone" placeholder="YOUR NUMBER?" required />
      </label>
      <label for="email">
        <!-- <p class="formHeader">Your Email:</p> -->
        <input type="email" name="email" placeholder="YOUR EMAIL?" required />
      </label>
      <label for="message">
        <!-- <p class="formHeader">Message:</p> -->
        <textarea name="message" class="body" placeholder="MESSAGE" required></textarea>
      </label>
      <button class="formSubmit" type="submit">SEND</button>
    </form>
  </div>
</template>

<style scoped>
#contactContainer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 5em 1em;
  text-align: center;
}

h2 {
  font-size: 2.5rem;
  text-align: center;
  padding: 20px;
  font-family: lora;
  font-weight: 600;
  letter-spacing: 5px;
  text-decoration: underline;
  text-decoration-color: rgb(50, 143, 75);
  text-decoration-thickness: 2px;
  text-underline-offset: 20px;
  padding-bottom: 40px;
}

.formHeader {
  padding-bottom: 5px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  width: 90%;
  max-width: 600px;
}

label {
  display: flex;
  flex-direction: column;
  font-weight: 500;
  border: none;
}

input,
textarea {
  padding: 10px;
  font-size: 1em;
  border: 1px black solid;
  border-top: none;
  border-left: none;
  border-right: none;
  background-color: rgb(250, 250, 250);
  color: black;
}

input::placeholder,
textarea::placeholder {
  opacity: 1;
}

textarea {
  resize: vertical;
  min-height: 100px;
}

input:focus,
textarea:focus {
  outline: none;
}

button.formSubmit {
  padding: 10px;
  border: none;
  border-radius: 3px;
  font-weight: 400;
  letter-spacing: 1.1px;
  font-size: 1.2em;
  cursor: pointer;
  transition: 0.3s ease;
  text-align: start;
  background-color: rgb(250, 250, 250);
  color: black;
}

button.formSubmit:hover {
  cursor: pointer;
  color: grey;
}
p {
  text-align: start;
}

@media (min-width: 768px) {
  h2 {
    font-size: 4.5rem;
  }

  form {
    width: 80%;
  }

  input {
    height: 40px;
    margin-top: 5px;
  }

  p {
    text-align: start;
  }
}
</style>
