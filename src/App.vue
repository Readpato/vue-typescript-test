<script setup lang="ts"></script>

<template>
  <main
    class="w-screen h-screen bg-purple-400 flex justify-center items-center flex-col space-y-2"
  >
    <h1 class="text-3xl text-white">Friends Form</h1>
    <form
      class="flex flex-col space-y-2 border-2 border-yellow-200 p-8 back text-white bg-gradient-to-br from-yellow-300/40 to-orange-300/40"
    >
      <label for="friend-name">Insert friend name</label>
      <input type="text" id="friend-name" class="text-black p-1" />
      <label for="friend-surname ">Insert friend surname</label>
      <input type="text" id="friend-surname" class="text-black p-1" />
      <label for="friend-age">Insert friend age</label>
      <input type="number" id="friend-age" class="text-black p-1" />
      <h2>Do you like this friend</h2>
      <div class="flex space-x-2 items-center justify-center text-center">
        <input
          type="radio"
          id="friend-favorite"
          name="favorite-group"
          :value="false"
        />
        <label for="friend-favorite">Yes</label>
        <input
          type="radio"
          id="friend-favorite"
          name="favorite-group"
          :value="false"
        />
        <label for="friend-favorite">No</label>
      </div>
      <button
        @click.prevent
        class="border-2 border-yellow-400 p-2 bg-yellow-400 text-purple-500"
      >
        Submit new Friend
      </button>
    </form>
  </main>
</template>
