
<body>
    
  <section class="bg-emerald-400">
    
    <h1>Nice Curves</h1>
    <p>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Deserunt
      accusamus provident soluta corrupti delectus non vitae nisi molestiae,
      inventore animi ea eaque rerum modi blanditiis a recusandae minima dolore
      quasi?
    </p>
    <div class="wave">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
            <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
        </svg>
    </div>
  </section>
  <section class="bg-emerald-800">
    <h1>Nice Curves</h1>
    <p>
      Beatae cum eum, accusamus consectetur necessitatibus dignissimos ex minus
      ullam nobis adipisci? Nisi aspernatur optio facere atque magni, esse
      consequatur natus, recusandae modi nemo, odit in veniam culpa possimus
      magnam.
    </p>

  </section>
  <section class="red">
    <h1>Nice Curves</h1>
    <p>
      Vero eveniet, saepe a natus doloribus officiis aperiam placeat quisquam
      maxime modi maiores non quos distinctio labore autem neque, quae eos
      laboriosam deserunt quis ducimus iure recusandae? Veniam, deserunt
      officia?
    </p>
  </section>
 
</body>

<style>
  body {
    margin: 0;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    color: white;
    background: #202731;
  }
  section {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 400px;
    padding: 100px 20vw;
  }

  .wave {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.wave svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 150px;
}

.wave .shape-fill {
    fill: #065f46;
}
 
</style>
