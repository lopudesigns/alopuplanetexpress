<template lang='pug'>
  .test1
    .text woo hoo
</template>

<script>
export default {
  name: 'test1-comp',
  data () {
    return {
      // objects: null,
      uuid: this._uid
    }
  },
  sockets: {
    connect: function(){
      // console.log("socket connect vue side")
    },
    // giveObjects(data){
    //   // console.log(data)
    //   if(this.uuid == data.id){
    //     this.objects = data.objects
    //   }
    // }
  },
  created () {
    // if(this.count !== 0){
    //   this.getObjects({
    //     count: this.count,
    //     sort: 'alphabetical',
    //     sortDirection: 'ascending',
    //     id: this.uuid
    //   })
    // } else {
    //   this.objects = null
    // }
  },
  methods: {
    // getObjects(opts){
    //   this.$socket.emit('getObjects', opts)
    // }
  },
  props: {
    "siteTitle": {}
  },
  components: {
  },
  watch: {
    // '$store.state.entity': function(){
    //   this.entity = this.$store.state.entity
    // },
  },  
  route: {
    canActivate(){
      return true
    }
  }}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../styles/vars'
.test1
  width: 100%
  max-width: 100%
  height: 100vh
  background: $green
  overflow: hidden

</style>
