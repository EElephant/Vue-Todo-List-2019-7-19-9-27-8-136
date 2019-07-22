<template>
    <div id="Footer">
        <ul>
            <li>
                <a @click="displayAll">All</a>
            </li>
            <li>
                <a @click="filterActive">Active</a>
            </li>
            <li>
                <a @click="filterComplete">Complete</a>
            </li>
        </ul>
    </div>
</template>

<script>

import store from '../store'

export default {
    data(){
        return {
            activeButtonFlag: '',
            buttonAll: 'ALL',
            buttonActive: 'ACTIVE',
            buttonComplete: 'COMPLETE'
        }
    },
    methods:{
        filterActive(){
            this.$store.commit('changeActiveButton', this.buttonActive)
        },
        filterComplete(){
            this.$store.commit('changeActiveButton', this.buttonComplete)
        },
        displayAll(){
            this.$store.commit('changeActiveButton', this.buttonAll)
        }
    }
    
}
</script>

<style>
li a {
    color: #fc999b;
    margin: 3px;
    padding: 3px 7px;
    text-decoration: none;
    border: 1px solid transparent;
    border-radius: 3px;
}
li {
    text-align: -webkit-match-parent;
    display: inline;
    margin: 0 0 5px 0;
    padding: 8px;
    list-style: none;
    outline: none;
}
#Footer{
    margin-left: 100px;
    width: 350px;
}
</style>
