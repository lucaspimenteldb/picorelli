<template>
  <v-app>
    <!-- Hero Section -->
    <v-container
      fluid
      class="hero-section pa-0"
    >
      <v-row no-gutters>
        <v-col cols="12">
          <v-img
            src="@/assets/hero-banner.png"
            cover
            class="position-relative"
          >
            <v-container class="fill-height pb-16">
              <v-row align="center">
                <v-col 
                  cols="12"
                  md="9"
                  class="px-6"
                >
                  <img
                    src="@/assets/logo.png"
                    max-width="90"
                    width="90"
                    alt="Arena Pionelli"
                    class="position-relative mb-12"
                  >
                  <h1 class="d-print-block mt-16 text-h4 text-md-h2 font-weight-bold text-center text-md-left text-white mb-4 text-fjalla">
                    SEJA UM ATLETA FUNDADOR DA <span class="text-yellow">ARENA PIONELLI</span>
                  </h1>
                  <p class="mt-2 mb-10 text-center text-md-left text-white text-body-2">
                    Na Arena Picorelli, acreditamos que todo ser humano carrega um atleta dentro de si , aquele que luta, que cai e levanta, que dá o primeiro passo mesmo com medo.
                    Por isso, abrimos as portas para a nossa primeira turma oficial. E ela vai carregar um nome especial: <span class="text-yellow">Os Atletas Fundadores.</span>
                  </p>
                  <v-btn
                    color="yellow"
                    size="large"
                    class="mx-auto mx-md-0 d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
                  >
                    Quero este plano
                  </v-btn>
                </v-col>
              </v-row>
            </v-container>
          </v-img>
        </v-col>
      </v-row>
    </v-container>

    <!-- Features Section -->
    <v-container class="pt-12">
      <v-row>
        <v-col
          cols="12"
          md="6"
          class="d-flex flex-column align-center"
        >
          <v-img
            src="@/assets/colagem-1.png"
            max-width="300"
            width="100%"
            contain
          />
        </v-col>
        <v-col
          cols="12"
          md="6"
        >
          <h2 class="mt-16 text-h6 text-md-h4 font-weight-bold mb-4 text-center text-md-left text-fjalla">
            QUEM COMEÇA COM A GENTE, <br> LIDERA COM A GENTE
          </h2>
          <p class="text-center text-md-left mb-6 text-body-2 font-weight-medium text-grey-51">
            Antes de existir uma estrutura, existe uma visão. <br>E são os primeiros que tornam essa visão realidade.
          </p>
          <!-- class="d-flex flex-column justify-center" -->
          <div class="mx-auto mx-md-0 w-300">
            <div
              v-for="(feature, index) in features"
              :key="index"
              class="mx-sm-6 mx-md-0 d-flex align-center mb-4"
            >
              <v-img
                src="@/assets/check-border.png"
                width="18"
                max-width="18"
              />
              <span class="ml-2 text-body-2 text-grey-51">{{ feature }}</span>
            </div>
          </div>
          <v-btn
            color="yellow"
            size="large"
            class="mt-8 mx-auto mx-md-0 d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
          >
            QUERO SER FUNDADOR
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    <!-- Training Options Section -->
    <v-container class="py-12">
      <v-row>
        <v-col
          cols="12"
          class="text-center mb-4"
        >
          <h2 class="mt-16 text-h6 text-md-h4 font-weight-bold mb-4 text-center text-fjalla">
            PARA QUEM BUSCA MAIS DO QUE TREINO
          </h2>
          <p class="text-center mb-6 text-body-2 font-weight-medium text-grey-51">
            Se você quer resultado, motivação e compromisso com sua evolução, aqui é o lugar.
          </p>
        </v-col>
      </v-row>
      <v-row class="d-flex">
        <v-col
          v-for="(option, index) in trainingOptions"
          :key="index"
          cols="12"
          sm="6"
          md="3"
          class="mb-4 text-center d-flex justify-center"
        >
          <v-card
            width="220"
            flat
          >
            <v-avatar
              size="120"
              class="mb-4"
            >
              <v-img
                :src="option.image"
                cover
              />
            </v-avatar>
            <h3 class="text-h6 font-weight-bold mb-2 text-military-green text-fjalla">
              {{ option.title }}
            </h3>
            <p class="text-body-2">
              {{ option.description }}
            </p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <!-- Facility Section -->
    <v-container
      fluid
      class="py-12 bg-grey-73"
    >
      <v-row no-gutters>
        <v-col
          cols="12"
          md="5"
          class="text-center mb-4"
        >
          <h2 class="text-h6 text-md-left text-md-h2 font-weight-bold mb-4 text-center text-fjalla">
            A ESTRUTURA QUE INSPIRA, DESAFIA E TRASFORMA
          </h2>
          <p class="text-center text-md-left mb-6 text-body-2 font-weight-medium">
            Nossa estrutura foi pensada para proporcionar performance, conforto e motivação. Da iluminação ao som, dos equipamentos à energia da equipe — tudo aqui te convida a dar o seu melhor. A <span class="text-yellow font-weight-bold">Arena Picorelli</span> não é uma academia comum. É um ambiente criado para te transformar, por dentro e por fora.
          </p>
        </v-col>
        <v-col
          cols="12"
          md="7"
          class="d-flex align-center justify-center"
        >
          <v-img
            src="@/assets/video-preview.png"
            width="100%"
            max-width="450"
            cover
            class="mx-auto"
          />
        </v-col>
      </v-row>
    </v-container>

    <!-- Benefits Section -->
    <v-container class="py-12">
      <v-row>
        <v-col
          cols="12"
          md="8"
          offset-md="2"
          class="text-center mb-8"
        >
          <h2 class="text-h6 text-md-h4 font-weight-bold mb-4 text-center text-fjalla">
            QUEM CHEGA PRIMEIRO RECEBE MAIS
          </h2>
          <p class="text-center mb-4 text-body-2 font-weight-medium">
            Conheça os benefícios exclusivos de ser um Atleta Fundador da <b class="text-military-green">Arena Picorelli</b>, vantagens reais para quem acredita desde o começo.
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(benefit, index) in benefits"
          :key="index"
          cols="12"
          md="6"
          class="text-center d-flex justify-center"
        >
          <v-card
            width="270"
            flat
            class="mb-8"
          >
            <v-img
              :src="benefit.image"
              cover
              class="mb-8"
            />
            <h3 class="text-h6 font-weight-bold mb-2 text-fjalla text-military-green">
              {{ benefit.title }}
            </h3>
            <p class="text-body-2 text-grey-51">
              {{ benefit.description }}
            </p>
          </v-card>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          cols="12"
          class="text-center mt-2"
        >
          <v-btn
            color="yellow"
            size="large"
            class="mx-auto d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
          >
            garantir minha vaga agora
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    <!-- Limited Spots Section -->
    <v-container
      fluid
      class="bg-grey-73 py-16"
    >
      <v-row>
        <v-col
          cols="12"
          md="4"
          offset-md="2"
          class="text-center"
        >
          <h2 class="text-h6 text-md-left text-md-h2 font-weight-bold mb-4 text-center text-fjalla">
            VAGAS LIMITADAS!
          </h2>
          <p class="text-center text-md-left mb-4 text-body-2 font-weight-medium">
            A <b class="text-yellow">Arena Picorelli</b> está abrindo um número exclusivo de vagas para Atletas Fundadores. Seja um dos primeiros a garantir sua posição. Depois que fechar, não volta.
          </p>
          <div class="mt-16 mb-4 d-flex justify-center">
            <div class="text-center mx-6">
              <div class="text-h2 font-weight-bold text-fjalla">
                100+
              </div>
              <div class="mt-2 text-body-2">
                VAGAS RESERVADAS
              </div>
            </div>
            <div class="text-center mx-6">
              <div class="text-h2 font-weight-bold text-yellow text-fjalla">
                180
              </div>
              <div class="mt-2 text-body-2">
                VAGAS RESERVADAS
              </div>
            </div>
          </div>
          <v-img
            src="@/assets/colete.png"
            max-width="300"
            class="d-md-none mt-16 mb-8 mx-auto position-relative"
          />
          <v-btn
            color="yellow"
            size="large"
            class="mx-auto d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
          >
            garantir minha vaga agora
          </v-btn>
        </v-col>
        <v-col
          cols="4"
          class="d-none d-md-flex"
          offset-md="1"
        >
          <v-img
            src="@/assets/colete.png"
            max-width="350"
            class=" mt-16 mb-8 mx-auto position-relative"
          />
        </v-col>
      </v-row>
    </v-container>

    <!-- Pricing Section -->
    <v-container class="py-12">
      <v-row>
        <v-col
          cols="12"
          md="8"
          offset-md="2"
          class="mt-md-12 text-center mb-8"
        >
          <p class="mb-2 font-weight-medium text-grey-73">
            • 1º Lote de 3 •
          </p>
          <h2 class="text-h6 text-md-h4 font-weight-bold mb-4 text-center text-fjalla">
            ESCOLHA COMO FAZER PARTE DESSE LEGADO
          </h2>
          <p class="text-center mb-4 text-body-2 font-weight-medium text-grey-51">
            Seja um Atleta Fundador da <b class="text-military-green">Arena Picorelli</b> com o plano que mais combina com seu momento. Todos com acesso completo aos benefícios exclusivos.
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(plan, index) in pricingPlans"
          :key="index"
          cols="12"
          md="4"
        >
          <v-card
            flat
            class="mb-16 py-2 h-100 text-center"
          >
            <v-img
              :src="plan.image"
              width="250"
              class="mx-auto"
            />
            
            <h2 class="text-h6 font-weight-bold pt-11 text-military-green text-fjalla">
              {{ plan.title }}
            </h2>
            <p class="mt-2 text-center text-body-1 font-weight-bold text-fjalla text-grey-73">
              DE <span class="text-decoration-line-through	">{{ plan.oldPrice }}</span>
            </p>
            <div class="mt-4 text-h4 font-weight-bold mb-4 text-fjalla">
              <span class="text-body-2 mr-2">Por:</span>R$ {{ plan.price }}
            </div>

            <v-list
              class="text-left px-16 px-md-0"
            >
              <v-list-item
                v-for="(feature, i) in plan.features"
                :key="i"
              >
                <div class="d-flex">
                  <v-icon
                    color="green-military"
                    size="small"
                    class="mr-2"
                  >
                    mdi-check
                  </v-icon>
                  <p class="text-grey-51">
                    {{ feature }}
                  </p>
                </div>
              </v-list-item>
            </v-list>

            <v-btn
              color="yellow"
              size="large"
              class="mt-8 mx-auto d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
            >
              quero este plano
            </v-btn>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <!-- Questions Section -->
    <v-container
      fluid
      class="bg-grey py-16"
    >
      <v-row>
        <v-col
          cols="12"
          md="5"
          offset-md="1"
          class="d-flex text-center flex-column justify-center px-12"
        >
          <h2 class="text-h6 text-md-left font-weight-bold mb-2 opacity-50 text-fjalla">
            FICOU COM DÚVIDAS?
          </h2>
          <h2 class="text-h5 text-md-left text-md-h3 font-weight-bold mb-4 text-fjalla">
            FALE COM NOSSA EQUIPE!
          </h2>
          <p class="text-center text-md-left mb-8 text-body-2 font-weight-medium">
            Se ainda restou alguma dúvida sobre como ser um Atleta Fundador, estamos prontos para te responder. É só clicar no botão abaixo e falar direto com a equipe da Arena pelo WhatsApp.
          </p>
          <v-btn
            color="yellow"
            size="large"
            class="d-none d-md-flex mx-auto d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
          >
            <v-icon class="mr-2">
              mdi-whatsapp
            </v-icon>
            Entrar em contato
          </v-btn>
        </v-col>
        <v-col
          cols="12"
          md="4"
        >
          <v-img
            src="@/assets/equipe-1.png"
            width="300"
            cover
            class="mx-auto"
          />
        </v-col>
        <v-col
          cols="12"
          class="d-md-none"
        >
          <v-btn
            color="yellow"
            size="large"
            class="mx-auto d-block text-uppercase font-weight-bold text-cyan px-8 rounded-lg text-fjalla"
          >
            <v-icon class="mr-2">
              mdi-whatsapp
            </v-icon>
            Entrar em contato
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    <!-- FAQ Section -->
    <v-container class="py-16">
      <v-row>
        <v-col
          cols="12"
          md="8"
          offset-md="2"
          class="text-center mb-8"
        >
          <h2 class="text-h6 text-md-h4 font-weight-bold mb-4 text-center text-fjalla">
            AINDA COM DÚVIDAS? CONFERE AQUI!
          </h2>
          <p class="text-center mb-4 text-body-2 font-weight-medium text-grey-51">
            Sabemos que começar algo novo pode gerar algumas perguntas.
            Se você ainda não falou com a nossa equipe ou prefere ver as dúvidas mais comuns por aqui mesmo, se liga nas respostas abaixo:
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          cols="12"
          md="10"
          offset-md="1"
        >
          <v-expansion-panels flat>
            <v-expansion-panel
              v-for="(faq, index) in faqs"
              :key="index"
              large
              class="border-b-md"
            >
              <v-expansion-panel-title
                collapse-icon="mdi-minus"
                expand-icon="mdi-plus"
                class="py-6 text-body-2 text-military-green text-fjalla"
              >
                {{ faq.question }}
              </v-expansion-panel-title>
              <v-expansion-panel-text>
                <p class="text-grey-51 text-body-2">
                  {{ faq.answer }}
                </p>
              </v-expansion-panel-text>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-col>
      </v-row>
    </v-container>

    <!-- Footer -->
    <v-footer class="bg-black py-8">
      <v-container>
        <v-row>
          <v-col
            cols="12"
            md="2"
          >
            <v-img
              src="@/assets/logo.png"
              max-width="120"
              class="mb-4"
            />
          </v-col>
          <v-col
            cols="12"
            md="10"
            class="d-md-flex align-center ga-0 ga-md-4"
          >
            <div class="ml-auto d-flex align-center mb-2 mb-md-0">
              <v-icon
                size="small"
                class="mr-2"
              >
                mdi-phone
              </v-icon>
              <span class="text-body-2">(83) 4141-9850</span>
            </div>
            <div class="d-flex align-center mb-2 mb-md-0">
              <v-icon
                size="small"
                class="mr-2"
              >
                mdi-email
              </v-icon>
              <span class="text-body-2">contato@arenapicorelli.com.br</span>
            </div>
            <div class="d-flex align-center">
              <v-icon
                size="small"
                class="mr-2"
              >
                mdi-map-marker
              </v-icon>
              <span class="text-body-2">Av. Esperança, 535 - Manaíra. João Pessoa - PB</span>
            </div>
          </v-col>
          <hr
            width="100%"
            height="2"
            class="my-2"
          >
          <v-col
            cols="12"
            md="4"
          >
            <p class="text-body-2">
              Copyright ® 2025 Arena Picorelli
            </p>
          </v-col>
          <v-col
            cols="12"
            md="8"
          >
            <div class="d-flex align-center ga-3">
              <v-btn
                icon="mdi-facebook"
                class="ml-md-auto rounded-xl text-grey-51"
                density="comfortable"
                color="yellow"
              />
              <v-btn
                icon="mdi-instagram"
                class="rounded-xl text-grey-51"
                density="comfortable"
                color="yellow"
              />
              <v-btn
                icon="mdi-youtube"
                class="rounded-xl text-grey-51"
                density="comfortable"
                color="yellow"
              />
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script lang="ts" setup>
import Treino1 from "@/assets/treino-1.png"
import Treino2 from "@/assets/treino-2.png"
import Treino3 from "@/assets/treino-3.png"
import Treino4 from "@/assets/treino-4.png"
import Primeiro1 from "@/assets/primeiro-1.png"
import Primeiro2 from "@/assets/primeiro-2.png"
import Primeiro3 from "@/assets/primeiro-3.png"
import Primeiro4 from "@/assets/primeiro-4.png"
import Preco1 from "@/assets/preco-1.png"
import Preco2 from "@/assets/preco-2.png"
import Preco3 from "@/assets/preco-3.png"

  // Features list
  const features = [
    'Faça parte da história desde o início',
    'Tenha benefícios e vantagens exclusivas',
    'Seja reconhecido como um dos primeiros a acreditar',
    'Inspire outros a começarem também',
  ]

  // Training options
  const trainingOptions = [
    {
      title: 'PERFORMANCE E SUPERAÇÃO',
      description: 'Para quem busca força, corrida e alta performance.',
      image: Treino1,
    },
    {
      title: 'RESULTADOS REAIS',
      description: 'Para quem quer emagrecer com orientação de verdade.',
      image: Treino2,
    },
    {
      title: 'ACESSO ILIMITADO',
      description: 'Tenha acesso total à Arena, na hora que quiser.',
      image: Treino3,
    },
    {
      title: 'RECOMEÇO COM DISCIPLINA',
      description: 'Para quem quer voltar a treinar com prazer e constância.',
      image: Treino4,
    },
  ]

  // Benefits
  const benefits = [
    {
      title: 'ACESSO ILIMITADO À ARENA',
      description:
        'Os Atletas Fundadores terão acesso total e irrestrito à Arena Picorelli , sem limite de dias, horários ou turnos. Manhã, tarde ou noite, seu treino acontece no seu ritmo. A liberdade de treinar quando quiser, com a estrutura de quem entrega resultado.',
      image: Primeiro1,
    },
    {
      title: 'CONSULTA COM NUTRICIONISTA',
      description: 'Os Atletas Fundadores terão direito a uma consulta completa com a nutricionista da Arena, além de dois retornos personalizados para ajustes e acompanhamento dos resultados. Uma jornada de transformação começa com alimentação estratégica.',
      image: Primeiro2,
    },
    {
      title: 'AVALIAÇÃO NUTRICIONAL AVANÇADA',
      description:
        'Você terá acesso à balança de bioimpedância profissional com tecnologia de ponta, que oferece uma avaliação corporal precisa e segura. Porque resultados sérios começam com diagnóstico exato.',
      image: Primeiro3,
    },
    {
      title: 'AVALIAÇÃO COM DINAMOMETRIA',
      description: 'Fundadores terão acesso a avaliações funcionais com dinamometria, ferramenta usada para medir força muscular e prevenir lesões. Com ela, seu treino será ainda mais eficaz e seguro — com acompanhamento e revisão periódica.',
      image: Primeiro4,
    },
  ]

  // Pricing plans
  const pricingPlans = [
    {
      image: Preco1,
      title: 'PLANO MENSAL',
      oldPrice: 'R$ 250,00',
      price: '99,90',
      features: [
        'Acesso ilimitado',
        'Nutricionista + Retorno',
        'Recovery esportivo',
        'Avaliação com dinamometria',
        'Acesso prioritário a mentorias e eventos internos',
        'Camiseta exclusiva "Atleta Fundador"',
      ],
    },
    {
      image: Preco2,
      title: 'PLANO SEMESTRAL',
      oldPrice: 'R$ 250,00',
      price: '149,90',
      features: [
        'Acesso ilimitado',
        'Nutricionista + Retorno',
        'Recovery esportivo',
        'Avaliação com dinamometria',
        'Acesso prioritário a mentorias e eventos internos',
        'Camiseta exclusiva "Atleta Fundador"',
      ],
    },
    {
      image: Preco3,
      title: 'PLANO ANUAL',
      oldPrice: 'R$ 250,00',
      price: '199,90',
      features: [
        'Acesso ilimitado',
        'Nutricionista + Retorno',
        'Recovery esportivo',
        'Avaliação com dinamometria',
        'Acesso prioritário a mentorias e eventos internos',
        'Camiseta exclusiva "Atleta Fundador"',
      ],
    },
  ]

  // FAQs
  const faqs = [
    {
      question: 'PRECISO PAGAR TAXA DE MATRÍCULA?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.',
    },
    {
      question: 'O QUE ESTÁ INCLUSO NO PLANO?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
    {
      question: 'POSSO TREINAR EM QUALQUER HORÁRIO?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
    {
      question: 'QUAL A DIFERENÇA ENTRE OS PLANOS?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
    {
      question: 'O QUE ESTÁ INCLUSO NO PLANO?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
    {
      question: 'POSSO EXPERIMENTAR ANTES DE FECHAR O PLANO?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
    {
      question: 'E SE EU TIVER MAIS DÚVIDAS?',
      answer:
        'Não! Todos os nossos planos são sem taxa de matrícula. Você paga apenas o valor indicado.'
    },
  ]
</script>

<style scoped>
/* Custom styles */
.v-app {
  color: white;
}

.w-300 {
  max-width: 330px;
}

.text-fjalla {
  font-family: 'Fjalla One', sans-serif !important;
  &:deep() {
    span {
      font-family: 'Fjalla One', sans-serif !important;
    }
  }
}
</style>
