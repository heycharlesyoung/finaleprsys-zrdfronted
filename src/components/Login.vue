<template>
    <div class="login_container">
        <div class="login_box">
            <!-- 头像区域-->
            <div class="avatar_box">
                <img src="../assets/logo.jpg" alt="">
            </div>
            <!--登录表单区-->
            <el-form label-width="0px" class="login_form">
                <el-form-item >
                <el-input prefix-icon="el-icon-user"></el-input>
                </el-form-item>
            <!--用户名 -->
                <el-form-item >
                <el-input prefix-icon="el-icon-lock"></el-input>
                </el-form-item>
          
            <!-- 密码 -->
            <el-form-item class="btns">
                <el-button type="primary">登录</el-button>
                <el-button type="info">重置</el-button>
                </el-form-item>
            </el-form>
            <!-- 按钮 -->
        </div>
            
                
    </div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
.login_container{
    background-color: rgb(3, 177, 104);
    height: 100%;
}
.login_box{
    width: 450px;
    height: 300px;
    background-color:#fff;
    border-radius: 3px;
    position: absolute;
    left: 50%;
    top:50%;
    transform: translate(-50%,-50%);
    .avatar_box{
        height: 130px;
        width: 130px;
        border: 1px solid #eee;
        border-radius: 50%;
        padding: 10px;
        box-shadow: 0 0 10px #ddd;
        position: absolute;
        left:50%;
        transform: translate(-50%,-50%);
        background-color: #fff;

        img{
            width:100%;
            height: 100%;
            border-radius: 50%;
            background-color: #eee;
        }
    }
}
.btns{
    display: flex;
    justify-content: flex-end;
}
.login_form{
    position:absolute;
    bottom: 0;
    width: 100%;
    padding: 0 20px;
    box-sizing:border-box;
}
</style>