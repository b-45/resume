<template>
  <section class="header border-b-2 mb-4">
    <div>
      <img
        class="w-16 h-16 rounded-full"
        src="https://avatars0.githubusercontent.com/u/27720835?s=460&v=4"
      />
    </div>
    <div>
      <div class="name text-2xl font-bold mb-2">Bernard Ade</div>
      <div class="title text-sm font-semibold mb-4">Business Engineer</div>
      <div class="items flex flex-wrap text-xs">
        <div class="email mr-6">
          <font-awesome-icon
            icon="envelope-square"
            class="mr-1"
          />
          <a
            class="no-underline text-blue-dark"
            href="mailto:bernard11ade@gmail.com"
          >bernard11ade@gmail.com
          </a>
        </div>
        <div class="website mr-6">
          <font-awesome-icon
            icon="link"
            class="mr-1"
          />
          <a
            href="http://b-45.com"
            class="no-underline text-blue-dark"
          >www.b-45.com</a>
        </div>
        <div class="location mb-3">
          <font-awesome-icon
            icon="location-arrow"
            class="mr-1"
          />
          Brooklyn, NY</div>
      </div>
    </div>

  </section>
</template>
 


<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 4fr;
  grid-gap: 10px;
}
</style>
 