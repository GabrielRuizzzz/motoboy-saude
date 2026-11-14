# LGPD no Motoboy Saúde

> Documento de análise do grupo (não é parecer jurídico). Base: Lei Geral de Proteção de Dados (Lei 13.709/2018). Recomenda-se validar com o Professor Mentor.

## 1. Ideia levantada pelo professor

Ao cadastrar a **placa da moto** no app, o botão de emergência já avisaria um familiar e chamaria o SAMU. O professor pediu para verificar a LGPD.

## 2. Que dados o app trata

| Dado | Classificação na LGPD | Observação |
|---|---|---|
| Nome, e-mail ou telefone | Dado pessoal | Necessário para o login |
| Placa da moto | Dado pessoal quando ligada à pessoa no cadastro | Só guardar se o usuário optar |
| Localização | Dado pessoal | Pode revelar rotina e endereço; usar só quando necessário |
| Contato de emergência (familiar) | Dado pessoal de **terceiro** | O usuário informa o contato; avisar o usuário dessa responsabilidade |
| Informações de saúde (sintomas, acidentes, fase 2) | Dado pessoal **sensível** (art. 5, II) | Exige cuidado reforçado |

## 3. Pontos de atenção

1. **Consentimento claro e separado.** Tela de aceite explicando o que é coletado e para quê (finalidade), com opção de recusar a placa e a localização.
2. **Minimização.** Coletar só o necessário: a placa é opcional; a localização só é lida quando o botão é acionado.
3. **Base legal na emergência.** A LGPD prevê o tratamento de dados para a proteção da vida ou da integridade física do titular (arts. 7º, VII, e 11, II, "e"). Mesmo assim, o app deve informar o usuário desde o cadastro.
4. **Transparência e direitos do titular.** Política de privacidade em linguagem simples, e opção de ver, corrigir e apagar os dados (art. 18) dentro do app.
5. **Segurança.** Login com autenticação (Firebase Authentication), regras de acesso no banco e nenhum dado pessoal de saúde em repositório público.
6. **Compartilhamento.** Os dados só vão ao familiar escolhido pelo usuário e ao serviço de emergência acionado; nunca a empresas parceiras ou plataformas de entrega sem consentimento específico.

## 4. O que é possível no protótipo

Hoje **não existe API pública** para o app acionar o SAMU automaticamente com a placa. Por isso, o protótipo faz o seguinte ao tocar no botão:

1. Abre a ligação para o **192** (o usuário confirma a chamada).
2. Abre uma mensagem de WhatsApp para o contato de emergência com a **localização** e, se o usuário tiver cadastrado, a **placa**.

Uma integração automática com o SAMU, órgãos de trânsito ou seguradoras fica como **evolução futura**, e exigiria convênio e uma avaliação de impacto à proteção de dados (RIPD).

## 5. Itens para implementar no app

- [ ] Tela de consentimento no primeiro acesso
- [ ] Placa e contato de emergência opcionais
- [ ] Página "Privacidade" com a política em linguagem simples
- [ ] Botão "Apagar meus dados" nas configurações
