<script lang="ts">
  import halfmoon from "halfmoon/js/halfmoon-module";
  import Icon from "fa-svelte";
  import { faMoon } from "@fortawesome/free-regular-svg-icons";

  import Button from "../../halfmoon/BasicElements/Button.svelte";
  import Navbar from "../../halfmoon/BuildingBlocks/Navbar/Navbar.svelte";
  import NavbarItem from "../../halfmoon/BuildingBlocks/Navbar/NavbarItem.svelte";
</script>

<Navbar>
  <NavbarItem href="/">Tasks</NavbarItem>
  <NavbarItem href="/archive">Archive</NavbarItem>
  <NavbarItem className="ml-auto">
    <Button onClick={() => halfmoon.toggleDarkMode()}>
      <Icon icon={faMoon} />
    </Button>
  </NavbarItem>
</Navbar>
