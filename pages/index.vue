<template>
  <div class="bg-gray-100 min-h-screen">
    <div class="flex items-top justify-center sm:items-center sm:pt-0">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 my-8 my-4 lg:my-8">
        <a class="flex justify-center sm:pt-0" href="/" target="_blank">
          <img src="/logo_pwit.svg" alt="logo">
        </a>
        <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
          <h2 class="text-2xl leading-7 font-semibold">
            Palmlund Wahlgren Innovative Technology AB
          </h2>
          <p class="mt-3 text-gray-600">
            Python experts using open source technologies to solve real problems.
          </p>
          <p class="mt-4 pt-4  text-center text-gray-800 border-t border-dashed">

            info@pwit.se <br><br>
            Håstenslöv 1588<br>
            268 72 Teckomatorp <br>
            Sweden
          </p>
        </div>
        <div class="flex justify-center pt-4 space-x-2">
          <a href="https://github.com/pwitab" target="_blank">
            <svg
              class="w-6 h-6 text-gray-600 hover:text-gray-800"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              aria-hidden="true"
              role="img"
              width="32"
              height="32"
              preserveAspectRatio="xMidYMid meet"
              viewBox="0 0 24 24"
            >
              <path
                d="M12 2.247a10 10 0 0 0-3.162 19.487c.5.088.687-.212.687-.475c0-.237-.012-1.025-.012-1.862c-2.513.462-3.163-.613-3.363-1.175a3.636 3.636 0 0 0-1.025-1.413c-.35-.187-.85-.65-.013-.662a2.001 2.001 0 0 1 1.538 1.025a2.137 2.137 0 0 0 2.912.825a2.104 2.104 0 0 1 .638-1.338c-2.225-.25-4.55-1.112-4.55-4.937a3.892 3.892 0 0 1 1.025-2.688a3.594 3.594 0 0 1 .1-2.65s.837-.262 2.75 1.025a9.427 9.427 0 0 1 5 0c1.912-1.3 2.75-1.025 2.75-1.025a3.593 3.593 0 0 1 .1 2.65a3.869 3.869 0 0 1 1.025 2.688c0 3.837-2.338 4.687-4.563 4.937a2.368 2.368 0 0 1 .675 1.85c0 1.338-.012 2.413-.012 2.75c0 .263.187.575.687.475A10.005 10.005 0 0 0 12 2.247z"
                fill="currentColor"/>
            </svg>
          </a>
        </div>
      </div>
    </div>
    <div id="side-projects" class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 my-8 my-4 lg:my-8">
      <div class="text-center my-4">
        <h3 class="text-2xl leading-7 font-semibold">
          Side Projects
        </h3>
      </div>

      <div class="flex flex-col sm:flex-row justify-evenly">

        <SideProjectCard logo_path="/utilitarian_logo_on_light.svg"><p>
          We offer our smart metering related services and products under the name Utilitarian.
        </p>
          <p>With several years of experience in Smart Metering we built a multi-utility AMR system as we wanted it to
            work</p>
          <p>We offer our AMR system and our services to utility companies and other service provider in the Smart
            Metering
            sector.</p>
        </SideProjectCard>
        <SideProjectCard logo_path="/holundergarden_logo_black.svg">
          <p>
            Sitting in front of a computer all day, every day is not healthy. We also run a small scale farm producing
            chemical free veggies, honey and eggs. This gives us some time to reflect on coding problems and the
            physical
            work keeps us healthy.
          </p>
          <p class="mt-2">
            All our internal farm/business support tools are of course built using Python
          </p>
        </SideProjectCard>


      </div>
    </div>
  </div>

</template>

<script lang="ts">
import Vue from 'vue'
import SideProjectCard from "~/components/SideProjectCard.vue";

export default Vue.extend({
  components: {SideProjectCard}
})
</script>
