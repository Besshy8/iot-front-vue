<template>
    <div>
        <p>API Response</p>
        <p><button @click="apiReq">REQUEST GO</button></p>
        <p>{{ this.info }}</p>
    </div>    
</template>

<script>

import axios from 'axios'

export default {
    name: "RestApi",
    data() {
        return {
            info: null
        }
    },
    methods: {
        apiReq() {
            axios.get('https://api.coindesk.com/v1/bpi/currentprice.json')
                .then(response => (this.info =response))
        }
    }
    
}
</script>