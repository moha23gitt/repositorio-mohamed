3. 20261119-LND-UT1-Examen-Tipo-01.pdf
Ejercicio 1 — Colocar justo debajo de <header>
HTML
<section id="ej1-tareas">
  <h2>Ejercicio 1</h2>
  <div class="grid-tareas">
    <article class="caja-t">
      <h3>Tareas para Halloween</h3>
      <ul>
        <li>Ir de fiesta</li>
        <li>Divertirse mucho</li>
        <li>No pasar miedo</li>
        <li>Hacer una pagina web de Halloween</li>
        <li>Reirse al leer la tarea anterior</li>
      </ul>
    </article>
    <article class="caja-t">
      <h3>Tareas para los Finaos</h3>
      <ol>
        <li>Ir al cementerio</li>
        <li>Vivir momentos entrañables</li>
        <li>Acordarse de los seres queridos</li>
        <li>Comer dulces</li>
        <li>Ser feliz</li>
      </ol>
    </article>
  </div>
</section>
CSS
#ej1-tareas h2 {
  text-align: center;
}

.grid-tareas {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-inline: 2rem;
}

.caja-t {
  background-color: lightblue;
  padding: 1rem;
}

/* Tablet */
@media (max-width: 1024px) {
  .caja-t {
    background-color: lightcoral;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .caja-t {
    background-color: lightgreen;
  }
}
Ejercicio 2 — Colocar justo antes de <footer>
HTML
<section id="ej2-cajas">
  <h2>Ejercicio 2</h2>
  <div class="grid-cajas">
    <article class="caja-e2">
      <h3>Primera caja</h3>
      <p>Este es el texto de la primera caja.</p>
    </article>
    <article class="caja-e2">
      <h3>Segunda caja</h3>
      <p>Este es el texto de la segunda caja.</p>
    </article>
    <figure class="img-e2">
      <img src="el-examen/calle.jpg" alt="Ejercicio 2">
    </figure>
  </div>
</section>
CSS
#ej2-cajas h2 {
  text-align: center;
}

.grid-cajas {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-inline: 2rem;
}

.img-e2 {
  margin: 0;
}

.img-e2 img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.caja-e2 {
  background-color: lightblue;
  padding: 1rem;
  text-align: left;
}

/* Tablet */
@media (max-width: 1024px) {
  .grid-cajas {
    grid-template-columns: repeat(2, 1fr);
  }
  .img-e2 {
    grid-column: 1 / -1;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .grid-cajas {
    grid-template-columns: 1fr;
  }
  .img-e2 {
    grid-column: auto;
  }
}





2. 20261119-LND-UT1-Examen-Tipo-02.pdf
Ejercicio 1 — Colocar justo debajo de <header>
HTML
<section id="ej1-paths">
  <h2>Exercise 1 - Learning Paths</h2>
  <div class="grid-paths">
    <article class="caja-p">
      <h3>Web Development</h3>
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
      </ul>
    </article>
    <article class="caja-p">
      <h3>Programming</h3>
      <ol>
        <li>Python</li>
        <li>Java</li>
        <li>PHP</li>
      </ol>
    </article>
    <article class="caja-p">
      <h3>Databases</h3>
      <ul>
        <li>SQL</li>
        <li>Tables</li>
        <li>Queries</li>
      </ul>
    </article>
    <article class="caja-p cyber-p">
      <h3>Cybersecurity</h3>
      <ol>
        <li>Passwords</li>
        <li>Networks</li>
        <li>Backups</li>
      </ol>
    </article>
  </div>
</section>
CSS
#ej1-paths h2 {
  text-align: center;
}

.grid-paths {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-inline: 2rem;
}

.cyber-p {
  grid-column: 1 / -1;
}

.caja-p {
  background-color: lightblue;
  padding: 1rem;
}

/* Tablet */
@media (max-width: 1024px) {
  .grid-paths {
    grid-template-columns: repeat(2, 1fr);
  }
  .cyber-p {
    grid-column: auto;
  }
  .caja-p {
    background-color: lightcoral;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .grid-paths {
    grid-template-columns: 1fr;
  }
  .caja-p {
    background-color: lightgreen;
  }
}
Ejercicio 2 — Colocar justo antes de <footer>
HTML
<section id="ej2-city">
  <h2>Exercise 2 - City Guide</h2>
  <div class="grid-city">
    <article class="caja-c discover-c">
      <h3>Discover</h3>
      <p>Explore interesting streets and landmarks.</p>
    </article>
    <article class="caja-c activities-c">
      <h3>Activities</h3>
      <p>Find places to visit and things to do.</p>
    </article>
    <article class="caja-c food-c">
      <h3>Food</h3>
      <p>Try traditional dishes and local cafes.</p>
    </article>
    <figure class="img-city">
      <img src="el-examen/city.jpg" alt="Exercise 2 - City Guide">
    </figure>
  </div>
</section>
CSS
#ej2-city h2 {
  text-align: center;
}

.grid-city {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: auto 1fr;
  gap: 20px;
  margin-inline: 2rem;
}

.img-city {
  grid-column: 2;
  grid-row: 1 / 3;
  margin: 0;
}

.img-city img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.caja-c {
  background-color: lightblue;
  padding: 1rem;
  text-align: left;
}

/* Tablet */
@media (max-width: 1024px) {
  .grid-city {
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: auto auto;
  }
  .img-city {
    grid-column: 1 / -1;
    grid-row: auto;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .grid-city {
    grid-template-columns: 1fr;
  }
}












1. 20261119-LND-UT1-Examen-Tipo-03.pdf
Ejercicio 1 — Colocar justo debajo de <header>
HTML
<section id="ej1-festival">
  <h2>Ejercicio 1 - Music Festival</h2>
  <div class="grid-festival">
    <article class="caja-f3">
      <h3>Concerts</h3>
      <ul>
        <li>Friday night</li>
        <li>Saturday night</li>
        <li>Sunday afternoon</li>
      </ul>
    </article>
    <article class="caja-f3">
      <h3>Artists</h3>
      <ol>
        <li>The Echoes</li>
        <li>Blue Moon</li>
        <li>North Star</li>
      </ol>
    </article>
    <article class="caja-f3 tickets-f3">
      <h3>Tickets</h3>
      <p>Book your festival pass online.</p>
    </article>
  </div>
</section>
CSS
#ej1-festival h2 {
  text-align: center;
}

.grid-festival {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-inline: 2rem;
}

.tickets-f3 {
  grid-column: 1 / -1;
}

.caja-f3 {
  background-color: lightblue;
  padding: 1rem;
}

/* Tablet */
@media (max-width: 1024px) {
  .grid-festival {
    grid-template-columns: repeat(2, 1fr);
  }
  .tickets-f3 {
    grid-column: 2;
  }
  .caja-f3 {
    background-color: lightcoral;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .grid-festival {
    grid-template-columns: 1fr;
  }
  .tickets-f3 {
    grid-column: auto;
  }
  .caja-f3 {
    background-color: lightgreen;
  }
}
Ejercicio 2 — Colocar justo antes de <footer>
HTML
<section id="ej2-nature">
  <h2>Nature Explorer</h2>
  <div class="grid-nature">
    <figure class="img-nature">
      <img src="el-examen/nature.jpg" alt="Nature Explorer">
    </figure>
    <div class="cajas-nature">
      <article class="caja-n">
        <h3>Mountains</h3>
        <p>Discover scenic hiking routes.</p>
      </article>
      <article class="caja-n">
        <h3>Forests</h3>
        <p>Enjoy peaceful woodland walks.</p>
      </article>
      <article class="caja-n">
        <h3>Lakes</h3>
        <p>Relax by the water.</p>
      </article>
    </div>
  </div>
</section>
CSS
#ej2-nature h2 {
  text-align: center;
}

.grid-nature {
  display: grid;
  grid-template-columns: 1.2fr 1fr;
  gap: 20px;
  margin-inline: 2rem;
}

.img-nature {
  margin: 0;
}

.img-nature img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.cajas-nature {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.caja-n {
  background-color: lightblue;
  padding: 1rem;
  text-align: left;
  flex: 1;
}

/* Tablet */
@media (max-width: 1024px) {
  .grid-nature {
    grid-template-columns: 1fr;
  }
  .cajas-nature {
    flex-direction: row;
  }
}

/* Móvil */
@media (max-width: 600px) {
  .cajas-nature {
    flex-direction: column;
  }
}
