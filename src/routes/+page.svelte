<script>
import {goto,beforeNavigate,afterNavigate} from '$app/navigation'

const handleClick= ()=> {

    console.log('placing your order');
    goto('/product',{replaceState: true});

};
beforeNavigate((navigation)=>{
    console.log({before:navigation});
    
})
afterNavigate((navigation)=>{
    console.log({ after:navigation})
})

</script>



<h1>Hello world !!!!</h1>
<!-- <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->
<a href='/blog'>Blog</a>
<a href="/contact">Contact</a>

<button on:click={handleClick}>Place order</button>