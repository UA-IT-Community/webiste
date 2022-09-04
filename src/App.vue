<script setup lang="ts">
import { RouterView } from "vue-router";
import { useDark, useToggle, useTitle } from "@vueuse/core";

const isDark = useDark();
const toggleDark = useToggle(isDark);
useTitle("🇺🇦 IT Спільнота");

setTimeout(() => {

  
  console.log(
    `%c
MMMMMMMMMMMMMMMMMMMMMMMMMMWN0d:,...,cd0NWMMMMMMMMM
MMMMMMMMMMMMMMMMMMMMMMWKkdl;.........',:lxXWMMMMMM
MMMMMMMMMMMMMMMMMMWN0dc,..........'''....'c0MMMMMM
MMMMMMMMMMMMMMMWXko;...........''.........'dNMMMMM
MMMMMMMMMMMMN0xc,...........'.............'oNMMMMM
MMMMMMMMMMNkc'.........'..................'oNMMMMM
MMMMMMMMWOc.........''',,''...............'oNMMMMM
MMMMMMMNx,.......''',;',,'................'oNMMMMM
MMMMMMWx'......'.',',,'...................'oNMMMMM
MMMMMMO,......'..''.......................'oNMMMMM
MMMMMNl......'............................'oNMMMMM
MMMMMX:    .''............................'oNMMMMM
MMMMMX:    .'....';lc,'...........'.......'oNMMMMM
MMMMMX:    .'....'cOXKko:,'.......'.......'dNMMMMM
MMMMMX:    .'.....',:dOXXKOl,.....',;,'..';OMMMMMM
MMMMMX:    .'.........,xNMXo'..';cx0Kd,..,dNMMMMMM
MMMMMX:    .'........,dXXOo'':okKX0xl;'',dXMMMMMMM
MMMMMX:    .'.......;xNKl,':kXXOdc,'..';xNMMMMMMMM
MMMMMX:    .'.....';kN0c'..;ll;''..'';oKWMMMMMMMMM
MMMMMX:    .'.....:ONO:'.........';cxKWMMMMMMMMMMM
MMMMMX:    .'....'cxd;'..'...'':okKNMMMMMMMMMMMMMM
MMMMMWd.   .'......''.....',cdOXWMMMMMMMMMMMMMMMMM
MMMMMMNx;. .'........'':ldkKNMMMMMMMMMMMMMMMMMMMMM
MMMMMMMMN0dl:'....',cdOXWMMMMMMMMMMMMMMMMMMMMMMMMM
MMMMMMMMMMMWKo;'';lkXWMMMMMMMMMMMMMMMMMMMMMMMMMMMM
`,
    "font:monospace"
  );
}, 200);
</script>

<template>
  <div class="app">
    <div class="app-header">
      <div>
        <i></i>
        <i></i>
        <i></i>
      </div>
      <div class="toggle">
        <input
          type="checkbox"
          id="toggle"
          :checked="isDark"
          @click="(e) => toggleDark()"
        />
        <label for="toggle" />
      </div>
    </div>

    <div class="app-body">
      <RouterView />
    </div>
  </div>
</template>
