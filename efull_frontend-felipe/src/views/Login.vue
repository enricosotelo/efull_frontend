<script setup>
    import Navbar from '@/components/Navbar.vue';
    import Footer from '@/components/Footer.vue';
</script>

<template>
   <div class="container">
	<div class="screen">
		<div class="screen__content">
			<form class="login">
                <img class="logo" src="https://res.cloudinary.com/daox93pja/image/upload/v1715122906/e-full/rxdmtvmlczmg69wkeovx.png" alt="">
				<div class="login__field">
					<i class="login__icon fas fa-user"></i>
					<input type="text" class="login__input" placeholder="Usuário / Email">
				</div>
				<div class="login__field">
					<i class="login__icon fas fa-lock"></i>
					<input type="password" class="login__input" placeholder="Senha">
				</div>
				<button class="btn-login">
					Entrar
					<i class="button__icon fas fa-chevron-right"></i>
				</button>	
                      <div class="links">
                          <router-link class="router-link"><p>Ainda não possui um cadastro?</p></router-link>
                          <router-link class="router-link"><p>Esqueci minha senha</p></router-link>
                      </div>
			</form>
		</div>	
        <div class="line"></div>
        <div class="footer-1">
                <span><b>EFULL</b><i>&copy;</i>  &nbsp;  &nbsp; Todos direitos reservados 2024</span>
        </div>
	</div>
</div>
        
</template>

<style scoped>

 @import url('https://fonts.googleapis.com/css?family=Raleway:400,700');

 .links {
    text-align: center;
    display: flex;
    flex-direction: column;
    font-weight: 300;
    font-size: 14px;
 }

.router-link {
    text-decoration: none !important;
    color: rgb(70, 70, 70);
    transition: 500ms;
}

.router-link:hover{
    opacity: 0.5;
}
.logo {
    max-width: 70px;
}

.container {
    width: 100%;
    height: 100vh;
	display: flex;
	align-items: center;
	justify-content: center;    
}

.screen {		
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
	height: 500px;
	width: 360px;	
    border-radius: 32px;
}







.login {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
	width: 320px;
	padding: 30px; 
    gap: 50px;
}



.login__input {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
	border: none;
	border-bottom: 2px solid #dddddd;
	background: none;
	padding: 10px;
	font-weight: 700;
	width: 100%;
	transition: .2s;
}

.login__input:active,
.login__input:focus,
.login__input:hover {
	outline: none;
	border-bottom-color: #ff7300;
}

.line {
    position: absolute;
    bottom: 80px;
    background: #000000;
    width: 1000%;
    display: flex;
    height: 1px;
    transform: scale(0.1);
}

.footer-1 {
    position: absolute;
    bottom: 0;
    background: #ffffff;
    width: 100%;
    display: flex;
    height: 80px;
    justify-content: center;
    align-items: center;
}

.footer-1 b {
    font-weight:900;
}

.footer-1 i {
    font-size: 10px ;
    position: absolute;
    margin-right:10px ;
}



</style>
    