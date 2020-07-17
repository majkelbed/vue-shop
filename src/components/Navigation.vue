<template>
  <nav id="nav">
    <div class="flex items-center">
      <span class="flex items-center mr-10">
        <img src="../assets/logo.png" alt="Eco company logo as three trees">
        <h2 class="ml-2 text-2xl text-green-800 font-bold">esaa</h2>
      </span>
      <button class="flex items-center mr-10 fill-current text-orange-500 font-bold">
        <MenuIcon></MenuIcon>
        <p class="ml-2 text-black">
          Categories
        </p>
      </button>
      <div class="flex py-2 px-4 rounded-full bg-gray-200 border focus-within:border-orange-500">
        <label
          class="mr-2 fill-current text-orange-500"
          for="search-product">
          <SearchIcon></SearchIcon>
        </label>
        <input
          class="bg-gray-200 text-gray-900 placeholder-gray-700 outline-none w-64"
          type="text"
          name="search-product"
          id="search-product"
          placeholder="tool for potatos">
      </div>
      <div class="ml-auto">
        <router-link to="/">Home</router-link>
        <router-link to="/contact">Contact</router-link>
      </div>
    </div>
  </nav>
</template>

<style lang="scss">
#nav {
  padding: 30px;
  a {
    margin-left:2rem;
    font-weight: bold;
  }

  .router-link-exact-active {
    text-decoration: underline;
  }
}
</style>

<script>
import Search from '../assets/icons/search.svg';
import Menu from '../assets/icons/menu.svg';

export default {
  name: 'Navigation',
  components: {
    SearchIcon: Search,
    MenuIcon: Menu,
  },
};
</script>
