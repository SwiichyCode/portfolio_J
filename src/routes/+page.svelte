<script>
  import Header from "../libs/Header/Header.svelte";
  import Main from "../libs/Main/Main.svelte";
  import SideLink from "../libs/Global/SideSocial.svelte";
  import SideEmail from "../libs/Global/SideEmail.svelte";
  import { onMount } from "svelte";
  import Popup from "../libs/Global/Popup.svelte";

  const url = "https://api.github.com/users/SwiichyCode/repos";
  let data = [];

  onMount(async () => {
    const response = await fetch(`${url}`);
    const repositories = await response.json();
    data = repositories;
  });
</script>

<div class="container">
  <SideLink />
  <SideEmail />
  <Header />
  <Main />

  {console.log(data)}
</div>

<style>
  .container {
    width: 100%;
    height: auto;
    transition: all 200ms ease-in-out;
    background-color: #0a192f;
    overflow: hidden;
  }
</style>
