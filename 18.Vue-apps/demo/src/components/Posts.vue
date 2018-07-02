<template>
    <div class="container">
        <table class="table table-striped mt-4">
            <thead>
            <tr>
                <th scope="row"></th>
                <th scope="col">id</th>
                <th scope="col">title</th>
                <th scope="col">body</th>
            </tr>
            </thead>
            <tbody>
            <tr v-for="post in posts" :key="post.id">
                <th scope="row"></th>
                <td>{{post.id}}</td>
                <td>{{post.title}}</td>
                <td>{{post.body}}</td>
            </tr>
            </tbody>
        </table>
    </div>
</template>



<script>
    export default{
        name: 'PostsExample',
        data(){
            return{
                posts:[
                    {id:1, title:'Post 1', body:'11111111111111111111'},
                    {id:2, title:'Post 2', body:'22222222222222222222'},
                    {id:3, title:'Post 3', body:'33333333333333333333'},
                    {id:4, title:'Post 4', body:'44444444444444444444'},
                    {id:5, title:'Post 5', body:'55555555555555555555'}
                ]
            }
        }
    }

</script>


<style>


</style>