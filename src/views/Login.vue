<template>
  <div class="login">  
      <div data-aos="zoom-in-left" class="container contain">
        <div class="card">
          <div class="form">
            <div class="left-side">
              <span></span> <span></span> <span></span> <span></span>
            </div>
            <div class="right-side">
              <div class="signup_form s_form">
                <div class="login">
                  <h2>User Login</h2>
                </div>
                <div class="input_text">
                  <input type="text" placeholder="Username" />
                </div>
                <div class="input_text">
                  <input
                    class="signup_pass"
                    type="password"
                    name="password"
                    placeholder="Password"
                  />
                </div>
                <div class="login_btn">
                  <button class="login_button">LOGIN</button>
                </div>
                <div class="forget">
                  <p>
                    Forgot <a href="#">Username</a> <a href="#">Password</a> ?
                  </p>
                </div>
                <div class="create margin">
                  <router-link to="/signup" class="create_acc"
                    >Sign Up
                  </router-link>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@300;400;600&display=swap");

.contain {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 500px;
}

.contain .card {
  height: 420px;
  width: 800px;
  background-color: #fff;
  position: relative;
  box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
  font-family: "Nunito Sans", sans-serif;
  border: none;
}

.contain .card .form {
  width: 100%;
  height: 100%;
  display: flex;
}

.contain .card .left-side {
  width: 50%;
  background-color: #fff;
  height: 100%;
  position: relative;
  overflow: hidden;
}

.left-side span:nth-child(1) {
  position: absolute;
  transform: rotate(45deg);
  top: 70px;
  left: -100px;
  display: flex;
  height: 180px;
  width: 400px;
  border-top-right-radius: 150px;
  border-bottom-right-radius: 150px;
  border: 15px solid #049464;
  background-image: linear-gradient(to right, #09bd8027, #09bd80);
}

.left-side span:nth-child(2) {
  position: absolute;
  transform: rotate(45deg);
  top: -20px;
  left: 130px;
  display: flex;
  height: 100px;
  width: 200px;
  border-top-right-radius: 150px;
  border-bottom-right-radius: 150px;
  background-image: linear-gradient(to right, #09bd8027, #09bd80);
}

.left-side span:nth-child(3) {
  position: absolute;
  transform: rotate(45deg);
  top: 280px;
  left: -70px;
  display: flex;
  height: 100px;
  width: 200px;
  border-top-right-radius: 150px;
  border-bottom-right-radius: 150px;
  background-image: linear-gradient(to right, #09bd8027, #09bd80);
}

.left-side span:nth-child(4) {
  position: absolute;
  transform: rotate(-135deg);
  top: 370px;
  left: 170px;
  display: flex;
  height: 100px;
  width: 200px;
  border-top-right-radius: 150px;
  border-bottom-right-radius: 150px;
  background-image: linear-gradient(to right, #09bd8027, #09bd80);
}

.contain .card .right-side {
  width: 50%;
  background-color: #fff;
  height: 100%;
  padding: 20px;
}

.d-none {
  display: none !important;
}

.login {
  display: flex;
  justify-content: center;
  text-align: center;
  width: 100%;
  margin-top: 20px;
}

.input_text {
  margin-top: 20px;
  width: 100%;
  position: relative;
}

input[type="text"] {
  height: 45px;
  width: 100%;
  border: none;
  background-color: #09bd8027;
  outline: 0;
  padding: 5px 10px;
  padding-left: 25px;
  border-radius: 10px;
}

input[type="password"] {
  height: 45px;
  width: 100%;
  border: none;
  background-color: #09bd8027;
  outline: 0;
  padding: 5px 10px;
  padding-left: 25px;
  padding-right: 28px;
  border-radius: 10px;
}

.fa-lock {
  position: absolute;
  top: 15px;
  left: 10px;
  cursor: pointer;
  color: #70747c;
}

.fa-user {
  position: absolute;
  top: 14px;
  left: 9px;
  cursor: pointer;
  color: #70747c;
}

.fa-envelope {
  position: absolute;
  top: 15px;
  left: 7px;
  cursor: pointer;
  color: #70747c;
  font-size: 14px;
}

.fa-eye-slash {
  position: absolute;
  top: 15px;
  right: 9px;
  cursor: pointer;
  color: #70747c;
}

.fa-eye {
  position: absolute;
  top: 15px;
  right: 9px;
  cursor: pointer;
  color: #70747c;
}

.login_btn {
  margin-top: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login_btn button {
  height: 45px;
  outline: 0;
  border: none;
  width: 100%;
  color: white;
  border-radius: 30px;
  background-color: #049464;
  font-size: 13px;
  cursor: pointer;
  transition: all 0.5s;
}

.login_btn button:hover {
  background-color: #09bd80;
  color: white;
}

.forget {
  text-align: center;
  margin-top: 20px;
  font-size: 13px;
  color: #b8b0b1;
  font-weight: 600;
  letter-spacing: 1px;
}

.forget p a {
  text-decoration: none;
  color: #049464;
}

.create {
  margin-top: 40px;
  text-align: center;
  text-decoration: none;
  font-size: 13px;
  font-weight: 700;
}

.margin {
  margin-top: 67px !important;
}

.create a {
  text-decoration: none;
  color: #049464;
}

@media (max-width: 750px) {
  .contain .card {
    max-width: 350px;
  }

  .contain .card .right-side {
    width: 100%;
  }

  .contain .card .left-side {
    display: none;
  }
}
</style>
