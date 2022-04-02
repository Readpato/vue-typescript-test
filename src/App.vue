<script setup lang="ts"></script>

<template>
  <main
    class="w-screen h-screen bg-purple-400 flex justify-center items-center flex-col space-y-2 text-white"
  >
    <h1 class="text-2xl">Friends Form</h1>
    <form class="flex flex-col space-y-2 border-2 border-yellow-400 p-8 back">
      <label for="friend-name">Insert friend name</label>
      <input type="text" id="friend-name" />
      <label for="friend-surname">Insert friend surname</label>
      <input type="text" id="friend-surname" />
      <label for="friend-age">Insert friend age</label>
      <input type="number" id="friend-age" />
      <h2>Do you like this friend</h2>
      <div class="flex space-x-2 items-center justify-center text-center">
        <input type="radio" id="friend-favorite" name="favorite-group" />
        <label for="friend-favorite">Yes</label>
        <input type="radio" id="friend-favorite" name="favorite-group" />
        <label for="friend-favorite">No</label>
      </div>
      <button @submit.prevent>Submit new Friend</button>
    </form>
  </main>
</template>
