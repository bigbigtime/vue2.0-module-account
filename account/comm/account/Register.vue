<template>
    <div id="login">
        <Navbar />
        <Pagename txt="注册" />
        <UsernameTypeTag />
        <Username />
        <Password />
        <!-- <Passwords /> -->
        <div class="blank-102"></div>
        <SubmitButton label="注册" type="register" />
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
    name: "Register",
    components: { Navbar, Pagename, UsernameTypeTag, Username, Code, Password, Passwords, SubmitButton }
}
</script>
<style lang="scss">
@import "../../styles/index";
</style>