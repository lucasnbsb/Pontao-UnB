# Introdução

O Pontão UnB é um cliente para o registro de ponto eletrônico na Universidade de Brasília, isso significa que o aplicativo utiliza exatamente a mesma infraestrutura e metodologia do registro de ponto existente, sendo porntanto condicionado às mesmas regras.

O funcionamento é simples, o usuário registra suas credenciais do sigrh e o sistema realiza Toda a navegação e o registro do ponto com um clique. Registrando a cada passo as respostas do sistema de ponto.

# Passo a passo:

## Cadastrar as Credenciais:

Ao abrir o aplicativo pela primeira vez, o usuário encontrará apenas uma menságem avisando sobre a necessidade de registrar as credenciais de acesso. Na tela de configurações o usuário deve digitar seu login e senha do Sigrh. Não se preocupe, seus dados serão guardados apenas no seu celular, e transmitidos ao Sigrh por uma conexão segura. Para limpar os dados, basta limpar os dados do aplicativo.

<div style="text-align:center">
 <img src="https://raw.githubusercontent.com/lucasnbsb/Pontao-UnB/master/imagens/flutter_01.png" height="533" width="300">
 <img src="https://raw.githubusercontent.com/lucasnbsb/Pontao-UnB/master/imagens/flutter_02.png" height="533" width="300">
</div>

## Bater o Ponto:
Após o registro dos dados o usuário está pronto para realizar o registro de ponto, clique bater ponto e confirme a operação, o aplicativo realiza todo o processo sozinho:

<img src="https://raw.githubusercontent.com/lucasnbsb/Pontao-UnB/master/imagens/entrada.gif" height="533" width="300">


## Seleção de Unidade.
Alguns funcionários precisam selecionar a unidade na qual o ponto será registrado antes de bater o ponto, para tanto é necessário o código da únidade. Logue uma vez sem preencher o código e o aplicativo listará as unidades e seus códigos, aí basta copiar o código para as configurações e daqui pra frente seu ponto será registrado sempre na mesma unidade.

# Almoço
O ponto de saída para o almoço segue as seguintes regras: 
1. A saída para o almoço só pode ser registrada das 11 às 15
2. A volta do almoço só pode ser registrada 1 hora após a saída.

O aplicativo trata a saída do almoço da seguinte forma:

1. A saída para almoço só pode ser registrada se o regime selecionado for 8 horas.
2. A saída para almoço só é registrada se o checkbox "Saída para o almoço se possível?" estiver marcado
3. A hora do celular deve estar entre 11 e 15

O sistema avisa quando uma saída é registrada como almoço e randomiza um emoji de comida pra servir como sugestão :)

Nas configurações é possível agendar um aviso após a saída para almoço, por padrão este aviso está configurado para 1 hora. Clique no botão "Notificar o retorno do almoço após X" para configurar o tempo desta notificação. Note que o seletor apresenta o formato am/pm, e para selecionar 59 minutos por exemplo o usuário deve selecionar 12:59AM no relógio.

# Regimes
O sistema apresenta uma configuração de regimes, 4, 6 ou 8 horas. Essa opção não afeta o comportamento do ponto exceto pelo almoço, como descrito acima e o cálculo da hora mínima de saída, que leva em conta os 15 minutos de tolerância diários, ou seja, no importando o seu regime você pode bater o ponto com qualquer uma das configurações.

# Perguntas mais frequêntes
1. Tem para IOs?
Tem e não tem, o aplicativo foi feito em Flutter, um framework da google que gera aplicativos nativos para as duas plataformas, mas infelizmente não é possível distribuir o aplicativo sem ser pela loja oficial da Apple ou pelo programa de beta test, e para isso é preciso uma conta de desenvolvedor que custa 99 USD por mês, e a aprovação na revisão manual

2. 
