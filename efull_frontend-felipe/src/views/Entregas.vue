<template>
    <div class="container-caue">
        <div class="menu"></div>
        <div class="menu" style="position: fixed;">
            <div class="brand">
                <img src="https://res.cloudinary.com/daox93pja/image/upload/v1715122906/e-full/rxdmtvmlczmg69wkeovx.png" alt="">
                <p>Efull Dashboard</p>
            </div>
            <div class="line"></div>
            <div class="menu-itens">
                <div class="menu-item-2">
                    <div class="icon-2">
                        <i class="bi bi-house-fill"></i>
                    </div>
                    <router-link aria-current="page" to="/dash">Dashboard</router-link>
                </div>
                <div class="menu-item">
                    <div class="icon">
                        <i class="bi bi-truck"></i>
                    </div>
                    <p>Entregas</p>
                </div>
                <div class="menu-item-2">
                    <div class="icon-2">
                        <i class="bi bi-people-fill"></i>
                    </div>
                    <p>Equipe</p>
                </div>
                <div class="menu-item-2">
                    <div class="icon-2">
                        <i class="bi bi-bar-chart-fill"></i>
                    </div>
                    <p>Desempenho</p>
                </div>
                <div class="menu-item-2">
                    <div class="icon-2">
                        <i class="bi bi-file-earmark-fill"></i>
                    </div>
                    <p>Relatórios</p>
                </div>
                <div class="menu-item-2">
                    <div class="icon-2">
                        <i class="bi bi-geo-alt-fill"></i>
                    </div>
                    <p>Rastreamento</p>
                </div>
            </div>
        </div>

        <div class="dashboard-caue">
            <div class="bar">
                <div class="pages">
                    <div class="q-pages">
                        <p class="pag">Páginas</p>
                        <p>/</p>
                        <p>Entregas</p>
                    </div>
                    <h1>Entregas</h1>
                </div>
                <h1>VJR Logística</h1>
                <p id="data"></p>
                <div class="nav">
                    <nav>
                        <ul>
                            <li><a href=""><i class="bi bi-gear-fill"></i></a></li>
                            <li><a href=""><i class="bi bi-bell-fill"></i></a></li>
                        </ul>
                    </nav>
                </div>
            </div> 
            <div class="table-caue">

                <ul class="responsive-table">
                 <li class="table-header">
                    <div class="col-caue"><h2>Entrega ID</h2></div>
                    <div class="icon-3"><i class="bi bi-upc"></i></div>
                    <div class="col-caue"><h2>Destinatário</h2></div>
                    <div class="icon-3"><i class="bi bi-person-fill"></i></div>
                    <div class="col-caue"><h2>Endereço</h2></div>
                    <div class="icon-3"><i class="bi bi-geo-alt-fill"></i></div>
                    <div class="col-caue"><h2>Data de Saida</h2></div>
                    <div class="icon-3"><i class="bi bi-calendar-check-fill"></i></div>
                    <div class="col-caue"><h2>Status</h2></div>
                    <div class="icon-3"><i class="bi bi-info-circle-fill"></i></div>
                  </li> 
                  <li class="active-caue">
                    <div class="col-caue" data-label="shipping Id">42235</div>
                    <div class="col-caue" data-label="Customer Name">Enrico Vinicus</div>
                    <div class="col-caue" data-label="Endress">Rua Christian Aráujo Costa, 1442</div>
                    <div class="col-caue" data-label="Amount">14/04/2024</div>
                    <div class="col-caue yellow" data-label="Payment Status">Pendente</div>
                  </li>
                  <li class="">
                    <div class="col-caue" data-label="Job Id">42442</div>
                    <div class="col-caue" data-label="Customer Name">Evoly LTDA</div>
                    <div class="col-caue" data-label="Endress">Rua Alves de Souza, 365</div>
                    <div class="col-caue" data-label="Amount">13/04/2024</div>
                    <div class="col-caue yellow" data-label="Payment Status">Pendente</div>
                  </li>
                  <li class="active-caue">
                    <div class="col-caue" data-label="Job Id">42257</div>
                    <div class="col-caue" data-label="Customer Name">Felipe Cauê</div>
                    <div class="col-caue" data-label="Endress">Rua Valdir Junior Pererira, 25</div>
                    <div class="col-caue" data-label="Amount">12/04/2024</div>
                    <div class="col-caue red" data-label="Payment Status">devolvida</div>
                  </li>
                  <li class="">
                    <div class="col-caue" data-label="Job Id">42311</div>
                    <div class="col-caue" data-label="Customer Name">Caio Sartunino</div>
                    <div class="col-caue" data-label="Endress">Rua Felipe Humilde Araujo, 777</div>
                    <div class="col-caue" data-label="Amount">11/04/2024</div>
                    <div class="col-caue green" data-label="Payment Status">Entregue</div>
                  </li>
                </ul>
              </div>
            </div>
        </div>
</template>

<style scoped> 
@import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100..900;1,100..900&display=swap');

* {
    padding: 0;
    margin: 0;
    font-family: "Raleway", sans-serif;
}



body {
  background: #f1f1f1;
}



.carousel-inner img {
  border-radius: 32px;
}

.carousel-inner {
  width: auto;
  height: auto;
  border-radius: 32px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

#carouselExampleSlidesOnly {
  margin-bottom: 10%;
}

.btn-login {
    width: auto;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 20px;
    background-image: linear-gradient( to right, #FF0000, #FFC000);
    border: none;
    color: rgb(255, 255, 255);
    padding: 4px 20px;
    font-size: 16px;
    font-weight: 600;
    cursor: pointer;
    margin-left: 10px;
    transition: 500ms;
}

.btn-login:hover {
    opacity: 0.5;
}

.btn:hover  {
    color: #b40000;
}

.title-gradient {
    background-image: linear-gradient(to right, #FF0000, #FF8000, #FFC000);
    background-clip: text;  
    -webkit-text-fill-color: transparent; 
    color: transparent;    
}
.text-box {
    margin: 10% 0 7% 0;
    display: flex;
    flex-direction: column;
}

.text-box h1 {
    font-size: 3.3em; 
    font-weight: 800;
}

.card {
    overflow: hidden;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    display: flex;
    flex-direction: column;
    position: relative;
    width: 300px;
    height: 300px;
    border-radius: 64px;
    overflow: hidden;
    background-color: #f8f9fa;
}

.bg-1 {

    background-color: #212529;
}

  .container-sm {
    display: flex;
    flex-direction: column;
    gap: 22px;
  }

  .card img {
    max-width: 100px;
  }



.aviso {
    display: flex;
    justify-content: left;
    align-items: center;
    margin-top: 10%;
    width: 100%;
    padding: 15px;
    border-radius: 32px;
    gap: 20px;
}

.aviso h7 {
    max-width: 800px;
}

.aviso i {
    font-size: 3rem;
}

.footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 10%;
    display: flex;
    padding: 10% 0% 5% 0%;
    background-color: #f8f9fa;
    border-top: 1px solid #e5e5e5;
  }
  
  .footer > * {
    flex:  1 100%;
  }
  
  .footer__addr {
    width: auto;
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin-bottom: 2em;
  }


  .footer img {
    max-width: 90px;
    margin-bottom: 30px;
  }
  
  .footer__addr h2 {
    margin-top: 1.3em;
    font-size: 15px;
    font-weight: 400;
  }
  
  .nav__title {
    font-weight: bold;
    font-size: 15px;
  }
  
  .footer address {
    font-style: normal;
  }
  
  .footer ul {
    list-style: none;
    padding-left: 0;
  }
  
  .footer li {
    line-height: 2em;
  }
  
  .footer a {
    text-decoration: none;
  }
  
  .footer__nav {
    display: flex;
    justify-content: space-between;
  }
  
  .footer__nav > * {
    flex: 1 50%;
    margin-right: 1.25em;
  }
  
  .nav__ul a {
    color: #212529;
  }
  
  .nav__ul--extra {
    column-count: 2;
    column-gap: 1.25em;
  }
  
  .copy {
    gap: 30px;
    background-color: #f8f9fa;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    width: 100%;
  }
    
 
  
  .heart {
    color: #2f2f2f;
  }
  
  @media screen and (min-width: 24.375em) {
    .legal .legal__links {
      margin-left: auto;
    }
  }
  
  @media screen and (min-width: 40.375em) {
    .footer__nav > * {
      flex: 1;
    }
    
    .nav__item--extra {
      flex-grow: 2;
    }
    
    .footer__addr {
      flex: 1 0px;
    }
    
    .footer__nav {
      flex: 2 0px;
    }
  }

  .branding {
    max-width: 100%;
    display: flex;
    align-items: center;
    gap: 100px;
  }
  
  .branding img {
    max-width: 500px;
  }



  .text-box a {
    color: #212529;
    font-size: 20px;
    text-decoration: none;
    transition: 1s;
  }

.text-box a:hover {
  color: #929394;
  text-decoration: underline;
}

  .branding  h1 {
    margin-left: 10px;
    font-size: 52px;
    font-weight: 800;
    max-width: 600px;
  }

  .branding p {
    margin-left: 10px;
    max-width:450px;
  }

  /*Dash*/


.menu {
    width: 20%;
    height: 100vh;
    position: relative;
    display: flex;
    align-items: center;
    flex-direction: column;
}

.brand {
    width: 100%;
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 18px;
    font-weight: bold;
    color: #4c4c4c;
}

.brand img {
    max-width: 35px;
    max-height: 35px;
}

.line {
    margin-bottom: 30px;
    width: 800%;
    height: 1px;
    background-image: linear-gradient(to left, rgba(255, 255, 255, 0), black, black,  rgba(255, 255, 255, 0));
    transform: scale(0.1);
}

.menu-itens {
    width: 100%;
    height: auto;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
    gap: 30px;
}

.menu-item {
    position: relative;
    padding: 16px;
    gap: 18px;
    width: 60%;
    border-radius: 16px;
    background-color: #f8f9fa;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    justify-content: left;
    align-items: center;
    display: flex;
}

.icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 30px;
    height: 30px;
    background-color: #FF0000;
    border-radius: 8px;
    color: white;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}



.menu-item-2 {
    position: relative;
    padding: 16px;
    gap: 18px;
    width: 60%;
    border-radius: 16px;
    justify-content: left;
    align-items: center;
    display: flex;
}

.icon-2 {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 30px;
    height: 30px;
    background-color: #f8f9fa;
    border-radius: 8px;
    color: rgb(29, 29, 29);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.container-caue {
    display: flex;
    position: relative;
    width: 100%;
}

.dashboard-caue {
    width: 80%;
    height: auto;
    position: relative;
    display: flex;
    flex-direction: column;
    padding: 50px;
    gap: 40px;
}

.q-pages {
    display: flex;
    gap: 8px;
}

.pag {
    color: #828181;
}

.bar {
    align-items: center;
    display: flex;
    justify-content: space-between;
}

nav ul li {
    list-style: none;
}

nav ul li a {
    color: #4c4c4c;
    font-size: 18px;
}

nav ul {
    display: flex;
    gap: 30px;
}

.info {
    width: 100%;
    justify-content: space-around;
    align-items: center;
    position: relative;
    display: flex;
    gap: 30px;
}

.card-info {
    position: relative;
    padding: 20px;
    width: 30%;
    height: auto;
    display: flex;
    justify-content: space-between;
    border-radius: 32px;
    background-color: #f8f9fa;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.green {
    color: green;
}

.red {
    color: red;
}

.infos {
    flex-direction: column;
    display: flex;
    gap: 40px;
}

.c-text {
    width: 60%;
    flex-direction: column;
    display: flex;
    gap: 15px;
}

.c-text p {
    font-size: 1.2rem;
}

.data {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

#data {
    width: 200px;
}


.number {
    justify-content: left;
    align-items: center;
    display: flex;
    gap: 20px;
    font-size: 18px;
}

.icon-3 {
    background-image: linear-gradient(to right, #FF0000, #FF8000, #FFC000);
    color: white;  
    display: flex;
    justify-content: center;  
    align-items: center;
    width: 50px;
    height: 50px;
    border-radius: 16px;
    font-size: 20px; 
}

.col-caue {
    justify-content: center;
    align-items: center;
    display: flex;
  }
  
  

.col h2 {
    font-weight: 400;
    font-size: 17px;
}

.info-icon {
    background-image: linear-gradient(to right, #FF0000, #FF8000, #FFC000);
    color: white;  
    display: flex;
    justify-content: center;  
    align-items: center;
    width: 60px;
    height: 60px;
    border-radius: 16px;
    font-size: 24px;
}

.info-icon-2 {
    color: rgb(19, 18, 18);  
    display: flex;
    justify-content: center;  
    align-items: center;
    width: 40px;
    height: 40px;
    border-radius: 16px;
    font-size: 14px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}




.congrats {
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 60%;
    border-radius: 32px;
    height: 80%;
    padding: 30px;
    background-color: #212529;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.graph {
    text-align: left;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 40%;
    border-radius: 32px;
    padding: 30px;
    height: 80%;
    background: #f8f9fa;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.g-box {
    position: relative;
    width: 100%;
    display: flex;
    flex-direction: column;
    text-align: left;
    gap: 20px;
    font-weight: 300;
}

a {
    text-decoration: none;
    color: #212529;
}

.c-box {
    align-items: center;
    width: 100%;
    height: 100%;
    display: flex;
    overflow: hidden;
    gap: 30px;
}

.c-icon {
    background-image: linear-gradient(to right, #FF0000, #FF8000, #FFC000);
    color: white;  
    display: flex;
    justify-content: center;  
    align-items: center;
    width: 200px;
    height: 200px;
    border-radius: 16px;
    font-size: 84px;
}

.title {
    font-weight: 800;
}

svg {
    margin: 0 auto;
    text-align: center;
    width: 100%;
    padding-top: 40px;
  }
  
  polyline {
    stroke-dasharray:  1000;
    stroke-dashoffset: 1000;
    animation: dash 4s ease-in forwards;
    animation-iteration-count: 1;
  }
  
  @keyframes dash {
    to {
      stroke-dashoffset: 0;
    }
  }

  .text {
    animation: moveRightToLeft 10s linear infinite;
    height: 20px;
    text-wrap: nowrap;
  }
  
.t-box {
    overflow: hidden;
}

.marquee-container {
    width: 80%;
    overflow: hidden;
  }
  
  .marquee {
    white-space: nowrap;
    animation: marquee 10s linear infinite;
  }
  
  @keyframes marquee {
    0% { transform: translateX(0); }
    100% { transform: translateX(-100%); }
  }

  @keyframes moveRightToLeft {
    0% {
      transform: translateX(100%);
    }
    100% {
      transform: translateX(-100%);
    }
  }

  h3 {
    font-weight: 400;
  }

  .g-box b {
    margin-left: 20px;
  }

  .g-icon {
    position: absolute;
    font-size: 24px;
    display: flex;
    gap: 24px;
    right: 0;
    flex-direction: column;
    cursor: pointer;
  }

  .responsive-table li {
    padding: 35px 40px;
    display: flex;
    justify-content: space-between;
  }
  
  .responsive-table .table-header {
    font-size: 14px;
    letter-spacing: 0.03em;
    border-radius: 32px 32px 0px 0px;
  }

  .table-caue {
    background-color: #f8f9fa;
    border-radius: 32px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  
  
  
  @media all and (max-width: 767px) {
    .responsive-table .table-header {
      display: none;
    }
    .responsive-table li {
      display: block;
    }
    .responsive-table .col {
      flex-basis: 100%;
      display: flex;
      padding: 10px 0;
    }
    .responsive-table .col:before {
      padding-right: 10px;
      content: attr(data-label);
      flex-basis: 50%;
      text-align: right;
    }
  }

  .yellow{
    color: #ffbf00;
  }

  .line-2 {
    width: 100%;
    height: 1px;
    background-color: #4c4c4c;
  }

  .active-caue  {
    background-color: #f1f1f1;
    border-radius: 0px !important;
  }



  
 
  


  
</style>
