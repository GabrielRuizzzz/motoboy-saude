# Requisitos e histórias de usuário — Motoboy Saúde

Escopo definido a partir da pesquisa com 19 motoboys (ver [pesquisa-usuarios.md](pesquisa-usuarios.md)).

## 1. Escopo do MVP

| Dentro do MVP | Fica para a fase 2 |
|---|---|
| Lembretes de pausa e água | Registro de acidentes e sintomas |
| Botão de emergência com localização | Painel semanal de saúde |
| Mapa de UBS/UPA/hospitais e pontos de apoio | Parcerias com benefícios (descontos) |
| Dicas de saúde e alimentação | Notificações com o app fechado |
| Login simples | Versão para lojas (Android/iOS) |

## 2. Requisitos funcionais

| ID | Requisito | Prioridade | Base na pesquisa |
|---|---|---|---|
| RF01 | O app deve enviar lembretes de pausa e de beber água em intervalos configuráveis | Alta | 42,1% pediram |
| RF02 | O app deve ter um botão de emergência que abre a ligação para o SAMU (192) e envia a localização por WhatsApp | Alta | 42,1% pediram |
| RF03 | O app deve mostrar em um mapa as UBS, UPAs e hospitais mais próximos | Alta | 36,8% pediram |
| RF04 | O app deve mostrar pontos de apoio e descanso (banheiro, água, abrigo) no mapa | Média | Pedido espontâneo em 3 respostas abertas |
| RF05 | O app deve exibir dicas curtas de saúde e alimentação | Média | 52,6% pediram (a mais votada) |
| RF06 | O usuário deve poder criar uma conta e entrar com e-mail ou telefone | Média | Necessário para configurações |
| RF07 | O usuário deve poder registrar acidentes e sintomas (fase 2) | Baixa | 36,8% pediram |

## 3. Requisitos não funcionais

| ID | Requisito |
|---|---|
| RNF01 | O app deve funcionar no navegador do celular e poder ser instalado na tela inicial (PWA) |
| RNF02 | A interface deve ter botões grandes e textos claros, para uso rápido com uma mão |
| RNF03 | O app deve ser leve e funcionar com internet fraca |
| RNF04 | Os dados pessoais e de localização devem seguir a LGPD, com pedido de consentimento |
| RNF05 | Os dados de estabelecimentos de saúde devem vir de fontes públicas (CNES/DATASUS) |
| RNF06 | O app deve ser gratuito para o motoboy |

## 4. Histórias de usuário

| ID | História | Critérios de aceite |
|---|---|---|
| HU01 | Como motoboy, quero receber lembretes de pausa e água para não trabalhar horas seguidas sem descanso | Posso escolher o intervalo (ex.: a cada 1h ou 2h); o lembrete aparece com som e texto; posso adiar ou confirmar |
| HU02 | Como motoboy, quero um botão de emergência para pedir ajuda rápido depois de um acidente | O botão fica visível na tela inicial; ao tocar, abre a ligação para o 192; permite enviar minha localização por WhatsApp para um contato |
| HU03 | Como motoboy, quero ver o posto de saúde mais próximo para me atender quando passar mal | O mapa mostra minha posição; lista UBS, UPAs e hospitais por distância; toco em um e abro a rota |
| HU04 | Como motoboy, quero achar pontos de apoio e descanso para beber água e descansar entre as entregas | O mapa tem uma camada de pontos de apoio; cada ponto mostra o que oferece (banheiro, água, abrigo) |
| HU05 | Como motoboy, quero dicas curtas de saúde e alimentação para cuidar de mim sem perder tempo | Cada dica tem até 3 linhas; recebo uma dica por dia; posso ler dicas anteriores |
| HU06 | Como motoboy, quero criar uma conta para guardar minhas configurações | Entro com e-mail ou telefone; minhas configurações voltam quando eu entro de novo |

## 5. Observação técnica

Por ser um PWA, os lembretes (RF01) funcionam de forma confiável com o app aberto. Notificações com o app fechado ficam para a fase 2, com app nativo.

O botão de emergência (RF02) é um apoio e não substitui o atendimento do SAMU. O app deve deixar isso claro ao usuário.
