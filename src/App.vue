<script setup>
  import {
    data
  } from "./data/data"
  const teams = [{
      name: "John Doe",
      designation: "Web Designer",
      image: "https://source.unsplash.com/random/300x200?1",
      profileLink: "https://unsplash.com/photos/a-vase-filled-with-lots-of-flowers-on-top-of-a-table-LTw2ld-5q4M"
    },
    {
      name: "Jane Doe",
      designation: "Web Designer",
      image: "https://source.unsplash.com/random/300x200?2",
      profileLink: "https://www.pexels.com/photo/pink-flower-in-close-up-photography-8311903/"
    },
    {
      name: "Jiniya Doe",
      designation: "Web Designer",
      image: "https://source.unsplash.com/random/300x200?3",
      profileLink: "https://www.pexels.com/photo/landscape-photography-of-the-river-seine-13988101/"
    },
  ];
  const singleMember = {
    name: "John Doe",
    designation: "Web Designer",
    image: "https://source.unsplash.com/random/300x200?1",
    profileLink: "https://unsplash.com/photos/a-vase-filled-with-lots-of-flowers-on-top-of-a-table-LTw2ld-5q4M"
  }
</script>

<template>
  <div class="card">
    <div class="card-header">
      {{ data.title }}
    </div>
    <div class="card-body">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <div class="card" style="width:20rem;margin:20px 0 24px 0">
              <img class="card-img-top" :src="teams[0].image" alt="image" style="width:100%">
              <div class="card-body">
                <h4 class="card-title">{{ teams[0].name }}</h4>
                <p class="card-text">{{ teams[0].designation }}</p>
                <a :href="teams[0].profileLink" class="btn btn-primary">See Profile</a>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card" style="width:20rem;margin:20px 0 24px 0">
              <img class="card-img-top" :src="teams[1].image" alt="image" style="width:100%">
              <div class="card-body">
                <h4 class="card-title">{{ teams[1].name }}</h4>
                <p class="card-text">{{ teams[1].designation }}</p>
                <a :href="teams[1].profileLink" class="btn btn-primary">See Profile</a>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card" style="width:20rem;margin:20px 0 24px 0">
              <img class="card-img-top" :src="teams[2].image" alt="image" style="width:100%">
              <div class="card-body">
                <h4 class="card-title">{{ teams[1].name }}</h4>
                <p class="card-text">{{ teams[1].designation }}</p>
                <a :href="teams[1].profileLink" class="btn btn-primary">See Profile</a>
              </div>
            </div>
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2 class="text-center">Single Member</h2>
            <div class="card" style="width:20rem;margin:20px 0 24px 0">
              <img class="card-img-top" :src="singleMember.image" alt="image" style="width:100%">
              <div class="card-body">
                <h4 class="card-title">{{ singleMember.name }}</h4>
                <p class="card-text">{{ singleMember.designation }}</p>
                <a :href="singleMember.profileLink" class="btn btn-primary">See Profile</a>
              </div>
            </div>
          </div>
        </div> 

      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
