<template>
    <container   class=" flex justify-between  text-[#1A5349]">
        <strong class="text-xl z-0 mt-7" >
          <icon name = 'mdi:doctor'></icon>
          Doctors'Apartment</strong>
        <section class="mt-7 z-0 md:space-x-7 xs:space-x-2 space-x-0 sm:block hidden" >
            <button class=" rounded-xl px-4  py-[0.35rem] border-[1px] border-[#1A5349] active:border-[#1A5349]/80 hover:border-[#1A5349]/50 transition-x hover:text-black/50 active:text-black/80">
                    About us
            </button>
            <span class='border-r-2  border-black/50'></span>

            <button class="glow rounded-xl px-4  py-[0.35rem] ">
   Login
            </button>
            <span class='border-r-2 border-black/50'></span>
            <button class=" rounded-xl bg-[#226b5e] hover:bg-[#1A5349]/60 active:bg-[#1A5349]/80 text-white  px-4 py-[0.35rem] shadow-sm transition-x">
     Sign Up
            </button>
        </section>
        <section  class=" mt-7  md:space-x-7 space-x-2 sm:hidden block ">
            <button @click="toggle" class=" rounded-xl border-[1px] border-transparent  hover:text-black/50 active:text-black/80">
                <Icon name="material-symbols:menu-rounded"  class="w-8 h-8"  />

            </button>
           
        </section>
    </container>
    <section :class="[!btn ? 'sidebar' : 'closeside']">
      <button v-if=!btn @click="toggle" class=" flex justify-start rounded-xl border-[1px] border-transparent  hover:text-black/50 active:text-black/80">
                <Icon name="material-symbols:menu-open-rounded"  class="w-8 h-8"  />

            </button>
            <strong class="text-xl z-0 mt-5 flex justify-center " v-if = !btn>
              <icon class="mt-1 mr-1" name = 'mdi:doctor'></icon>
              Doctors'Apartment</strong>
            <section v-if = !btn class="mt-7 z-0 flex flex-col-reverse  justify-center mx-[30%]" >
            <button class=" glow rounded-xl border-[1px] border-[#1A5349]  my-5 px-4  py-[0.35rem]">
                    About us
            </button>

            <button class="glow rounded-xl border-[1px] border-[#1A5349]  my-5 px-4  py-[0.35rem] ">
   Login
            </button>

            <button class=" glow rounded-xl border-[1px] border-[#1A5349]  my-5 px-4  py-[0.35rem]">
     Sign Up
            </button>
        </section>

</section>
</template>

<script>
export default {
  data (){
    return {
      btn:true
    }
  },
  methods: {
    toggle() {
      this.btn = !this.btn;
    }
  },
 
}
</script>
<style scoped>
.sidebar{
  color:white;
  top:0;
  right: 0;
  position: fixed;
  overflow-x: hidden;
  transition: ease 500ms;
  background-color: #3f9989;
  height: 100vh;
  display: flex;
  flex-direction: column;
  animation: show 500ms 1;
  width: 100vw;
}
@keyframes show {
  0%{width: 0%;}
  100%{width:100vw;}
}
.closeside{
  top:0;
  right: 0;
  position: fixed;
  overflow-x: hidden;
  transition: ease 500ms;
  background-color: #327a6d;
  animation: show 500ms 1;
  height: 100vh;

  transition: ease 500ms;
  background-color: #327a6d;
  animation: hide 500ms 1;
}
@keyframes hide {
  from{width: 100vw;}
  to{width:0vw;}
}
.glow:hover {

  box-shadow: 0 0 2px 1px #fff, 0 0 5px 3px #327a6d, 0 0 30px 4.5px #517e76;
  transition: all 400ms;
}
.Is_open{
    display: hidden;
}
.glow:active {

    box-shadow: 0 0 20px 1px #fff, 0 0 20px 3px #3f9989, 0 0 100px 4.5px #74b1a6;
    transition: all 400ms;

  }
.transition-x{
    transition-property: all;
    transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
    transition: 300ms;
}
</style>