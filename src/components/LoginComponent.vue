<template>
    <div class="container-fluid Login-container">
        <div>
           <font-awesome-icon class="ico_arrow" icon="fa-solid fa-caret-down" />
        </div>
        <div class="container login-fix">
            <div class="thumb-gym">
                <img src="../assets/img/home_img-compressor.jpg" alt="">
            </div>
            <div class="login-system">
                <h3 >Sign Up  For A Free Training Session!</h3>
                <form action="get">
                    <label class="margin" for="Name">Nome *</label>
                    <input  type="text" v-model="name">
                     <label class="email-inp" for="email">Email</label>
                    <input type="Email" v-model="email">
                    <button class="margin-y text-uppercase">Start Now!</button>

                </form>
                
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: "LoginComponent",
    data(){
        
        return{
        name :"",
        email: "",
        }
    }
}
</script>


<style lang="scss" scoped>
.Login-container{
    background-color:#252a2d;
    height: 70vh;
    display:Flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    position:relative;

    .ico_arrow{
       color: #6b6b6b;
    font-size: 71px;
    position: absolute;
    top: -36.5px;
    left: 49.5%;

    }
        .login-system{
            position:relative;

            h3{
                position:absolute;
                bottom:73%;
                left:12%;
                color:white;
            }
        }
    .login-fix{
        display:flex;
        
        justify-content: center;
        align-content: center;
        align-items: center;
        form{
            margin-top:50px;
            padding:70px;
            display:flex;
            flex-direction: column;
            .margin{
                margin-top:50px;
            }
            label{
                color:white;
            }
            input{
                width: 415px;
                padding:6px;
                border:1px solid white;
                background-color:#252a2d;;
                color:white;
            }
            
            .email-inp{
                margin-top:45px;
            }

            .margin-y{
                margin-top:85px;
                padding:10px;
                background-color:#d5625f;
                color:white;    
                border:none;        }
        }
    }
}
</style>