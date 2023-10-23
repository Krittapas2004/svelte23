<script>
    function showCat() {
        let cat = document.querySelector(".mainIndexContainer");
        cat.classList.remove("notShowCat");
    }
    function hideCat() {
        let cat = document.querySelector(".mainIndexContainer");
        cat.classList.add("notShowCat");
    }
</script>

<nav>
    <img id="logo" src="img/catlogo.png" alt="Cat Logo">
    <ul>
        <!-- svelte-ignore a11y-mouse-events-have-key-events -->
        <li><a on:mouseover={showCat} on:mouseout={hideCat} href="/">Home</a></li>    
        <!-- svelte-ignore a11y-mouse-events-have-key-events -->
        <li><a on:mouseover={showCat} on:mouseout={hideCat} href="catType">Cat Type</a></li>
        <!-- svelte-ignore a11y-mouse-events-have-key-events -->
        <li><a on:mouseover={showCat} on:mouseout={hideCat} href="store">Store</a></li>        
    </ul>
    <div class="container">
        <form action="https://www.google.com/search" method="get" class="searchbar">
            <input type="text" name="q" placeholder="search">
            <!-- svelte-ignore a11y-missing-attribute -->
            <button type="submit"><img src="img/searchBar.png"></button>
        </form>
    </div>
    <div id="login_bar" style="text-align: right">                                               
        <ul id="login_signup">
            <li><a href="login" id="login_link">Login <span>&#x25c0;</span></a></li>
        </ul>
    </div>
</nav>

<div class="mainIndexContainer notShowCat">
</div>  

<div class="sliding-text">
    <span>What We</span>
    <span>Provide</span>
</div>