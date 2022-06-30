<script context="module">
  // @ts-ignore
  export async function load({ fetch }) {
    const res = await fetch("https://jsonplaceholder.typicode.com/users");
    const userNames = await res.json();

    if (res.ok) {
      return {
        props: {
            userNames,
        },
      };
    }
    return {
      status: res.status,
      error: new Error('Could not fetch')
    };
  }
</script>

<script>
import LayoutGuides from "./guides/__layout-guides.svelte";


  
    export /**
* @type {any}
*/
     let userNames
</script>

<div class="userNames">
    <ul>
        {#each userNames as userName}
        <li>
            <a href={`/guides/${userName.id}`}>{userName.name}</a>
        </li>

        {/each}
    </ul>
</div>

<style>

</style>
