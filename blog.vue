Vue.component('blog-post', {
    props: ['blogpost'],
    template: `<div id='singlePost'>
                <h2>{{ blogpost.title }}</h2>
                <h3>{{ blogpost.username }}</h3>
                <h4>{{ blogpost.date }}</h4>
                <p>{{ blogpost.content }}</p>
                </div>`,
})

let blogVue = new Vue({
    el: '#blogPosts',
    data: {
        posts: [
            { title: 'First Post', username: 'Jesse Smart', date: 'March 6th, 2021', content: 'This is the content of the March 6th post.'},
            {title: 'Second Post', username: 'Jesse Smart', date: 'March 8th, 2021', content: 'This is the content of the March 8th post.'}
        ]
    }
})