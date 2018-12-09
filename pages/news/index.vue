<template>
    <div>
        <h2>News index page</h2>
        <p>NewsId:{{$route.params.newsId}}</p>
        <ul>
            <li><a href="/">home</a></li>
        </ul>
        <ul>
            <li>
                <a href="/">home</a>
            </li>
            <li>
                <!-- <a href="/news/456">news-1</a> -->
                <nuxt-link :to="{name:'news-id',params:{id:456,title:'xiaokun.com'}}">news-1</nuxt-link>
            </li>
            <li>
                <a href="/news/abc">new-2</a>
            </li>
        </ul>
    </div>
</template>
