<template>
    <section class="hero-bg w-full flex items-center justify-center relative">
        <div class="absolute inset-0 bg-black opacity-60 w-full h-full z-10"></div>
        <article class="container w-full h-full inset-0 absolute z-20 m-auto flex flex-col items-center justify-center px-4 md:px-0">
            <div class="w-full flex flex-col items-center justify-center gap-y-5 text-center lg:w-10/12">
                <h1 class="font-bold">Where will you go next?</h1>
                <div class="bg-white py-2 px-3 rounded-full w-full flex items-center gap-x-2 md:py-4 md:px-6 lg:w-10/12">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 text-gray-500">
                        <path stroke-linecap="round" stroke-linejoin="round" d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                    </svg>
                    <input type="search" name="" value="" class="w-full border-none shadow-none outline-none text-black" placeholder="search your option">
                </div>
                <p class="text-sm leading-7 w-full lg:w-10/12">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In sed et donec purus viverra. Sit justo velit, eu sed sollicitudin tempus, risus. Sed sit elit mauris adipiscing. Lobortis pellentesque nulla accumsan id urna, ullamcorper gravida varius. Massa mauris, cursus orci magna non enim fames et sed. </p>
            </div>

            <div class="w-full flex flex-col items-center justify-center gap-y-2 text-green-300 absolute bottom-0 pb-8">
                <p class="text-xl lg:text-2xl font-bold">Let's Go</p>
                <i class="fa-solid fa-arrow-down"></i>
            </div>
            
        </article>
    </section>
</template>

<style scoped>
h1 {
    font-size: 1.3rem;
}

@media only screen and (min-width: 640px) {
    h1 {
        font-size: 2.5rem;
    } 
}

@media only screen and (min-width: 1024px) {
    h1 {
        font-size: 4rem;
    } 
}
</style>