<script>
    let user = {loggedIn:false};

    function toggle(){
        user.loggedIn = !user.loggedIn;
    }
</script>


{#if user.loggedIn}
<button on:click={toggle}>LogOut</button>
{/if}

{#if !user.loggedIn}
<button on:click={toggle}>LogIn</button>
{/if}



