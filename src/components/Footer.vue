<template>
  <footer class="py-5">
    <div class="container">
        <div class="col-6">        
            <ul>
                <li class="h5"> Address </li>
                <li> {{this.contactInfo.address}} </li>
                <li class="my-2"> {{this.contactInfo.phone}}</li>
                <li> {{this.contactInfo.email}}</li>
            </ul>
            <div class="my-2">
                logo logo logo logo
            </div>
        </div>
        <div class="col-6">
            
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    data:function(){
        return{
            contactInfo:{
                address:'Indirizzo e via',
                phone:'305 547-9909',
                email:'support@maxcoach.com'
            }
        }
    }
}
</script>

<style lang="scss">
    footer{
        background-color: rgb(211, 165, 165);
    }
</style>