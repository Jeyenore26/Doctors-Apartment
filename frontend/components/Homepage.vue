<template >
    <container   class="  flex justify-between mt-10  text-[#1A5349]">
        <section class="mt-20 font-bold text-[15px] md:text-[20px] w-[50rem] ">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur cumque vitae suscipit accusamus libero corporis similique, labore omnis possimus quasi quidem consectetur nemo, debitis animi veritatis, architecto voluptas! Ab, fugiat!
            <span class="flex justify-center sm:justify-start">
                <button class=" rounded-xl mt-10  bg-[#226b5e] hover:bg-[#1A5349]/60 active:bg-[#1A5349]/80 text-white  px-4 py-[0.35rem] shadow-sm transition-x">
     Check Out
            </button>
            </span>
        </section>
        <img src = '../public/Doc1.png' class="bg-cover w-[20em] h-[15.5rem] md:w-[30rem] md:h-[25rem] hidden sm:block" />
            

    </container>
    <span class= "border-gray-400 border-t-[0.1px] mt-20 mb-10  flex justify-center"></span>
    <h2 class="font-bold text-[25px] text-[#1A5349]">Explore What We Do</h2>
    <container class="flex flex-col md:flex-row py-10 justify-between  xl:justify-evenly">
        <span class="w-[12rem] h-[12rem] flex justify-center   rounded-lg bg-[#c9f7fc] hover:bg-[#7babb1] hover:text-white hover:w-[14rem] transition-x hover:h-[14rem] hover:border-[1px] hover:border-blue-200 relative hover:shadow-lg md:mb-0 mb-10  mx-auto md:mx-0"><h5 class="m-4">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Autem molestiae velit ipsum asperiores ipsa 
        </h5></span>
        <span class="w-[12rem] h-[12rem] flex justify-center rounded-lg bg-[#c9f7fc] hover:bg-[#7babb1] hover:text-white hover:w-[14rem] transition-x hover:h-[14rem] hover:border-[1px] hover:border-blue-200 relative hover:shadow-lg md:mb-0 mb-10 mx-auto md:mx-0"><h5 class="m-4">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Autem molestiae velit ipsum asperiores ipsa 
        </h5></span>
        <span class="w-[12rem] h-[12rem] flex justify-center rounded-lg bg-[#c9f7fc] hover:bg-[#7babb1] hover:text-white hover:w-[14rem] transition-x hover:h-[14rem] hover:border-[1px] hover:border-blue-200 relative hover:shadow-lg md:mb-0 mb-10 mx-auto md:mx-0"><h5 class="m-4">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Autem molestiae velit ipsum asperiores ipsa 
        </h5></span>
        <span class="w-[12rem] h-[12rem] flex justify-center rounded-lg bg-[#c9f7fc] hover:bg-[#7babb1] hover:text-white hover:w-[14rem] transition-x hover:h-[14rem] hover:border-[1px] hover:border-blue-200 relative hover:shadow-lg md:mb-0 mb-10 mx-auto md:mx-0"><h5 class="m-4">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Autem molestiae velit ipsum asperiores ipsa 
        </h5></span>

    </container>
    <div class="mt-[40rem]">d</div>
</template>

<script>

export default {
    name:'Homepage'
};
</script>

<style>
.gradient{
    background-image: linear-gradient(to right , #F2FEFF , #EDFDFF,  #fff , #EDFDFF , #F2FEFF);
    height: 100vh;
    width: 100%;
}
.transition-x{
    transition-property: all;
    transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
    transition: 300ms;
}
</style>