<svelte:head>
    <title>Login Form</title>
</svelte:head>

<!-- This code represents the login form structure for the Login Page. 
     It includes fields for entering a username and password, 
     a "Log In" button, an option to remember the login, and a link for password recovery. -->
<div class="login-form">
    <div class="form-container">
        <h2>Login Page</h2>
        <div class="login">
            <form class="loginBar" method="get">
                <div class="form-group">
                    <i class="fa-solid fa-user" />
                    <input
                        type="text"
                        name="Uname"
                        id="Uname"
                        placeholder="Username"
                    />
                </div>
                <div class="form-group">
                    <i class="fa-solid fa-lock" />
                    <input
                        type="Password"
                        name="Pass"
                        id="Pass"
                        placeholder="Password"
                    />
                </div>

                <input type="button" name="log" id="log" value="Log In" />

                <div class="rememberLogin">
                    <input type="checkbox" id="check" />
                    <span>Remember me</span>
                </div>

                <div class="form-group">
                    Forgot <a href="/">Password</a>
                </div>
            </form>
        </div>
    </div>
</div>
