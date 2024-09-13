<script setup>
import { reactive, ref, } from 'vue'
const isOverlayOpen = ref(false)

const folderName = ref("");
const setDetail = (name) => {
  folderName.value = name;
  toggleOverlay();
}
const thumbnails = reactive([
  {
    imgSrc: 'kuva-28',
    title: 'kuva logo and brand identify design',
    subTitle: 'Agency Brandie',
    like: 200,
    view: 2000
  },
  {
    imgSrc: 'kizo-29',
    title: 'kuva logo and brand identify design',
    subTitle: 'Agency Brandie',
    like: 200,
    view: 2000
  },
  {
    imgSrc: 'latte-6',
    title: 'kuva logo and brand identify design',
    subTitle: 'Agency Brandie',
    like: 200,
    view: 2000
  },
  {
    imgSrc: 'tree-45',
    title: 'kuva logo and brand identify design',
    subTitle: 'Agency Brandie',
    like: 200,
    view: 2000
  }
])
const getDetailImage = () => {
  const length = folderName.value.split('-')[1]
  let arr = []
  for (let i = 1; i <= length; i++) {
    arr.push(`/assets/images/${folderName.value}/${i}.png`)
  }
  return arr
}
const toggleOverlay = () => {
  isOverlayOpen.value = !isOverlayOpen.value;
}

</script>
<template>
  <header class="relative">
    <!-- Top Half: Black Background -->
    <div class="h-[120px] w-full bg-black flex justify-end">
      <!-- <span class="word-art word-art-position">Everything is Designed !!</span> -->
      <img src="/assets/images/bia.png" alt="Logo" />
    </div>
    <div class="logo">
      <router-link to="/"> <img src="/assets/images/Avt.png" alt="Logo" /></router-link>
    </div>
    <!-- Moved Logo to the Left -->

  </header>

  <body class="px-[10%] md:px-[10%] min-h-screen items-center justify-center bg-white">
      <div class="mx-auto sm:block md:flex p-4">
      <!-- Sidebar -->
      <div class="w-[100%] md:w-[350px] sm:m-auto  text-white text-center md:text-left">

        <div class="max-w-sm bg-white p-6">
          <div class="text-black text-2xl font-bold">Agency Brandie</div>
          <!-- Status -->
          <div
            class="px-3 py-2 w-fit flex text-sm bg-green-100 items-center rounded-xl m-auto md:m-0 md:mx-0 md:my-2 md:mb-4 ">
            <span class="mr-1 h-1 w-1 rounded-full bg-green-500"></span>
            <span class="text-green-300 font-semibold	">Available Now</span>
          </div>

          <!-- Profile Info -->
          <div>
            <p class="text-sm text-black flex md:items-start sm:items-center">
            <div class="icon-style">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                aria-labelledby="IconBase-title-4dbb2be7-c8ac-4bb5-a474-b805a6c650bd IconBase-description-4dbb2be7-c8ac-4bb5-a474-b805a6c650bd"
                role="graphics-symbol img" width="100%" height="100%" class="ProfileCard-infoIcon-wVi">
                <title id="IconBase-title-4dbb2be7-c8ac-4bb5-a474-b805a6c650bd">Info</title>
                <desc id="IconBase-description-4dbb2be7-c8ac-4bb5-a474-b805a6c650bd"></desc>
                <g><!--[-->
                  <path
                    d="M11.875,14.375H11.25A1.877,1.877,0,0,1,9.375,12.5V9.375H8.75a.625.625,0,0,1,0-1.25h.625a1.251,1.251,0,0,1,1.25,1.25V12.5a.626.626,0,0,0,.625.625h.625a.625.625,0,0,1,0,1.25Z">
                  </path>
                  <path d="M9.687,6.875a.938.938,0,1,1,.938-.937A.939.939,0,0,1,9.687,6.875Z"></path>
                  <path
                    d="M10,0A10,10,0,1,1,0,10,10.011,10.011,0,0,1,10,0Zm0,18.75A8.75,8.75,0,1,0,1.25,10,8.76,8.76,0,0,0,10,18.75Z">
                  </path><!--]-->
                </g>
              </svg>
            </div>
            <span class="ml-1 inline-block">Agency thiết kế Logo & Bộ nhận diện thương hiệu</span>
            </p>

            <p class="font-medium text-black"><a href="mailto:eidaamin.work@gmail.com">
                <div class="icon-style">
                  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1234.27 1080"
                    aria-labelledby="IconBase-title-f03eec97-82d0-416d-b7e7-dd7b45427661 IconBase-description-f03eec97-82d0-416d-b7e7-dd7b45427661"
                    role="graphics-symbol img" width="100%" height="100%" class="ProfileCard-briefcaseIcon-W5P"
                    fill="#707070">
                    <title id="IconBase-title-f03eec97-82d0-416d-b7e7-dd7b45427661">Briefcase</title>
                    <desc id="IconBase-description-f03eec97-82d0-416d-b7e7-dd7b45427661"></desc>
                    <g><!--[-->
                      <g>
                        <g>
                          <path
                            d="m1092.75,1080H141.52c-78.03,0-141.52-63.48-141.52-141.52V372.88c0-78.04,63.49-141.52,141.52-141.52h951.23c78.03,0,141.52,63.48,141.52,141.52v565.59c0,78.04-63.49,141.52-141.52,141.52ZM141.52,308.8c-35.33,0-64.08,28.75-64.08,64.08v565.59c0,35.33,28.74,64.08,64.08,64.08h951.23c35.33,0,64.08-28.74,64.08-64.08V372.88c0-35.33-28.74-64.08-64.08-64.08H141.52Z">
                          </path>
                        </g>
                        <g>
                          <path
                            d="m848.5,308.81c-21.38,0-38.72-17.34-38.72-38.72,0-106.22-86.42-192.65-192.64-192.65s-192.64,86.42-192.64,192.65c0,21.38-17.33,38.72-38.72,38.72s-38.72-17.34-38.72-38.72c0-72.14,28.09-139.97,79.1-190.98S544.99,0,617.13,0s139.97,28.09,190.98,79.11c51.01,51.01,79.11,118.84,79.11,190.98,0,21.38-17.34,38.72-38.72,38.72Z">
                          </path>
                        </g>
                        <g>
                          <path
                            d="m501.45,617.27H38.72C17.34,617.27,0,599.93,0,578.55s17.33-38.72,38.72-38.72h462.73c21.38,0,38.72,17.34,38.72,38.72s-17.33,38.72-38.72,38.72Z">
                          </path>
                        </g>
                        <g>
                          <path
                            d="m1195.55,617.27h-462.73c-21.39,0-38.72-17.34-38.72-38.72s17.33-38.72,38.72-38.72h462.73c21.38,0,38.72,17.34,38.72,38.72s-17.34,38.72-38.72,38.72Z">
                          </path>
                        </g>
                        <g>
                          <path
                            d="m617.13,784.29c-41.21,0-79.96-16.04-109.12-45.17-29.18-29.15-45.25-67.92-45.28-109.16v-61.7c.04-85.07,69.27-154.3,154.33-154.35h.08c85.11,0,154.36,69.21,154.4,154.33v61.7c-.04,85.07-69.27,154.3-154.33,154.34h-.08Zm-76.96-154.37c.01,20.56,8.03,39.88,22.57,54.41,14.53,14.52,33.85,22.51,54.39,22.51h.04c42.39-.02,76.9-34.53,76.93-76.92v-61.66c-.02-42.42-34.57-76.93-77-76.9-42.39.02-76.9,34.53-76.92,76.92v61.64Z">
                          </path>
                        </g>
                      </g><!--]-->
                    </g>
                  </svg>
                </div>
                agencybrandie@gmail.com
              </a></p>
            <p class="text-gray-600">
            <div class="icon-style">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                aria-labelledby="IconBase-title-df59dbea-af75-46ea-8a7a-f675cacb836f IconBase-description-df59dbea-af75-46ea-8a7a-f675cacb836f"
                role="graphics-symbol img" width="100%" height="100%" class="ProfileCard-globeIcon-v6R"
                stroke="#707070">
                <title id="IconBase-title-df59dbea-af75-46ea-8a7a-f675cacb836f">Globe Grid</title>
                <desc id="IconBase-description-df59dbea-af75-46ea-8a7a-f675cacb836f">Globe with grid lines</desc>
                <g><!--[-->
                  <g transform="translate(-51.999)">
                    <rect width="20" height="20" transform="translate(51.999)" fill="none" stroke="none"></rect>
                    <g transform="translate(53.999 2)">
                      <path d="M.362,8.362a8,8,0,1,0,8-8,8,8,0,0,0-8,8" transform="translate(-0.362 -0.362)" fill="none"
                        stroke-linecap="round" stroke-linejoin="round" stroke-width="1.15"></path>
                      <path d="M5.371,16.163C4.255,14.6,3.5,11.662,3.5,8.341S4.255,2.012,5.371.483"
                        transform="translate(1.121 -0.305)" fill="none" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="1.15"></path>
                      <path d="M6.819,16.163c1.116-1.564,1.87-4.5,1.87-7.822S7.935,2.012,6.819.483"
                        transform="translate(2.689 -0.305)" fill="none" stroke-linecap="round" stroke-linejoin="round"
                        stroke-width="1.15"></path>
                      <path d="M.362,5.8h16" transform="translate(-0.362 2.205)" fill="none" stroke-linecap="round"
                        stroke-linejoin="round" stroke-width="1.15"></path>
                      <path d="M.99,8.33H15.141" transform="translate(-0.066 3.403)" fill="none" stroke-linecap="round"
                        stroke-linejoin="round" stroke-width="1.15"></path>
                      <path d="M.99,3.26H15.141" transform="translate(-0.066 1.007)" fill="none" stroke-linecap="round"
                        stroke-linejoin="round" stroke-width="1.15"></path>
                    </g>
                  </g><!--]-->
                </g>
              </svg>
            </div>
            Tòa R6 Royal City, Thanh Xuân, Hà Nội</p>
            <p>
            <div class="icon-style">
              <svg xmlns="http://www.w3.org/2000/svg" width="16px" height="14px" viewBox="0 0 24 24" fill="black" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
  <path d="M22 16.92V21a2 2 0 0 1-2.18 2A19.88 19.88 0 0 1 2 5.18 2 2 0 0 1 4 3h4.09a2 2 0 0 1 2 1.72 12.05 12.05 0 0 0 .57 2.57 2 2 0 0 1-.45 2.11L8.91 10.91a16 16 0 0 0 6.59 6.59l1.51-1.51a2 2 0 0 1 2.11-.45 12.05 12.05 0 0 0 2.57.57 2 2 0 0 1 1.72 2.01z"/>
</svg>

            </div>
            <a  class="text-black ml-1">0868379318</a>
            </p>
          </div>

          <!-- Hire Options -->
          <!-- <div class="mt-6 text-black border-solid border-2 border-gray-100 rounded-sm p-3 hidden-mobile">
            <div class="pb-2 justify-start text-md font-semibold border-solid border-b-2 border-gray-100">Hire Eid A
              Amin</div>
            <div class="space-y-2">
              <div class="flex items-center  justify-between py-2 border-b-2 border-gray-100">
                <a href="#" class=" hover:bg-gray-50">
                  <div class="icon-style-large blue-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 19.997 20"
                      class="AvailabilityInfoCard-leadingIcon-jcE">
                      <g transform="translate(-778.375 0.625)">
                        <g transform="translate(779 0)">
                          <path
                            d="M9.014,9.869a2.535,2.535,0,0,1,1.722.672q.019.017.036.036a2.542,2.542,0,0,1-.1,3.544c-.833.827-3.71,1.418-4.279,1.528a.625.625,0,0,1-.732-.733c.111-.569.7-3.443,1.528-4.277A2.521,2.521,0,0,1,9.014,9.869Zm.856,1.574a1.292,1.292,0,0,0-1.784.069l-.007.007a8.39,8.39,0,0,0-.984,2.7,8.361,8.361,0,0,0,2.7-.983l.008-.008A1.284,1.284,0,0,0,9.87,11.443Z"
                            transform="translate(-0.625 -0.623)"></path>
                          <path
                            d="M10.608,5.265A.625.625,0,0,1,10.166,4.2L13.2,1.166a1.85,1.85,0,0,1,2.616,0l.867.867a.625.625,0,0,1-.884.884l-.867-.867a.6.6,0,0,0-.849,0L11.05,5.082A.623.623,0,0,1,10.608,5.265Z"
                            transform="translate(-0.625 -0.623)"></path>
                          <path
                            d="M11.907,12.629a.623.623,0,0,1-.442-.183l-2.6-2.6a.625.625,0,0,1,0-.884L15.8,2.032a2.463,2.463,0,0,1,3.484,3.482l-6.933,6.932A.623.623,0,0,1,11.907,12.629ZM10.192,9.4l1.715,1.715L18.4,4.631a1.222,1.222,0,0,0,0-1.717,1.218,1.218,0,0,0-1.715,0Z"
                            transform="translate(-0.625 -0.623)"></path>
                          <path
                            d="M16.24,8.3a.623.623,0,0,1-.442-.183l-2.6-2.6a.625.625,0,0,1,.884-.884l2.6,2.6A.625.625,0,0,1,16.24,8.3Z"
                            transform="translate(-0.625 -0.623)"></path>
                          <path
                            d="M15.054,20H.937a.937.937,0,0,1-.663-1.6l.5-.5c1.368-1.368,1.36-2.269,1.308-8.134-.011-1.305-.024-2.785-.024-4.569A6.329,6.329,0,0,1,4.506.4c.1-.087.179-.163.235-.218A.625.625,0,0,1,5.183,0H8.89a.625.625,0,1,1,0,1.25H5.431l-.086.078A5.14,5.14,0,0,0,3.308,5.195c0,1.779.013,3.255.024,4.558.053,6,.064,7.274-1.641,9H14.925l.851-.85c1.362-1.362,1.339-2.736,1.3-5.23-.007-.449-.015-.913-.015-1.418a.625.625,0,0,1,1.25,0c0,.495.008.953.015,1.4.043,2.554.073,4.4-1.663,6.135l-.944.943A.937.937,0,0,1,15.054,20Z"
                            transform="translate(-0.625 -0.623)"></path>
                        </g>
                      </g>
                    </svg>
                  </div>
                  <span class="font-semibold hover:text-blue-100">Full Time Job</span>
                </a>
                <div class="icon-style fill-blue-300">
                  <svg xmlns="http://www.w3.org/2000/svg" width="8" height="13.42" viewBox="0 0 8 13.42"
                    class="AvailabilityInfoCard-arrow-z0K">
                    <path
                      d="M1.28,0a1.07,1.07,0,0,1,.25,0L1.77.1A.91.91,0,0,1,2,.21,1.2,1.2,0,0,1,2.2.38L7.62,5.8a1.52,1.52,0,0,1,.28.43,1.15,1.15,0,0,1,.1.48,1.16,1.16,0,0,1-.1.49,1.34,1.34,0,0,1-.28.42L2.2,13a1.42,1.42,0,0,1-.43.29,1.32,1.32,0,0,1-.48.09,1.37,1.37,0,0,1-.49-.09A1.1,1.1,0,0,1,.38,13a1.34,1.34,0,0,1-.28-.42,1.23,1.23,0,0,1,0-1,1.34,1.34,0,0,1,.28-.42L4.9,6.72.38,2.18A1.34,1.34,0,0,1,.1,1.76a1.23,1.23,0,0,1,0-1A1.34,1.34,0,0,1,.38.38L.58.21A.65.65,0,0,1,.8.1L1,0a1,1,0,0,1,.24,0Z">
                    </path>
                  </svg>
                </div>
              </div>
              <div class="flex items-center justify-between ">
                <a href="#" class=" hover:bg-gray-50">
                  <div class="icon-style-large blue-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"
                      class="AvailabilityInfoCard-leadingIcon-jcE">
                      <g transform="translate(0.625 0.625)">
                        <g transform="translate(0 0)">
                          <path
                            d="M14.375,8.759A5.625,5.625,0,1,1,8.75,14.384,5.631,5.631,0,0,1,14.375,8.759Zm0,10A4.375,4.375,0,1,0,10,14.384,4.38,4.38,0,0,0,14.375,18.759Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path
                            d="M16.585,15.009h-2.21a.625.625,0,0,1-.625-.625v-2.21a.625.625,0,0,1,1.25,0v1.585h1.585a.625.625,0,0,1,0,1.25Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path d="M8.75,9.384H4.375a.625.625,0,0,1,0-1.25H8.75a.625.625,0,0,1,0,1.25Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path d="M6.875,12.509h-2.5a.625.625,0,0,1,0-1.25h2.5a.625.625,0,0,1,0,1.25Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path d="M6.875,15.634h-2.5a.625.625,0,0,1,0-1.25h2.5a.625.625,0,0,1,0,1.25Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path
                            d="M8.125,20.009H1.875A1.875,1.875,0,0,1,0,18.134V5.009A1.877,1.877,0,0,1,1.875,3.134H4.427a3.751,3.751,0,0,1,7.4,0h2.552A1.877,1.877,0,0,1,16.25,5.009V6.884a.625.625,0,1,1-1.25,0V5.009a.626.626,0,0,0-.625-.625H11.25a.625.625,0,0,1-.625-.625,2.5,2.5,0,0,0-5,0A.625.625,0,0,1,5,4.384H1.875a.626.626,0,0,0-.625.625V18.134a.625.625,0,0,0,.625.625h6.25a.625.625,0,0,1,0,1.25Z"
                            transform="translate(-0.625 -0.634)"></path>
                          <path d="M8.125,4.384a.937.937,0,1,1,.938-.937A.939.939,0,0,1,8.125,4.384Z"
                            transform="translate(-0.625 -0.634)"></path>
                        </g>
                      </g>
                    </svg>
                  </div>
                  <span class="font-semibold hover:text-blue-100">Freelance/Project</span>
                  <p class="ml-7 text-xs">Availability: Now</p>
                </a>
                <div class="icon-style fill-blue-300">
                  <svg xmlns="http://www.w3.org/2000/svg" width="8" height="13.42" viewBox="0 0 8 13.42"
                    class="AvailabilityInfoCard-arrow-z0K">
                    <path
                      d="M1.28,0a1.07,1.07,0,0,1,.25,0L1.77.1A.91.91,0,0,1,2,.21,1.2,1.2,0,0,1,2.2.38L7.62,5.8a1.52,1.52,0,0,1,.28.43,1.15,1.15,0,0,1,.1.48,1.16,1.16,0,0,1-.1.49,1.34,1.34,0,0,1-.28.42L2.2,13a1.42,1.42,0,0,1-.43.29,1.32,1.32,0,0,1-.48.09,1.37,1.37,0,0,1-.49-.09A1.1,1.1,0,0,1,.38,13a1.34,1.34,0,0,1-.28-.42,1.23,1.23,0,0,1,0-1,1.34,1.34,0,0,1,.28-.42L4.9,6.72.38,2.18A1.34,1.34,0,0,1,.1,1.76a1.23,1.23,0,0,1,0-1A1.34,1.34,0,0,1,.38.38L.58.21A.65.65,0,0,1,.8.1L1,0a1,1,0,0,1,.24,0Z">
                    </path>
                  </svg>
                </div>
              </div>

            </div>
          </div> -->

          <!-- Statistics Section -->
          <div class="mt-8 text-left hidden-mobile">
            <div class="mb-2 flex justify-between">

              <span class="text-gray-600"> <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12"
                  viewBox="0 0 16 16" class="ProjectCoverNeue-icon-zWO inline-block mr-1">
                  <path
                    d="M8.5 3.5c-5 0-8 5-8 5s3 5 8 5 8-5 8-5-3-5-8-5zm0 7c-1.105 0-2-.896-2-2 0-1.106.895-2 2-2 1.104 0 2 .894 2 2 0 1.104-.896 2-2 2z">
                  </path>
                </svg>Tổng lượt xem</span>
              <span class="font-semibold text-gray-800">71,472</span>
            </div>
            <div class="mb-2 flex justify-between">
              <span class="text-gray-600">
                <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0.5 0.5 16 16"
                        class="Appreciations-icon-Z4i ProjectCoverNeue-icon-zWO inline-block">
                        <path fill="none" d="M.5.5h16v16H.5z"></path>
                        <path
                          d="M.5 7.5h3v8h-3zM7.207 15.207c.193.19.425.29.677.293H12c.256 0 .512-.098.707-.293l2.5-2.5c.19-.19.288-.457.293-.707V8.5c0-.553-.445-1-1-1h-5L11 5s.5-.792.5-1.5v-1c0-.553-.447-1-1-1l-1 2-4 4v6l1.707 1.707z">
                        </path>
                        </svg>
                Tổng lượt thích</span>
              <span class="font-semibold text-gray-800">13,580</span>
            </div>
            <div class="mb-2 flex justify-between text-gray-800">
              <a href="tel:+0868379318" class="call-button">
  <svg class="inline-block" xmlns="http://www.w3.org/2000/svg" width="14px" height="14px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
    <path d="M22 16.92V21a2 2 0 0 1-2.18 2A19.88 19.88 0 0 1 2 5.18 2 2 0 0 1 4 3h4.09a2 2 0 0 1 2 1.72 12.05 12.05 0 0 0 .57 2.57 2 2 0 0 1-.45 2.11L8.91 10.91a16 16 0 0 0 6.59 6.59l1.51-1.51a2 2 0 0 1 2.11-.45 12.05 12.05 0 0 0 2.57.57 2 2 0 0 1 1.72 2.01z"/>
  </svg>
 <span> Gọi ngay cho chúng tôi</span>
</a>
            </div>
            <div class="mb-4 flex justify-between text-gray-800">
              <a href="sms:+0868379318" class="message-button">
  <svg class="inline-block" xmlns="http://www.w3.org/2000/svg" width="14px" height="14px" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
    <path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/>
  </svg>
  Nhắn tin
</a>
            </div>
          </div>

          <!-- On the Web -->
          <div class="mt-6 hidden-mobile">
            <h3 class="mb-2 text-lg text-black font-semibold">On The Web</h3>
            <a href="#" class="flex items-center rounded-lg border p-2 text-black hover:bg-gray-50">
              <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" class="mr-2 h-5 w-5"
                alt="Instagram" />
              Instagram
            </a>
          </div>

          <!-- Teams Section -->
          <!-- <div class="mt-6">
            <h3 class="mb-2 text-lg font-bold">Teams</h3>
            <div class="space-y-2">
              <a href="#" class="flex items-center rounded-lg border p-2 hover:bg-gray-50">
                <img src="https://upload.wikimedia.org/wikipedia/commons/8/80/Shopno_Logo.png" class="mr-2 h-8 w-8"
                  alt="Shopno" />
                <div class="flex-grow">
                  <p class="font-semibold">Shopno</p>
                  <p class="text-sm text-gray-500">Jhenaidah, Bangladesh</p>
                </div>
                <button class="text-blue-500">+ Follow</button>
              </a>
              <a href="#" class="flex items-center rounded-lg border p-2 hover:bg-gray-50">
                <img src="https://upload.wikimedia.org/wikipedia/commons/e/e8/Efuture_Logo.png" class="mr-2 h-8 w-8"
                  alt="efuture studio" />
                <div class="flex-grow">
                  <p class="font-semibold">efuture studio</p>
                  <p class="text-sm text-gray-500">Telegraph, TX, USA</p>
                </div>
                <button class="text-blue-500">+ Follow</button>
              </a>
            </div>
          </div> -->

          <!-- Links Section -->
          <!-- <div class="mt-6">
            <h3 class="mb-2 text-lg font-bold">Links</h3>
            <div class="space-y-2">
              <a href="https://wa.me/8801795063000" class="flex items-center rounded-lg border p-2 hover:bg-gray-50">
                <span class="flex-grow text-gray-700">WhatsApp</span>
              </a>
              <a href="#" class="flex items-center rounded-lg border p-2 hover:bg-gray-50">
                <span class="flex-grow text-gray-700">Skype</span>
              </a>
            </div>
          </div> -->

          <!-- About Me Section -->
          <div class="mt-8 text-left hidden-mobile">
            <h3 class="mb-2 text-lg font-bold">About Me | About My Services</h3>
            <p class="text-gray-700">Available for New Project!</p>
            <p class="text-gray-700">Logo, Branding Identity, animations, etc</p>
            <p class="mt-4 text-gray-700">My ultimate goal is to hear from you "I am very satisfied with your design &
              services". You will get changes until you are 100% satisfied. I will create an awesome logo & brand
              identity for you.</p>
            <p class="mt-4 text-gray-500">Member since: March 30, 2019</p>
          </div>
        </div>
      </div>

      <!-- Grid -->
      <div class="ml-4 sm:mt-0 md:mt-12 flex-1">
        <div class="grid grid-cols-1   md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-3 gap-4">
          <div v-for="thumb in thumbnails" class="rounded bg-white  ">
            <div class="group relative max-w-sm overflow-hidden rounded bg-white hover:cursor-pointer ">
              <img class="w-full" :src="`/assets/thumbnails/${thumb.imgSrc}.png`"
                alt="Project Image" />

              <!-- Overlay that shows on hover -->
              <div @click="setDetail(thumb.imgSrc)" 
                class="absolute inset-0 flex flex-row items-end justify-center bg-black bg-opacity-50  transition-opacity duration-300 opacity-100 md:opacity-0  group-hover:opacity-100">
                <div class="flex items-center justify-between w-full p-2 pb-3">
                  <div class="text-xs">
                    <div class="font-bold text-white">{{ thumb.title }}
                    </div>
                    <p class="text-gray-100">{{ thumb.subTitle }}</p>
                  </div>

                  <div class="mt-4 flex items-center space-x-2">
                    <div class="flex items-center space-x-1  fill-white">
                      <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0.5 0.5 16 16"
                        class="Appreciations-icon-Z4i ProjectCoverNeue-icon-zWO">
                        <path fill="none" d="M.5.5h16v16H.5z"></path>
                        <path
                          d="M.5 7.5h3v8h-3zM7.207 15.207c.193.19.425.29.677.293H12c.256 0 .512-.098.707-.293l2.5-2.5c.19-.19.288-.457.293-.707V8.5c0-.553-.445-1-1-1h-5L11 5s.5-.792.5-1.5v-1c0-.553-.447-1-1-1l-1 2-4 4v6l1.707 1.707z">
                        </path>
                      </svg>
                      <span class="text-xs text-gray-300">{{ thumb.like }}</span>
                    </div>
                    <div class="flex items-center space-x-1 fill-white">
                      <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 16 16"
                        class="ProjectCoverNeue-icon-zWO">
                        <path
                          d="M8.5 3.5c-5 0-8 5-8 5s3 5 8 5 8-5 8-5-3-5-8-5zm0 7c-1.105 0-2-.896-2-2 0-1.106.895-2 2-2 1.104 0 2 .894 2 2 0 1.104-.896 2-2 2z">
                        </path>
                      </svg>
                      <span class="text-xs text-gray-300"> {{ thumb.view }}</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

        </div>
      </div>

      <!-- Overlay List -->
      <transition name="fade">
        <div v-show="isOverlayOpen" @click.self="toggleOverlay"
          class="overlay fixed inset-0 bg-black bg-opacity-85 flex justify-center items-center">
          <div class="bg-white p-2 rounded  h-screen overflow-y-auto" style="width: 70%;">
            <ul>
              <li v-for="item in getDetailImage(folderName)" :key="item" class="text-gray-700">
                <img class="w-full " :src="item" alt="Project Image" />
              </li>
            </ul>
          </div>
        </div>
      </transition>
      <!-- <div v-if="isOverlayOpen" class="fixed inset-0 bg-gray-800 bg-opacity-75 flex justify-center items-center">
            <div class="bg-white p-5 rounded shadow-lg h-full w-4/5 sm:w-3/5 lg:w-3/5">
                <ul class="space-y-2">
                    <li v-for="i in 29" :key="item" class="text-gray-700">
                      <img class="w-full " :src="`/assets/images/kuzo-29/${i}.png`" alt="Project Image" />
                    </li>
                </ul>
            </div>
        </div> -->

    </div>
  </body>
  <footer class="bg-black text-white mt-12 py-6 px-8 text-sm">
    <div class="container mx-auto flex justify-between items-center">
      <div class="flex items-center space-x-2">
        <img
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Adobe_Corporate_Logo.png/768px-Adobe_Corporate_Logo.png"
          alt="Adobe Logo" class="h-6">
        <span>&copy; 2024 Adobe Inc. All rights reserved.</span>
      </div>
      <div class="flex space-x-4">
        <a href="#" class="hover:underline">English</a>
        <a href="#" class="hover:underline">TOU</a>
        <a href="#" class="hover:underline">Privacy</a>
        <a href="#" class="hover:underline">Community</a>
      </div>
    </div>
  </footer>
</template>

<style>
.icon-style {
  margin: 3px 8px 0 0;
  min-width: 14px;
  width: 14px;
  display: inline-block;
}

.icon-style-large {
  margin: 3px 8px 0 0;
  min-width: 18px;
  width: 18px;
  display: inline-block;
}

.white-icon {
  fill: white
}

.blue-icon {
  @apply fill-blue-100;
}

.button-style {
  @apply flex justify-center items-center mb-2 w-full rounded-3xl font-bold;
}

.logo {
  position: absolute;
  transform: translate(280%, -60%);
  z-index: 10;
}

.overlay {
  z-index: 99;
}

.logo img {
  width: 5.5rem;
  height: 5.5rem;
}

@media only screen and (max-width: 600px) {
  .logo {
    transform: translate(-50%, -60%);
    left: 50%;
  }


}



.zoom {
  transition: transform .2s;
  /* Animation */
}

.word-art {
  font-family: 'Arial', sans-serif;
  font-size: 14px;
  font-weight: 300;
  letter-spacing: 4px;
  word-spacing: 4px;
  color: gainsboro;
  text-shadow:
    3px 3px 0 #000,
    /* black outline */
    -3px 3px 0 #000,
    3px -3px 0 #000,
    -3px -3px 0 #000,
    6px 6px 0 rgba(0, 0, 0, 0.5);
  /* 3D effect */
}

.word-art-position {
  margin-right: 10%;
  margin-top: 20px;
}

@media only screen and (max-width: 600px) {
  .word-art {
    font-size: 12px;
  }
}

/* @media only screen and (max-width: 1920px) {
 .container-main {
  display: flex;
 }
}
@media only screen and (max-width: 1200px) {
  .container-main {
  display: block;
 }
} */
@media only screen and (max-width: 600px) {
  .hidden-mobile {
    display: none;
  }
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter,
.fade-leave-to

/* .fade-leave-active in Vue 2.1.8 and earlier */
  {
  opacity: 0;
}

#element::-webkit-scrollbar {
    display: none;
}

::-webkit-scrollbar {
    display: none;
}
</style>