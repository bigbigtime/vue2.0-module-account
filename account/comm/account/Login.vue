<template>
    <div id="login">
        <Navbar />
        <Pagename txt="登录" />
        <UsernameTypeTag />
        <Username />
        <Password :passwords_show="false"/>
        <div class="blank-102"></div>
        <SubmitButton />
        <div class="link">
            <router-link to="/register">注册</router-link>
            <router-link to="/forget">忘记密码</router-link>
        </div>
    </div>
</template>
<script>
import Navbar from "../../components/comm/Navbar";
import Username from "../../components/form/Username";
import Password from "../../components/form/Password";
import Passwords from "../../components/form/Passwords";
import SubmitButton from "../../components/form/Submit";
import Code from "../../components/form/Code";
import Pagename from "./components/PageTitle";
import UsernameTypeTag from "../../components/form/UsernameType";

export default {
    name: "Login",
    components: { Navbar, Pagename, UsernameTypeTag, Username, Code, Password, Passwords, SubmitButton }
}
</script>
<style lang="scss">
@import "../../styles/index";
.link {
    padding: 20px 0;
    text-align: center;
    font-size: 12px;
    a { margin: 0 10px; }
}
</style>