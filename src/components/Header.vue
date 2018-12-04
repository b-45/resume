<template>
  <section class="header border-b-2 mb-4">
    <div></div>
    <div>
      <div class="name text-2xl font-bold mb-2">Bernard Ade</div>
      <div class="title text-sm font-semibold mb-2">Business Engineer</div>
      <div class="items flex text-xs">
        <div class="email mr-2">
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
        <div class="website mr-2">
          <font-awesome-icon
            icon="link"
            class="mr-1"
          />
          <a
            href="http://b-45.com"
            class="no-underline text-blue-dark"
          >www.b-45.com</a>
        </div>
        <div class="location mb-2">
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
}
</style>
 