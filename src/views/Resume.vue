<template>
<div class="max-w-xl text-left p-8 mx-auto">
  <div class="flow-root">
    <ul class="mb-8">
   
      <li v-for="event in timelineEvents" >
        <div class="relative pb-8" data-aos="fade-right">
          <span class="absolute top-5 left-5 -ml-px h-full w-0.5 bg-gray-200" aria-hidden="true"></span>
          <div class="relative flex items-start space-x-3">
            <div>
              <div class="relative px-1">
                <div class="h-8 w-8 bg-blue-500 rounded-full ring-8 ring-white flex items-center justify-center animate__animated animate__pulse animate__infinite">
                  <svg class="text-white h-5 w-5" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6" />
                  </svg>
                </div>
              </div>
            </div>
            <div class="min-w-0 flex-1 py-0">
              <div class="text-md text-gray-500">
                <div>
                  <p class="font-medium text-gray-900 mr-2">{{ event.title }}</p>
                  
                  
                  
                  <a href="#" class="my-0.5 relative inline-flex items-center bg-white rounded-full border border-gray-300 px-3 py-0.5 text-sm">
                    <div class="absolute flex-shrink-0 flex items-center justify-center">
                      <span class="h-1.5 w-1.5 rounded-full bg-blue-500" aria-hidden="true"></span>
                    </div>
                    <div class="ml-3.5 font-medium text-gray-900">{{ event.label }}</div>
                  </a>
                  
                </div>
                <span class="whitespace-nowrap text-sm">{{ event.date }}</span>
              </div>
              <div class="mt-2 text-gray-700">
              
                <p>{{ event.description }}</p>
              
              </div>
            </div>
          </div>
        </div>
      </li>

    </ul>
  </div>
 </div>
</template>
<script>
export default {
	name: 'Resume',
  title: 'Resume | Albin Varghese',
	props: [],
	components: {},
	data() {
		return {
			timelineEvents: [
				{title: 'Started learning PHP', label: 'php', labelColor: 'blue', subTitle: 'something', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse aliquam orci eu magna sodales, in luctus dolor semper. Maecenas dignissim velit non fermentum sodales. Nulla sed orci neque. Pellentesque ac rutrum mauris. Nulla at magna id metus eleifend molestie. Cras blandit eleifend iaculis. ', date: '13-05-2021'},
				{title: 'Started learning Node Js', label: 'php', labelColor: 'blue', subTitle: 'something', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse aliquam orci eu magna sodales, in luctus dolor semper. Maecenas dignissim velit non fermentum sodales. Nulla sed orci neque. Pellentesque ac rutrum mauris. Nulla at magna id metus eleifend molestie. Cras blandit eleifend iaculis. ', date: '13-05-2021'},
				{title: 'Started learning  Python', label: 'php', labelColor: 'blue', subTitle: 'something', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse aliquam orci eu magna sodales, in luctus dolor semper. Maecenas dignissim velit non fermentum sodales. Nulla sed orci neque. Pellentesque ac rutrum mauris. Nulla at magna id metus eleifend molestie. Cras blandit eleifend iaculis. ', date: '13-05-2021'},
				{title: 'Started learning Css', label: 'php', labelColor: 'blue', subTitle: 'something', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse aliquam orci eu magna sodales, in luctus dolor semper. Maecenas dignissim velit non fermentum sodales. Nulla sed orci neque. Pellentesque ac rutrum mauris. Nulla at magna id metus eleifend molestie. Cras blandit eleifend iaculis. ', date: '13-05-2021'},
				{title: 'Started learning Sass', label: 'php', labelColor: 'blue', subTitle: 'something', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse aliquam orci eu magna sodales, in luctus dolor semper. Maecenas dignissim velit non fermentum sodales. Nulla sed orci neque. Pellentesque ac rutrum mauris. Nulla at magna id metus eleifend molestie. Cras blandit eleifend iaculis. ', date: '13-05-2021'},
				]
			}
		}
	
}
</script>