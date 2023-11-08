<!-- This is a header bar for each page -->
<!-- This is a functions for showing and hiding the "mainIndexContainer" element based on mouse hover events on navigation links. -->
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
    <img id="logo" src="img/catlogo.png" alt="Cat Logo" />
    <ul>
        <!-- Navigation menu with mouse hover events to trigger the showCat and hideCat functions. -->
        <div class="header-button">
            <!-- svelte-ignore a11y-mouse-events-have-key-events -->
            <li>
                <a on:mouseover={showCat} on:mouseout={hideCat} href="/">Home</a
                >
            </li>
            <!-- svelte-ignore a11y-mouse-events-have-key-events -->
            <li>
                <a on:mouseover={showCat} on:mouseout={hideCat} href="catType"
                    >Our Cat</a
                >
            </li>
            <!-- svelte-ignore a11y-mouse-events-have-key-events -->
            <li>
                <a on:mouseover={showCat} on:mouseout={hideCat} href="store"
                    >Store</a
                >
            </li>
        </div>
    </ul>
    <div class="container">
        <form
            action="https://www.google.com/search"
            method="get"
            class="searchbar"
        >
            <input
                type="text"
                name="q"
                placeholder="Search"
                style="color:black"
            />
            <!-- svelte-ignore a11y-missing-attribute -->
            <button type="submit"><img src="img/searchBar.png" /></button>
        </form>
    </div>
    <div id="login_bar" style="text-align: right">
        <ul id="login_signup">
            <li>
                <a href="login" id="login_link">Login <span>&#x25c0;</span></a>
            </li>
        </ul>
    </div>
</nav>

<div class="mainIndexContainer notShowCat" />
