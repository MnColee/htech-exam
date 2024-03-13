<template>
    <section class="w-full h-auto flex flex-col items-center justify-center relative text-center">
        <h1 class="font-bold text-black py-5">World's Best Places to Visit</h1>
        <article class="container relative w-full h-full 2xl:w-9/12">
            <video class="iframe w-full" loop controls>
                <source src="https://www.youtube.com/watch?v=CDx2fxb5ZF4" type="video/mp4">
                <source src="https://www.youtube.com/watch?v=CDx2fxb5ZF4" type="video/ogg">
                    Your browser does not support the video tag.
            </video>

            <div class="absolute z-20 inset-0 w-full flex items-center justify-center px-4 lg:px-0 ">
                <div class="absolute inset-0 bg-black opacity-10 w-full h-full z-10"></div>
                <div class="w-full flex flex-col items-center justify-center gap-y-8 text-center lg:w-7/12">
                    <h1 class="font-bold">Trips For your first solo traveling</h1>
                    <small class="leading-7">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In sed et donec purus viverra. Sit justo velit, eu sed sollicitudin tempus, risus. Sed sit elit mauris adipiscing. Lobortis pellentesque nulla accumsan id urna, ullamcorper gravida varius. </small>
                    <div class="flex flex-col items-center gap-2 w-full">
                        <i class="fa-solid fa-circle-play text-red-600"></i>
                        <h6 class="text-gray-200">Watch Video</h6>
                    </div>
                </div>
            </div>
        </article>
    </section>
</template>

<style scoped>
.fa-circle-play {
    font-size: 4rem;
}

h6 {
    font-size: 1.5rem;
}

.iframe {
    height: 35rem;
}

h1 {
    font-size: 1.5rem;
}

@media only screen and (min-width: 640px) {
    h1 {
        font-size: 2rem;
    } 

}
</style>