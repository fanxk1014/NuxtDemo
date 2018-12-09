<template>
    <div>
        <h2>news-content</h2>
        <p>
            newsId:[{{$route.params.id}}]
        </p>
        <ul>
            <li>
                <a href="/">home</a>
            </li>
        </ul>
    </div>
</template>
<script>
    export default{
        validate({params}){
            return /^\d+$/.test(params.id)
        },
        data(){
            return {
                title: this.$route.params.title,
            }
        },
        head(){
            return {
                title: this.title,
                meta: [
                    {
                        hid: 'Keywords',
                        name: 'seo-Keywords-name',
                        content: 'seo-Keywords-content'
                    },
                    {
                        hid: 'description',
                        name: 'seo-description-name',
                        content: 'seo-description-content'
                    }
                ]
            }
        }
    }
</script>