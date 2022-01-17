<script>
  let dropdownActive = false;
</script>

<main class="h-full">
  <div class="hero">
    <div
      class="hero-body is-fluid is-justify-content-center is-align-content-center "
    >
      <figure class="image">
        <img
          class="profile-img is-rounded"
          src="/images/Profile.jpg"
          alt="profile"
        />
      </figure>
      <h2 class="is-size-1">Tyler Mayoff</h2>
      <div>
        <a class="button " href="https://github.com/tmayoff">Github</a>
        <a class="button " href="https://github.com/tmayoff">LinkedIn</a>
      </div>
    </div>
  </div>

  <div class="bg-sky-600 h-full p-3 mt-3">
    <div class="dropdown" class:is-active={dropdownActive}>
      <div class="dropdown-trigger">
        <button
          class="button is-outlined"
          aria-haspopup="true"
          aria-controls="dropdown-menu"
          on:click={() => (dropdownActive = !dropdownActive)}
        >
          <span class="navbar-item has-dropdown is-size-4">
            <ion-icon name="menu" />
          </span></button
        >
      </div>

      <div class="dropdown-menu">
        <div class="dropdown-content">
          <a
            class="dropdown-item"
            href="#technical-skills"
            on:click={() => (dropdownActive = false)}>Technical Skills</a
          >
        </div>
      </div>
    </div>

    <h1 class="is-size-3" id="technical-skills">Technical Skills</h1>
  </div>
</main>

<style lang="scss">
  .profile-img {
    height: 450px !important;
    width: auto;
    margin: auto;
  }

  .button {
    background: transparent;
    border-color: rgb(0.2, 0.2, 0.2);
  }

  .hero {
    text-align: center;
  }

  .h-full {
    height: 100%;
  }

  .bg-sky-600 {
    background-color: #8bddd8;
    color: black;
  }
</style>
