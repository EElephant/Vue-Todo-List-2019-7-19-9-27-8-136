<template>
    <div id="Footer">
        <ul>
            <li>
                <a href="#">All</a>
            </li>
            <li>
                <a href="#">Active</a>
            </li>
            <li>
                <a href="#">Complete</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    
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
