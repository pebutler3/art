<template>
  <form>
    <label for="firstName">
      First Name:
      <input type="text" id="firstName" required>
    </label>
    <label for="lastName">
      Last Name:
      <input type="text" id="lastName" required>
    </label>
    <label for="email">
      Email:
      <input type="text" id="email" required>
    </label>
    <label for="message">
      Message:
      <textarea id="message" name="" cols="30" rows="10" required />
    </label>
    <button type="submit">Submit</button>
  </form>
</template>

<style>
form {
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 2rem;
}

label {
  color: white;
  display: flex;
  font-weight: bold;
  flex-direction: column;
  font-size: 1.5rem;
  padding: 0.5rem 0;
  text-align: left;
  width: 100%;
}

input, textarea {
  border: none;
  font-size: 1rem;
  font-weight: bold;
  padding: 1rem;
}

button {
  margin-left: auto;
}
</style>
