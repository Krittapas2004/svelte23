<svelte:head>
    <title>Login Form</title>
</svelte:head>

<div class="login-form">
    <div class="form-container">
        <h2>Login Page</h2>
        <div class="login">
            <form id="login" method="get">
                <div class="form-group">
                    
                    <input type="text" name="Uname" id="Uname" placeholder="Username"><i class="fa-solid fa-user"></i>
                </div>
                <div class="form-group">
                    
                    <input type="Password" name="Pass" id="Pass" placeholder="Password"><i class="fa-solid fa-lock"></i>
                </div>
                
                <input type="button" name="log" id="log" value="Log In">
                
                <div class="form-group">
                    <span>Remember me</span>
                    <input type="checkbox" id="check">
                </div>
                
                <div class="form-group">
                    Forgot <a href="/">Password</a>
                </div>
            </form>
        </div>
    </div>
</div>