<script>
    export let productId=100
</script>



<a href="/">home</a>
<h1>List of products is</h1>

<h2><a href="/product/1">product1</a></h2>
<h2><a href="/product/2">product2</a></h2>
<h2><a href="/product/3">product3</a></h2>
<h2><a href={`/product/${productId}`}>product {productId}</a></h2>


