<script>
  import svelteLogo from "./assets/svelte.svg";
  import CondicionalIf from "./components/CondicionalIf.svelte";
  import SpecialTags from "./components/SpecialTags.svelte";
  import LogicEach from "./components/LogicEach.svelte";
  import Reactive from "./components/Reactive.svelte";
  import State from "./components/State.svelte";
  import Await from "./components/Await.svelte";
  import Transitions from "./components/Transitions.svelte";
    import Key from "./components/Key.svelte";
    import Widtget from "./layout/Widtget.svelte";
    import Card from "./layout/Card.svelte";
    import Slot from "./layout/Slot.svelte";
    import FancyList from "./layout/FancyList.svelte";
    import Self from "./layout/Self.svelte";
</script>

<main>
  <Widtget>
    <p>Contenido adicional</p>
  </Widtget>
  <div>
    <a href="https://svelte.dev" target="_blank" rel="noreferrer">
      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
    </a>
    <CondicionalIf />
    <LogicEach />
    <State />
    <Reactive />
    <SpecialTags />
    <Await />
    <Transitions />
    <Key/>
    <Self/>
  </div>

  <Card>
    <svelte:fragment slot="footer">

    <p>All rights reserved.</p>
		<p>Copyright &copy; 2019 Svelte Industries</p>

    </svelte:fragment>
  </Card>

  <Slot>
    <h1 slot="title">Blog Post Title</h1>
  </Slot>

  <FancyList>
    <div slot="item" let:item>{item.title}</div>
    <p slot="footer">Copyright (c) 2019 Svelte Industries</p>
  </FancyList>
    
</main>


<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
</style>
