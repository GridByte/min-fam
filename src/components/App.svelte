
<script>  
  import MainView from './MainView.svelte';
</script>

<main>
  <div class="root__navbar"> 
    <div class="top-text">
      Gaute Aasmo 3STH - Min familie
    </div>
  </div>
  <div class="root__sidebar">
    
  </div>
  <div class="root__main_view">
    <MainView/>
  </div>
</main>

<style>
  main {
    width: 100%;
    height: 100%;
    padding: 0;
    display: grid;
    grid-template-areas: 
    "navbar navbar"
    "sidebar main_view";
    grid-template-columns: 0px 200fr;
		grid-template-rows: 75px 1fr;
  }

  .root__navbar {
    grid-area: navbar;
    background-color: rgb(24, 24, 24);
  }

  .root__sidebar {
    grid-area: sidebar;
    background-color: green;
  }
  
  .root__main_view {
    grid-area: main_view;
    background-color: rgb(75, 80, 75);
  }

  .top-text {
    color: white;
    opacity: 1;
    widows: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>
