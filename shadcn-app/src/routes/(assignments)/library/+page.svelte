<script lang="ts">
    import { books } from '$lib/store'
    books.update(books => [...books, 
    {
        author: "Murakami",
        title: "Norwegian Wood",
        genre: "Realism",
        pages: 200,
        read: false}])

</script>