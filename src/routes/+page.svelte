<script lang="ts">
  let data: Array<any> = Array(5);

  data.fill({
    body: "Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.",
    cim10: ["infactus", "rhume", "fracture"],
  });
</script>

{#each data as item}
  <div class="flex space-x-1 items-start m-5">
    <label class="">
      <input class="checkbox" type="checkbox" checked />
    </label>
    <div class="flex-col">
      <h2 class="text-primary-500 font-bold">Compte rendu de Rhumatologie</h2>
      <div>
        {#each item.cim10 as i}
          <!-- content here -->
          <span class="badge variant-filled m-1">{i}</span>
        {/each}
      </div>
      <p>{item.body}</p>
    </div>
  </div>
{/each}
