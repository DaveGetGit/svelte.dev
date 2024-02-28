<script>
  import ReactiveAssignment from "./Reactive_Assignment.svelte";
  import Nested from "../../components/Nested.svelte";

    let count = 0 ;

    $: if(count >=10){
        alert('count is dangeroously high');
        count=0;
    }

    function handleClick(){
        count += 1;
    }
</script>

<button on:click={handleClick}>
    Clicked {count} 
    {count === 1 ? 'time' : 'times'}
</button>

