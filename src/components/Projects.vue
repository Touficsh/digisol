<template>
  <div class="projects-2 project-raised">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 ml-auto mr-auto text-center mb-5">
          <h2 class="title">Some of Our Projects</h2>
          <div class="section-space"></div>
        </div>
      </div>
      <ul
        class="nav nav-pills nav-pills-primary nav-pills-icons nav-pills-lg"
        role="tablist"
      >
        <li class="nav-item m-auto">
          <a
            class="nav-link active"
            data-toggle="tab"
            role="tablist"
            @click="setProjectNumber(0)"
          >
            <i class="tim-icons icon-bag-16"></i>
             961 Home
          </a>
        </li>
        <li class="nav-item m-auto">
          <a
            class="nav-link"
            data-toggle="tab"
            role="tablist"
            @click="setProjectNumber(1)"
          >
            <i class="tim-icons icon-puzzle-10"></i> Orenda Clinic
          </a>
        </li>
        <li class="nav-item m-auto">
          <a
            class="nav-link"
            data-toggle="tab"
            role="tablist"
            @click="setProjectNumber(2)"
            >
            <i class="tim-icons icon-components"></i> The avenues
          </a>
        </li>
        <li class="nav-item m-auto">
          <a
            class="nav-link"
            data-toggle="tab"
            role="tablist"
            @click="setProjectNumber(3)"
          >
            <i class="tim-icons icon-wifi"></i> Sodetel
          </a>
        </li>
        <li class="nav-item mx-auto">
          <a
            class="nav-link"
            data-toggle="tab"
            role="tablist"
            @click="setProjectNumber(4)"
          >
            <i class="tim-icons icon-mobile"></i> Treetz
          </a>
        </li>
      </ul>
      <div class="tab-content tab-space">
        <div v-for="(item, index) in projects" :key="index">
          <div
             v-if="index === projectNumber"
            class="tab-pane active"
          >
            <div class="col-lg-12 mt-2">
              <div class="row mt-2">
                <div class="col-md-12">
                  <div class="card card-blog">
                    <div class="card-body text-left">
                      <div class="card-footer mt-0">
                        <img class="abc"  :src="item.imgURL" />
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue' ;

const projectNumber = ref(0);
const test = ref('../../src/assets/img/projects/961.jpg');

const projects = reactive([
  {
    name: '961 Home',
    imgURL: '../../src/assets/img/projects/961.jpg',
  },
  {
    name: 'Orenda Clinic',
    imgURL: '../../src/assets/img/projects/orenda_clinic.jpg',
  },
  {
    name: 'The avenues',
    imgURL: '../../src/assets/img/projects/avenues.jpg',
  },
  {
    name: 'Sodetel',
    imgURL: '../../src/assets/img/projects/sodetel.jpg',
  },
  {
    name: 'Treetz',
    imgURL: '../../src/assets/img/projects/Treetz.jpg',
  },
]);

function setProjectNumber(number) {
  projectNumber.value = number;
}

</script>

<style scoped>
.abc {
  min-height: 200px !important;
}
</style>
