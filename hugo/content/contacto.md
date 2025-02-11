+++
date = '2025-02-11T12:15:14+01:00'
draft = false
isContacto = true
title = 'Contacto'
+++

<section>
  <div class="content">
    <form class="form-panel"
	  name="contact"
          action="/contacto-ok.html"
	  method="POST"
	  data-netlify="true"
	  netlify-honeypot="bot">
      <h2>¿Hablamos?</h2>
      <div class="hidden">
        <label for="bot">Por favor, NO rellenes este campo:</label>
        <input name="bot" id="bot" type="text">
      </div>
      <div class="form-control">
        <label for="name">Nombre:</label>
        <input name="name" id="name" type="text">
      </div>
      <div class="form-control">
        <label for="email">Mail:</label>
        <input name="email" id="email" type="email">
      </div>
      <div class="form-control">
	<label for="profile">¿Cuál es tu perfil?:</label>
	<div class="form-select">
          <select name="profile">
            <option value="Docente">Docente</option>
            <option value="Investigador">Investigador</option>
            <option value="TIC">Responsable TIC</option>
            <option value="Familia">Familia</option>
            <option value="Inversor">Inversor</option>
            <option value="Otro">Otro</option>				
          </select>
        </div>
      </div>
      <div class="form-control">
        <label for="message">Mensaje:</label>
        <textarea name="message" id="message"></textarea>
      </div>
      <div class="buttons">
        <button type="submit" class="btn">Enviar</button>
      </div>
    </form>
    
  </div>
</section>
