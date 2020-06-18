<template>
<head>
    <title>Contact Form</title>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/emailjs-com@2.4.1/dist/email.min.js"></script>
    <script type="text/javascript">
        (function(){
           emailjs.init('user_TMkl3kJFoaI7qrIt4dbI2');
        })();
    </script>
    <script type="text/javascript">
        window.onload = function() {
            document.getElementById('contact-form').addEventListener('submit', function(event) {
                event.preventDefault();
                // generate the contact number value
                this.contact_number.value = Math.random() * 100000 | 0;
                emailjs.sendForm('contact_service', 'contact_form', this);
            });
        }
    </script>
</head>
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
      <input type="submit" value="Enviar">
    </div>
  </form>
</template>
