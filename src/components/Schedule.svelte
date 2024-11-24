<script>
  let schedule = [
    { day: "lundi", classes: ["vinyasa 1 - 9h30", "vinyasa 2 - 10h45"] },
    { day: "mardi", classes: ["vinyasa flow - 19h45"] },
    { day: "mercredi", classes: ["yin - 18h"] },
    { day: "jeudi", classes: ["vinyasa 2 - 19h45"] },
    { day: "vendredi", classes: ["yin yang - 13h"] },
  ];
</script>

<div class="schedule">
  <h2>Horaires</h2>
  <ul>
    {#each schedule as { day, classes }}
      <li>
        <span class="day">{day}</span>
        {#each classes as cour}
          <span class="class">{cour}</span>
        {/each}
      </li>
    {/each}
  </ul>
</div>

<style>
  .schedule {
    /* padding: 2rem; */
    /* background-color: var(--background-color); */
    /* border-radius: 8px; */
  }

  h2 {
    font-family: "Libre Caslon Text", serif;
    color: var(--primary-color);
    margin-bottom: 1.5rem;
    text-align: center;
    font-size: 1.7rem;
    font-weight: 400;
    font-style: italic;
    letter-spacing: 0.15rem;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  li {
    margin-bottom: 1rem;
    color: var(--primary-color);
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .day {
    font-weight: bold;
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
    /* margin-right: 0.5rem; */
  }

  .class {
    /* display: block; */
    /* margin-left: 1rem; */
    /* color: #6b5c3f; */
  }
</style>
