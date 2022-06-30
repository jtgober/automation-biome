<script context="module">
  // @ts-ignore
  export async function load({ fetch, params }) {
    const id = params.id;
    const res = await fetch(`https://jsonplaceholder.typicode.com/users/${id}`);
    const userName = await res.json();

    if (res.ok) {
      return {
        props: {
          userName,
        },
      };
    }
    return {
      status: res.status,
      error: new Error("Could not fetch"),
    };
  }
</script>

<script>
  export /**
   * @type {{ name: any, email:any }}
   */
  let userName;
</script>

<div class="guide">
  <h2>{userName.name}</h2>
  <p>{userName.email}</p>
</div>

<style>
  .guide {
    margin-top: 40px;
    padding: 10px;
    border: 1px dotted rgba(255, 255, 255, 0.2);
  }
</style>
