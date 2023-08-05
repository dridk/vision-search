<script>
  // Your selected Skeleton theme:
  import "@skeletonlabs/skeleton/themes/theme-rocket.css";

  // This contains the bulk of Skeletons required styles:
  import "@skeletonlabs/skeleton/styles/skeleton.css";

  import "../app.css";

  import { AppShell } from "@skeletonlabs/skeleton";
  import Header from "../components/Header.svelte";
  import SideBar from "../components/SideBar.svelte";
</script>

<AppShell>
  <svelte:fragment slot="header"><Header /></svelte:fragment>
  <svelte:fragment slot="sidebarLeft"><SideBar /></svelte:fragment>
  <!-- (sidebarRight) -->
  <slot />
  <!-- ---- / ---- -->
  <svelte:fragment slot="pageFooter">Page Footer</svelte:fragment>
  <!-- (footer) -->
</AppShell>

<slot />
