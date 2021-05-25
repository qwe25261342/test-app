<template>
  <header>
    <div class="box">
      <a href="/">
        <img src="../assets/img/logo.png" alt="" class="logo" />
      </a>
      <div class="searchbox">
        <input type="text" />
        <button>
          <img src="../assets/img/search.png" alt="" class="search" />
        </button>
      </div>
      <a href="" class="avatarbox">
        <button>
          <img src="../assets/img/user.png" alt="" class="user" />
        </button>
      </a>
    </div>
  </header>
</template>
<script>
import { BIcon, BIconArrowUp, BIconArrowDown } from "bootstrap-vue";

export default {
  components: {
    BIcon,
    BIconArrowUp,
    BIconArrowDown,
  },
};
</script>