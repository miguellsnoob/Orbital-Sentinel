# Orbital Sentinel

### Global Solution 2026.1 — Cross-Platform Application Development | FIAP

![Banner do Projeto](./assets/screenshots/banner.png)

## Sobre o projeto

O **Orbital Sentinel** é um aplicativo mobile desenvolvido para a Global Solution 2026.1, com o tema de monitoramento de sistemas espaciais.

A ideia do projeto é simular uma plataforma de análise preditiva para acompanhar uma missão orbital. Pelo aplicativo, é possível visualizar dados de sensores, energia, comunicação e alertas da missão, usando informações simuladas.

Durante o desenvolvimento, procurei criar uma interface com visual mais tecnológico e espacial, além de organizar os dados de uma forma simples para facilitar a leitura dos indicadores principais da missão.

## Equipe

| Nome                 | RM     |
| -------------------- | ------ |
| Miguel Lima da Silva | 565141 |

Modalidade: Individual

## Telas do aplicativo

### Home — Dashboard principal

![Home](./assets/screenshots/home.png)

Tela inicial do aplicativo, mostrando um resumo geral da missão. Nela aparecem os principais indicadores, como energia, temperatura, sinal de comunicação e estabilidade orbital.

### Dashboard de sensores

![Sensores](./assets/screenshots/sensores.png)

Tela com dados simulados dos sensores da missão. O objetivo é acompanhar informações importantes para o funcionamento dos sistemas espaciais, como temperatura e outros indicadores técnicos.

### Dashboard de energia

![Energia](./assets/screenshots/energia.png)

Dashboard voltado para o acompanhamento da parte energética da missão, exibindo informações como nível de energia, consumo e situação geral do sistema.

### Dashboard de comunicação

![Comunicação](./assets/screenshots/comunicacao.png)

Tela responsável por mostrar a situação da comunicação da missão, incluindo qualidade do sinal, latência e estabilidade da telemetria.

### Alertas

![Alertas](./assets/screenshots/alertas.png)

Tela que lista os alertas gerados automaticamente pelo aplicativo. Esses alertas aparecem quando algum dado simulado passa dos limites configurados, como energia baixa ou temperatura elevada.

### Configurações

![Configurações](./assets/screenshots/configuracoes.png)

Tela com formulário para configurar os limites críticos da missão. O usuário consegue alterar os valores de referência para geração dos alertas, com validação dos campos antes de salvar.

## Funcionalidades desenvolvidas

* Navegação entre telas usando Expo Router
* Dashboard principal com resumo da missão
* Dashboard de sensores
* Dashboard de energia
* Dashboard de comunicação
* Sistema de alertas baseado em limites críticos
* Formulário para configuração dos limites da missão
* Validação dos campos do formulário
* Uso de Context API para compartilhar dados entre telas
* Uso de AsyncStorage para salvar as configurações localmente
* Dados simulados para representar uma operação orbital
* Interface com identidade visual inspirada no tema espacial
* Componentes reutilizáveis para organizar melhor o código

## Tecnologias utilizadas

* React Native
* Expo
* Expo Router
* TypeScript
* Context API
* AsyncStorage
* React Hooks
* Expo Go

## Estrutura do projeto

```txt
orbital-sentinel-miguel/
│
├── app/
│   ├── _layout.tsx
│   ├── index.tsx
│   ├── sensores.tsx
│   ├── energia.tsx
│   ├── comunicacao.tsx
│   ├── alertas.tsx
│   └── configuracoes.tsx
│
├── assets/
│   └── screenshots/
│       ├── banner.png
│       ├── home.png
│       ├── sensores.png
│       ├── energia.png
│       ├── comunicacao.png
│       ├── alertas.png
│       └── configuracoes.png
│
├── components/
│   ├── CardIndicador.tsx
│   ├── MissionAlert.tsx
│   ├── SectionTitle.tsx
│   └── StatusBadge.tsx
│
├── context/
│   └── MissionContext.tsx
│
├── types/
│   └── mission.ts
│
├── utils/
│   └── missionData.ts
│
├── README.md
├── entrega_fiap.txt
├── package.json
├── app.json
├── tsconfig.json
├── babel.config.js
└── .gitignore
```

## Como executar o projeto

### Pré-requisitos

Antes de rodar o projeto, é necessário ter instalado:

* Node.js
* npm
* Expo Go no celular

### Passo a passo

Clone o repositório:

```bash
git clone https://github.com/miguellsnoob/Orbital-Sentinel.git
```

Entre na pasta do projeto:

```bash
cd orbital-sentinel-miguel
```

Instale as dependências:

```bash
npm install
```

Inicie o projeto com Expo:

```bash
npx expo start
```

Depois disso, basta escanear o QR Code com o aplicativo Expo Go no celular.

Caso tenha problema de conexão, também é possível iniciar usando:

```bash
npx expo start --tunnel
```

## Como o app funciona

O aplicativo trabalha com dados simulados de uma missão espacial. Esses dados são exibidos nos dashboards e também são usados para gerar alertas quando algum indicador fica fora do limite esperado.

Na tela de configurações, o usuário pode alterar os limites críticos da missão. Esses valores são salvos localmente com AsyncStorage, então continuam disponíveis mesmo depois de fechar e abrir o aplicativo novamente.

A Context API foi usada para centralizar os dados principais da missão e permitir que diferentes telas acessem as mesmas informações.

## Vídeo de demonstração

O vídeo abaixo apresenta o funcionamento geral do aplicativo, mostrando as telas principais, os dashboards, a tela de alertas e o formulário de configurações.

[Clique aqui para assistir ao vídeo de demonstração](COLE_AQUI_O_LINK_DO_VIDEO)

## Observações finais

Este projeto foi desenvolvido para fins acadêmicos, como parte da Global Solution 2026.1 da FIAP, na disciplina de Cross-Platform Application Development.

A proposta foi criar uma solução mobile simples, funcional e organizada, aplicando os conteúdos trabalhados durante o semestre em um contexto ligado à indústria espacial moderna.

## Autor

Miguel Lima da Silva
RM: 565141
FIAP — Ciência da Computação — 2º Ano
