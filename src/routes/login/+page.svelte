<svelte:head>
    <title>Login Form</title>
</svelte:head>

    
    <div class="form-container">
        <h2>Login Page</h2>
        <div class="login">
            <form id="login" method="get" action="login.php">
                <div class="form-group">
                    <label>Username</label>
                    <input type="text" name="Uname" id="Uname" placeholder="Username">
                </div>
                <div class="form-group">
                    <label>Password</label>
                    <input type="Password" name="Pass" id="Pass" placeholder="Password">
                </div>
                
                <input type="button" name="log" id="log" value="Log In Here">
                
                <div class="form-group">
                    <input type="checkbox" id="check">
                    <span>Remember me</span>
                </div>
                
                <div class="form-group">
                    Forgot <a href="">Password</a>
                </div>
            </form>
        </div>
    </div>
