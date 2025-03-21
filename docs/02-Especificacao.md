# Especificação do projeto

<span style="color:red">Pré-requisitos: <a href="01-Contexto.md"> Documentação de contexto</a></span>

Definição do problema e ideia de solução a partir da perspectiva do usuário. É composta pela definição do  diagrama de personas, histórias de usuários, requisitos funcionais e não funcionais além das restrições do projeto.

Apresente uma visão geral do que será abordado nesta parte do documento, enumerando as técnicas e/ou ferramentas utilizadas para realizar a especificações do projeto.

## Personas

*1. Ana Clara, 32 anos*

Profissão: Analista de Marketing

Localização: Belo Horizonte - MG

Estado civil: Casada 

Perfil: Consumidora frequente de medicamentos para a família, preocupa-se com o meio ambiente, mas não sabe como descartar blisters corretamente

Motivação: Quer contribuir para a reciclagem e aproveitar descontos em produtos de higiene ou alimentícios 

Frustrações: 
- Falta de pontos de coleta próximos de casa 
- Desconhecimento sobre como blisters impactam o solo

---------------

*2. Carlos Mendes, 45 anos*

Profissão: Farmacêutico e dono de uma rede de farmácias 

Localização: Belo Horizonte - MG 

Estado civil: Casado 

Perfil: Busca diferenciar sua farmácia como sustentável e atrair novos clientes 

Motivação: Quer reduzir custos com descarte de resíduos e aumentar o fluxo de clientes 

Frustrações: 

- Dificuldade em gerenciar resíduos de blisters 

- Baixo engajamento em campanhas ambientais anteriores 

---------------

*3. João Ribeiro, 28 anos*

Profissão: Ciclista freelancer 

Localização: Betim - MG 

Estado civil: Solteiro 

Perfil: Usa a bicicleta como meio de transporte e busca renda extra 

Motivação: Quer trabalhar com entregas sustentáveis e evitar empregos tradicionais poluentes 

Frustrações: 

- Falta de oportunidades de trabalho flexíveis que aliem renda e propósito 

- Entregas via aplicativos tradicionais não valorizam sua pegada ecológica 

---------------

*4. Mariana Costa, 50 anos*

Profissão: Líder de uma cooperativa de reciclagem 

Localização: Contagem - MG 

Estado civil: Viúva 

Perfil: Lutadora por causas ambientais, busca parcerias para aumentar a reciclagem de materiais complexos 

Motivação: Quer ampliar a capacidade de processamento de blisters (alumínio e plástico) 

Frustrações: 

- Dificuldade em receber blisters separados corretamente 

- Falta de infraestrutura para reciclagem especializada 



## Histórias de usuários

As US abaixo foram elaboradas com base nas personas definidas e nos casos de uso do sistema:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Ana Clara (Consumidora)  | Registrar-me na plataforma com e-mail e CPF | Ter um cadastro no sistema e utiliza-lo |
|Ana Clara (Consumidora)  | Visualizar pontos de descarte | Entregar blisters no local correto |
|Ana Clara (Consumidora)  | Converter pontos de descarte em descontos | Ter um cadastro no sistema e utiliza-lo |
|Ana Clara (Consumidora)  | Acompanhar o histórico de descartes | Medir e acompanhar meu impacto ambiental |

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Carlos Mendes (Farmacêutico)   | Cadastrar minha farmácia como ponto de coleta | Atrair mais clientes e gerenciar resíduos |
|Carlos Mendes (Farmacêutico)   | Visualizar pontos de descarte | Entregar blisters no local correto |
|Carlos Mendes (Farmacêutico)   | Converter pontos de descarte em descontos | Ter um cadastro no sistema e utiliza-lo |

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|João Ribeiro (Ciclista)   | Registrar-me na plataforma com e-mail e CPF | Ter um cadastro no sistema e utiliza-lo |
|João Ribeiro (Ciclista)   | Visualizar pontos de descarte | Entregar blisters no local correto |
|João Ribeiro (Ciclista)   | Converter pontos de descarte em descontos | Ter um cadastro no sistema e utiliza-lo |

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Mariana Costa (Cooperativa)   | Registrar-me na plataforma com e-mail e CPF | Ter um cadastro no sistema e utiliza-lo |
|Mariana Costa (Cooperativa)   | Visualizar pontos de descarte | Entregar blisters no local correto |

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Todos os usuários | Registrar-me na plataforma com e-mail e CPF | Ter um cadastro no sistema e utiliza-lo |
|Todos os usuários | Visualizar pontos de descarte | Entregar blisters no local correto |

## Requisitos

*Requisitos Funcionais (RF) e Não Funcionais (RNF):* 

Os requisitos foram priorizados usando a técnica MoSCoW (Must have, Should have, Could have, Won't have), adaptada para alta, média e baixa prioridade. A priorização considera: 

- Alta (Must have): Funcionalidades essenciais para o MVP

- Média (Should have): Funcionalidades importantes, mas que podem ser desenvolvidas após o MVP

- Baixa (Could have): Melhorias ou features complementares

### Requisitos funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que usuários se cadastrem na plataforma com e-mail, CPF e endereço | ALTA | 
|RF-002| Exibir mapa interativo com geolocalização de farmácias parceiras | ALTA |
|RF-003| Sistema de pontuação por descarte de blisters (ex: 1 blister = 10 pontos) | ALTA |
|RF-004| Enviar notificações push sobre novos descontos e campanhas | BAIXA |
|RF-005| Permitir que farmácias cadastrem descontos em produtos que não sejam medicamentos | MÉDIA |
|RF-006| Sistema de confirmação de coleta via QR Code ou foto do material descartado | MÉDIA |
|RF-007| Permitir que ciclistas visualizem solicitações de coleta próximas | ALTA |

### Requisitos não funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve responder a requisições em menos de 4 segundos | ALTA | 
|RNF-002| Código otimizado para consumo mínimo de memória e energia | MÉDIA | 
|RNF-003| Integração com APIs de geolocalização (ex: Google Maps) | ALTA | 
|RNF-004| Gamificação com badges para usuários que mais reciclam | BAIXA | 
|RNF-005| Armazenamento de dados em bancos de dados otimizados para reduzir consumo de energia | BAIXA | 
|RNF-006| Suporte para português e inglês | BAIXA | 


## Restrições

O projeto está restrito aos itens apresentados na tabela a seguir:

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|001| O projeto deverá ser entregue até o final do semestre |
|002| O projeto não envolve gastos financeiros |
|003| Dependência de parceria com farmácia para validar ponto de coleta |
|004| Utilização obrigatória de tecnologias gratuitas |
|005| Conformidade com a LGPD |

## Diagrama de casos de uso

<img src="https://github.com/ICEI-PUC-Minas-PBE-ADS-SI/2025-1-p5-tias-projeto-eco-farma/blob/main/docs/images/Diagrma%20caso%20de%20uso%20TI.jpeg?raw=true" alt="Diagrama de caso de uso">

