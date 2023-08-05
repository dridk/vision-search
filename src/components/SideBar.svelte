<script lang="ts">
  import { ListBox, ListBoxItem } from "@skeletonlabs/skeleton";
  let valueSingle: string = "books";
</script>

<ListBox class="w-60 h-full border-r border-gray-500">
  <ListBoxItem bind:group={valueSingle} name="medium" value="books"
    >Prescripteur</ListBoxItem
  >
  <ListBoxItem bind:group={valueSingle} name="medium" value="movies"
    >Ages</ListBoxItem
  >
  <ListBoxItem bind:group={valueSingle} name="medium" value="tv"
    >Date</ListBoxItem
  >
</ListBox>
