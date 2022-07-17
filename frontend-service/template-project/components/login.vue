<template>
    <div class="login-container">
        <div class="background">
            <img class="login-bg" src="../assets/img/login-bg.jpg" alt="" />
        </div>
        <div class="loginform">
            <form class="form">
                <h2>Brand</h2>
                <label>User Name :</label>
                <input type="text"/>
                <label>Password :</label>
                <input type="password"/>

                <button type="submit" class="button">sign-in</button>
                <span>or</span>
                <button  class="button">sign-up</button>
            </form>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .login-container{
        margin: 0;
        padding: 0;
        display: flex;
    }
    .background {
        flex: 1;
    }
    .login-bg {
        height: 100vh;
        width: 100%;
    }
    .loginform {
        width: 40%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

    }
    .form {
        height: 90%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
    }

    input {
        margin-bottom: 20px;
        height: 40px;
        width: 300px;
        border-radius: 5px;
        border: none;
        font-weight: 600;
        word-spacing: 2px;
        font-size: 1.2rem;
        padding: 0 10px;
    }
    input:focus {
       outline: none;
    }

    label {
        font-weight: 600;
        color: #fff;
        margin: 5px 0;
    }
    span {
        color: #fff;
    }
    .form h2 {
        font-family: 'Pacifico', cursive;
        color: #fff;
        font-size: 3.5rem;
    }
    
    @media screen and (max-width: 777px) {
        .background{
            height: 10%;
            width: 100%;
            display: none;
        }
        .login-bg {
            width: 100%;
            height: 10%;
        }
        .login-container{ 
            justify-content: center;
            flex-direction: column;
            align-items: center;
        }
    }

    @media screen and (min-width: 1366px) {
        .loginform {
            width: 60%;
        }
    }
</style>