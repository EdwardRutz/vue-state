<template>
    <div class="hello">
        <div class="left">
            <h1>{{ title }}</h1>
        </div>
        <div class="right">

        </div>
    </div>
</template>

<script>
  import { mapState } from 'vuex'

  //mapState, is a helper that allows access to the state from Vuex.

  export default {
    name: 'HelloWorld',
    //Computed, calls mapState and passes an array with the name of the state property we defined.
    computed: mapState([
      'title'
    ])
  }
</script>

<style scoped>
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
