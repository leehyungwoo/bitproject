<template>
  <div>
    <headerComponent/>
    <!-- inner-banner -->
    <section class="inner-banner" id="home">
        <div class="inner-layer">
            <div class="container">
            </div>
        </div>
    </section>
    <!-- //inner-banner -->
    <!-- breadcrumb -->
    <div class="breadcrumb-w3pvt">
        <div class="container">
            <nav aria-label="breadcrumb">
                <ol class="breadcrumb">
                    <!-- <li class="breadcrumb-item"><a href="index.html">Home</a></li> -->
                    <li class="breadcrumb-item" aria-current="page">Login</li>
                </ol>
            </nav>
        </div>
    </div>
    <!-- //breadcrumb -->
    <!-- contact -->
    <section class="contact py-5">
        <div class="container py-lg-5">
            <h2 class="heading mb-sm-5 mb-4"><strong> Login </strong></h2>
            <div class="row">
                <div class="col-lg-12 contact-form mt-md-0 mt-sm-5 mt-4">
                    <h4 class="mb-4 w3f_title">로그인</h4>
                    <div name="contactform" id="contactform">
                        <div class="form-group">
                            <label>아이디</label>
                            <input type="text" class="form-control" id="user_id" placeholder="Enter Id" name="user_id">
                        </div>
                        <div class="form-group">
                            <label>비밀번호</label>
                            <input type="password" class="form-control" id="user_password" placeholder="Enter Password" name="user_password">
                        </div>
                        <button @click="login()" class="btn btn-default">Login</button>
                        <router-link to="find-user" class="btn btn-default">FindUser</router-link>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- //contact -->
    <copyright></copyright>
    <movetop></movetop>
    </div>
</template>

<script>

import headerComponent from "@/components/common/headerComponent"
import copyright from "@/components/common/copyright"
import movetop from "@/components/common/movetop"
export default {
    data(){
        return{
           
        }
    },
    components:{
        headerComponent,
        copyright,
        movetop
    },
    methods:{
        login(){
            alert("로그인")
        }
    }
}
</script>



<style scoped>
#contactform a{border: 2px solid #ffc168;
    border-radius: 5px;
    color: #fff;
    background: #ffc168;
    font-size: 16px;
    letter-spacing: 1px;
    padding: 8px 30px;
    display: inline-block;}
</style>
