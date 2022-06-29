<script context="module">
  // @ts-ignore
  export async function load({ fetch }) {
    const res = await fetch("https://jsonplaceholder.typicode.com/users");
    const guides = await res.json();

    if (res.ok) {
      return {
        props: {
          guides,
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
  
    export /**
* @type {any}
*/
     let guides
</script>

<div class="guides">
    <ul>
        {#each guides as guide}
        <li>
            <a href="/">{guide.name}</a>
        </li>

        {/each}
    </ul>
</div>

<style>

</style>
