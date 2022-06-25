<template>
  <v-container>
    <v-app-bar
      app
      elevate-on-scroll
    >
      <v-toolbar-side-icon>
            <v-img class="mr-3" src="logoGerenciei _navbar.png" height="60px" width="60px"/> 
     </v-toolbar-side-icon>
      <v-toolbar-title
        class="hidden-sm-and-down"
      >Gerenciei.com</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        v-for="icon in icons"
        :key="icon"
        :href="icon.href"
        class="mx-4"
        color="#8600FF"
        icon
      >
        <v-icon size="24px">
          {{ icon.icon }}
        </v-icon>
      </v-btn>
    </v-app-bar>
    <v-img
      src="capa_home.svg"
    >
      <div class="capa_text">
        <div class="capa_text_in">
          <h2>Em breve</h2>
          <h1 class="font-weight-bold">Gerenciei.com</h1>
          <h3>O seu novo jeito de gerenciar</h3>
          <v-btn rounded block color="#FDA100" href="#anchorBtnBanner">Nós conheça</v-btn>
        </div>
      </div>
    </v-img>


    <!--INI - BANNER WITH 920PX LOW-->
    <v-img
      src="capa_home.svg"
    >
      <div class="capa_text">
        <div class="capa_text_in">
          <h2>Em breve</h2>
          <h1 class="font-weight-bold">Gerenciei.com</h1>
          <h3>O seu novo jeito de gerenciar</h3>
          <v-btn rounded block color="#FDA100" href="#anchorBtnBanner">Nós conheça</v-btn>
        </div>
      </div>
    </v-img>

    <!--END - BANNER WITH 920PX LOW-->


    <br><br><br><br><br><br>
    <v-row justify="center" id="anchorBtnBanner">
        <h1 class="display-1">Com o <b style="color:#FDA100">Gerenciei.com</b> você terá acesso a indicadores financeiros que te guiarão, fazendo seu negócio decolar! </h1>
    </v-row>
    <br><br><br><br><br>
    <v-row>
      <v-col cols="12" align-self="center" >
        <v-card
          elevation="2"
          outlined
          shaped
          
        >
        <v-card-text >
          <div class="headline" >
            O <b style="color:#FDA100">Gerenciei.com</b> é uma plataforma de inovação tecnológica, educação e gestão financeiras
            que permite aos pequenos e médios empresários a tomar decisões importantes com informações financeiras
            atualizadas e precisas sobre seu negócio
          </div>
        </v-card-text>
        </v-card>
      </v-col>
        <v-col cols="sm">
          <v-card
            elevation="2"
            outlined
            style="background-color:#654F79"
            shaped
          > 
          <v-img
            height="250"
            src="semGerenciei.png"
            contain
          ></v-img>
          <v-card-text>
            <div class="headline" style="color: white;">
              <b>SEM</b> o <b style="color:#FDA100">Gerenciei.com</b> é muito fácil se perder e acabar errando nas suas tomadas de 
              decições perdendo assim o seu potêncial de crescimento
            </div>
          </v-card-text>
        </v-card>   
      </v-col>
      <v-col cols="sm">
        <v-card
          elevation="2"
          outlined
          style="background-color:#8600FF"
          shaped
        >
          <v-img
            height="250"
            src="comGerenciei.png"
            contain
          ></v-img>
          <v-card-text>
            <div class="headline" style="color: white;">
              <b>COM</b> o <b style="color:#FDA100">Gerenciei.com</b> você terá em suas mãos índices financeiros poderosos que te 
              ajudarão a potêncializar o seu crescimento
            </div>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <br><br><br><br><br><br>
    <v-row justify="center">
      <v-col cols="sm">
        <v-text class="display-1">
          Com o <b style="color:#FDA100">Gerenciei.com</b> você só terá que colocar suas informações e deixar que nossa mágica aconteca
        </v-text>
        <br>
        <v-text class="headline">
          Não perca seu tempo estudando calculos financeiros e foque sua atenção exclusivamente no seu negócio! 
        </v-text>
      </v-col>
    </v-row>
    <br><br><br><br><br><br>
    <v-row style="background-color:#FFDDA1">
      <v-col cols="12" >
        <v-text style="color:#8600FF;align-items: center;" class="display-1">
          <b>O que o Gerenciei.com tem a te oferecer</b>
        </v-text>
      </v-col>
      <v-col cols="sm">
        <v-expansion-panels
        
          v-model="panel"
        >
          <v-expansion-panel @click="onExpansionPanelClick($event,1)">
            <v-expansion-panel-header>Painéis intuitivos</v-expansion-panel-header>
              <v-expansion-panel-content>
                Cansado de ficar perdendo seu valioso tempo procurando tal funcionalidade em meio a paíneis bagunçados?<br>
                Aqui na <b style="color:#FDA100">Gerenciei.com</b> todas as informações ficam a um clique de distância e são extremamente sintetizados
                para você ter só oque realmente quer.<br>
                Os nossos paíneis e indicadores foram contruídos e projetados para
                que se adeguem automáticamente em todos os tamanhos de telas, fazendo que você possa acessar em qualquer tipo
                de disposítivo conectado a internet!
              </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel @click="onExpansionPanelClick($event,2)">
            <v-expansion-panel-header>Multi canais de suporte</v-expansion-panel-header>
              <v-expansion-panel-content>
                Ficou com alguma dúvida ou está se sentindo meio perdido? <br>
                Não se preocupe! Aqui na <b style="color:#FDA100">Gerenciei.com</b> possuímos multi-canais de suporte para você
                entrar em contato conosco e tirar suas dúvidas ou receber orientações com nossos especialistas.<br>
                Se sua dúvida for simples você poderá tirar sua dúvida com o Jorge, nossa inteligência aritifical que irá sanar suas dúvidas na hora,
                mas caso a sua dúvida seja mais complexa, você poderá abrir um ticket de atendimento* para ser atendido por um de nossos
                especialistas!
                <br>
                <i style="font-size:70%">*Tickets limitados de acordo com o plano de assinatura</i>
              </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel @click="onExpansionPanelClick($event,3)">
            <v-expansion-panel-header>Educação</v-expansion-panel-header>
              <v-expansion-panel-content>
                Está curioso para saber como funciona este mundo da contabilidade financeira?<br>
                A <b style="color:#FDA100">Gerenciei.com</b> está sempre preocupada com a educação e nossa responsabilidade social
                é divulgar e ensinar aos empresários os paradigmas da contabilidade financeira e como ela funciona. E todos os nossos índices
                contém o seu embasamento teórico para que você possa aprender de onde veio as informações e como elas podem ser úteis!<br>
                E fique ligado nas nossas redes sociais que sempre estamos postando conteúdo educacional gratuito e de qualidade! 
              </v-expansion-panel-content>
          </v-expansion-panel>
          <v-expansion-panel @click="onExpansionPanelClick($event,4)">
            <v-expansion-panel-header>Inteligência Artificial</v-expansion-panel-header>
              <v-expansion-panel-content> 
                Já pensou em ter sua própria inteligência artificial te ajudando a gerir o seu negócio?<br>
                Nós da <b style="color:#FDA100">Gerenciei.com</b> te proporcionamos essa chance! Quando você assina qualquer um de
                nossos planos você será automáticamente auxiliado pela nossa inteligência artificial e quanto mais você usar mais ela
                aprenderá com os dados que você inserir e mais personalizada ela se tornará! 
              </v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </v-col>
      <v-col cols="6" class="d-none d-sm-none d-md-none d-lg-flex d-xl-flex">
        <v-card >
          <v-img
            v-if="painel1"
            src="photoPainel1.png"
          />
          <v-img
            v-if="painel2"
            src="photoPainel2.png"
          />
          <v-img
            v-if="painel3"
            src="photoPainel3.png"
          />
          <v-img
            v-if="painel4"
            src="photoPainel4.png"
          />
        </v-card>
      </v-col>
    </v-row>
    <br><br><br><br><br><br>
    <v-row>
      <v-col cols="12">
        <v-text class="display-1">
          O <b style="color:#FDA100">Gerenciei.com</b> será lançado em breve estamos trabalhando com carinho e dedicão para entregar o melhor sempre!<br>
        </v-text>
        <v-text class="headline">
         Confira abaixo em qual estágio a gente se encontra 
        </v-text>
      </v-col>
      <v-col cols="12">
        <v-stepper alt-labels>
          <v-stepper-header>
            <v-stepper-step step="1" complete>
              Desenvolvimento
            </v-stepper-step>
            <v-divider></v-divider>
            <v-stepper-step step="2">
              Testes
            </v-stepper-step>
            <v-divider></v-divider>
            <v-stepper-step step="3">
              Alpha
            </v-stepper-step>
            <v-divider></v-divider>
            <v-stepper-step step="4">
              Beta
            </v-stepper-step>
            <v-divider></v-divider>
            <v-stepper-step step="5">
              Lançamento
            </v-stepper-step>
          </v-stepper-header>
        </v-stepper>
      </v-col>
    </v-row>
    <br><br><br><br><br><br>
    <v-row>
      <v-col cols="12">
        <v-text class="display-1">
          Se interessou e quer nós acompanhar de pertinho?<br>
        </v-text>
        <v-text class="headline">
          Nós siga nas nossas redes sociais e preencha o formulário abaixo para receber as informações em primeira mão!
        </v-text>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12">
         <v-alert
            shaped
            dark
            color="info"
            v-if="emailSuccess"
          >
            E-mail enviado com sucesso!!
          </v-alert>
          <v-alert
            shaped
            prominent
            type="error"
            v-if="emailError"
          >
           Ocorreu um erro ao enviar o e-mail, porfavor tente novamente mais tarde.
          </v-alert>
        <v-card
          elevation="4"
        >
          <v-form v-model="valid" ref="form" @submit.prevent="sendEmail">
            <v-container>
              <v-row>
                <v-col
                  cols="12"
                  md="4"
                >
                  <v-text-field
                    v-model="firstname"
                    :rules="nameRules"
                    :counter="50"
                    label="Nome"
                    required
                  ></v-text-field>
                </v-col>

                <v-col
                  cols="12"
                  md="4"
                >
                  <v-text-field
                    v-model="lastname"
                    :rules="nameRules"
                    :counter="50"
                    label="Sobrenome"
                    required
                  ></v-text-field>
                </v-col>

                <v-col
                  cols="12"
                  md="4"
                >
                  <v-text-field
                    v-model="email"
                    :rules="emailRules"
                    label="E-mail"
                    required
                  ></v-text-field>
                </v-col>
              </v-row>
              <v-btn
                class="mr-4"
                @click="sendEmail()"
                :disabled="!this.valid"
                color="#8600FF"
              >Enviar</v-btn>
            </v-container>
          </v-form>
        </v-card>
      </v-col>
    </v-row>
    <br><br><br><br><br><br>
    <v-footer
      dark
      padless
    >
      <v-card
        class="flex"
        flat
        tile
      >
        <v-card-title style="background-color:#8600FF">
          <strong class="subheading">Fique conectado com a gente nas redes sociais!</strong>

          <v-spacer></v-spacer>

          <v-btn
            v-for="icon in icons"
            :key="icon.href"
            class="mx-4"
            dark
            icon
          >
            <v-icon size="24px">
              {{ icon.icon }}
            </v-icon>
          </v-btn>
        </v-card-title>

        <v-card-text class="py-2 white--text text-center">
          {{ new Date().getFullYear() }} — <strong>Gerenciei.com</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-container>



  <!--Modal de E-mail enviado com sucesso-->
</template>

<style>
  
  
  /* .capa_text{
    width: 70%;
    height: 50%;
  }
  .capa_text_in{
    padding-left:30%;
    padding-right: 30%;
    padding-top: 10%;
  }
  .capa_text_in h1, h2, h3{
    text-align: center;
    
  }
  .capa_text_in h2, h3{
    color:white;
    font-size: 30px;
  }
  .capa_text_in h1{
    color:#FDA100;
    font-size: 50px;
  }

  .capa_text_in v-btn{
    align-content: center;
  } */

 
  /* Extra small devices (phones, 600px and down) */
  @media only screen and (max-width: 600px) {
    .capa_text {
      width: 100%;
      height: 200px;
    }
    .capa_text_in{
      padding:2%;
    }
    .capa_text_in h1, h2, h3{
      text-align: center;
    
    }
    .capa_text_in h2, h3{
      color:white;
      font-size: 20px;
    }
    .capa_text_in h1{
      color:#FDA100;
      font-size: 25px;
    }
  }

  /* Small devices (portrait tablets and large phones, 600px and up) */
  @media only screen and (min-width: 600px) {
    .capa_text {
      width: 80%;
      height: 200px;
    }
    .capa_text_in{
      padding-left:10%;
      padding-right: 25%;
      padding-top: 3%;
    }
    .capa_text_in h1, h2, h3{
      text-align: center;
    }
    .capa_text_in h2, h3{
      color:white;
      font-size: 20px;
    }
    .capa_text_in h1{
      color:#FDA100;
      font-size: 25px;
    }
  }

  /* Medium devices (landscape tablets, 768px and up) */
  @media only screen and (min-width: 768px) {
    .capa_text {
      width: 60%;
      height: 200px;
    }
    .capa_text_in{
      padding-left:20%;
      padding-right: 20%;
      padding-top: 8%;
    }
    .capa_text_in h1, h2, h3{
      text-align: center;
      
    }
    .capa_text_in h2, h3{
      color:white;
      font-size: 20px;
      text-align: center;
    }
    .capa_text_in h1{
      color:#FDA100;
      font-size: 25px;
    }
  }

  /* Large devices (laptops/desktops, 992px and up) */
  @media only screen and (min-width: 992px) {
    .capa_text {
      width: 80%;
      height: 200px;
    }
    .capa_text_in{
      padding-left:15%;
      padding-right: 30%;
      padding-top: 3%;
    }
    .capa_text_in h1, h2, h3{
      text-align: center;
      
    }
    .capa_text_in h2, h3{
      color:white;
      font-size: 21px;
    }
    .capa_text_in h1{
      color:#FDA100;
      font-size: 40px;
    }
  }

  /* Extra large devices (large laptops and desktops, 1200px and up) */
  @media only screen and (min-width: 1200px) {
    .capa_text {
      width: 60%;
      height: 100%;
    }
    .capa_text_in{
      padding-left:30%;
      padding-right: 30%;
      padding-top: 10%;
    }
    .capa_text_in h1, h2, h3{
      text-align: center;
      
    }
    .capa_text_in h2{
      color:white;
      font-size: 30px;
    }
    .capa_text_in h3{
      color:white;
      font-size: 21px;
    }
    .capa_text_in h1{
      color:#FDA100;
      font-size: 40px;
    }
  }
</style>


<script lang="js">
  import emailjs from '@emailjs/browser';
  export default {
    name: 'IndexPage',
    data:()=>{
      return{
        panel:0,
        painel1:true,
        painel2:false,
        painel3:false,
        painel4:false,
        readonly: false,
        valid: false,
        firstname: '',
        lastname: '',
        nameRules: [
          v => !!v || 'Name é obrigatório',
          v => v.length <= 50 || 'O nome deve ser menor que 50 caracteres',
        ],
        email: '',
        emailRules: [
          v => !!v || 'E-mail é obrigatório',
          v => /.+@.+/.test(v) || 'O e-mail deve ser válido',
        ],
        icons: [
          {
            icon:'mdi-facebook',
            href:'https://www.facebook.com/Gerencieicom-109825071747769'
          },
          {
            icon:'mdi-linkedin',
            href:'https://www.linkedin.com/company/gerenciei-com/about/'
          },
          {
            icon:'mdi-instagram',
            href:'https://instagram.com/gerenciei_com?igshid=YmMyMTA2M2Y='
          },
          {
            icon:'mdi-youtube',
            href:''
          }
        
      ],
      emailError:false,
      emailSuccess:false
      }
  },
  methods:{
    onExpansionPanelClick(event,numPainel) {
      if(!event.currentTarget.classList.contains('v-expansion-panel-header--active')) {
        switch (numPainel){
          case 1:
            this.painel1 = true
            this.painel2 = false
            this.painel3 = false
            this.painel4 = false
            break;
          case 2:
            this.painel1 = false
            this.painel2 = true
            this.painel3 = false
            this.painel4 = false
            break;
          case 3:
            this.painel1 = false
            this.painel2 = false
            this.painel3 = true
            this.painel4 = false
            break;
          case 4:
            this.painel1 = false
            this.painel2 = false
            this.painel3 = false
            this.painel4 = true
            break;
          default:
            break;
        }
      }
    },
    sendEmail() {
      try {
        emailjs.send('service_lfoiev6', 'template_rqhkyp9',
        {
          from_name: `${this.firstname} ${this.lastname}`,
          from_email: this.email,
        },'dza2dyaGEwMQxLSMl')
      
        this.emailSuccess = true
        setTimeout(function(){ this.emailSuccess = false }, 3000);
      } catch(error) {
        this.emailError = true
        setTimeout(function(){ this.emailError = false }, 3000);
        console.log({error})
      }
      // Reset form field
      this.name = ''
      this.email = ''
    },
  }
}
</script>
