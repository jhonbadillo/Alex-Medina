<template>
  <form>
    <!-- Name -->
    <div class="field">
      <label class="label is-medium">Nombre</label>
      <div class="control has-icons-left">
        <input class="input is-medium" type="text" placeholder="Jhon B" />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="user" />
        </span>
      </div>
    </div>
    <!-- Email -->
    <div class="field">
      <label class="label is-medium">Email</label>
      <div class="control has-icons-left">
        <input
          class="input is-medium"
          type="email"
          placeholder="you@email.com"
        />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="envelope" />
        </span>
      </div>
    </div>
    <!-- Subject -->
    <div class="field">
      <label class="label is-medium">Asunto</label>
      <div class="control has-icons-left">
        <input
          class="input is-medium"
          type="text"
          placeholder="Breve resumen"
        />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="briefcase" />
        </span>
      </div>
    </div>
    <!-- Message -->
    <div class="field">
      <label class="label is-medium">Mensaje</label>
      <div class="control">
        <textarea
          class="textarea"
          placeholder="Descripción detallada de su comentario, solicitud, etc."
          rows="8"
        ></textarea>
      </div>
    </div>
    <div class="control">
     <button class="button is-primary">
        Contactenos
      </button>
    </div>
  </form>
</template>
