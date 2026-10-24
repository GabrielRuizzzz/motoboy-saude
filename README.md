<p align="center">
  <img src="docs/identidade-visual/logo.svg" alt="Logo Motoboy Saúde" width="320">
</p>

# 🏍️ Motoboy Saúde

> Aplicativo de saúde e segurança para motoboys e entregadores de moto.

**Projeto integrador FMU Tech Inovação · ODS 3 — Saúde e Bem-Estar**
**Equipe:** Gabriel Ruiz de Farias, Gustavo Florencio dos Anjos, David Kenzo Iamaguti
**Professor Mentor:** Robson Carmo
**Status:** 🟡 Checkpoint 1 — Ideação

---

## 1. Problema

### Declaração do problema

Motoboys passam o dia exposto ao trânsito, em jornadas longas e sob pressão por velocidade, e quase não têm acompanhamento de saúde nem apoio rápido em caso de acidente. O resultado é um grupo com alto risco de lesões graves, mortes evitáveis e adoecimento (fadiga, dor, estresse), que sobrecarrega o SUS e deixa famílias sem renda.

### Dados e impacto (fontes públicas)

| Dado | Fonte |
|---|---|
| Mortes de motociclistas subiram de 12 mil (2022) para 13,5 mil (2023), alta de 12,5%; foram 28,4 mil feridos em 2023 | Atlas da Violência 2025 (Ipea/FBSP), com dados do SIM e Sinan, Ministério da Saúde |
| A taxa de internação de motociclistas por lesões no trânsito cresceu 55% entre 2011 e 2021 | Boletim Epidemiológico, Ministério da Saúde (2023) |
| Em 2024, cerca de 165 mil motociclistas deram entrada na rede pública, com custo de quase R$ 258 milhões ao SUS | DATASUS |
| Entre 2015 e 2025, o SUS registrou 1.247.801 internações e 22.984 mortes hospitalares de motociclistas; 81,7% das vítimas são homens, com média de 33,9 anos | DRG Brasil / DATASUS |
| Perfil dos mortos: 88,1% homens, majoritariamente jovens de 20 a 29 anos | Boletim Epidemiológico, Ministério da Saúde |
| O estado de SP registrou número recorde de mortes de motociclistas no 1º semestre de 2025 | Governo do Estado de SP |

> ⚠️ **Limitação:** as estatísticas oficiais tratam de *motociclistas* em geral. Dados específicos de *entregadores* são escassos; por isso o projeto inclui uma pesquisa própria com motoboys (ver seção 3).

### Relação com o ODS 3

- **Meta 3.6:** reduzir pela metade as mortes e lesões no trânsito
- **Meta 3.8:** acesso a serviços essenciais de saúde
- **Meta 3.4:** reduzir doenças não transmissíveis e promover saúde mental

---

## 2. Solução proposta (ideia inicial)

O **Motoboy Saúde** é um app que acompanha a saúde e a segurança do motoboy durante o trabalho.

**Funcionalidades candidatas ao MVP** *(serão validadas com usuários)*:

- ⏱️ Lembretes de pausa, hidratação e descanso
- 🆘 Botão de emergência com localização para contatos e SAMU
- 🏥 Mapa de UBS, UPAs e hospitais próximos
- 📋 Registro de acidentes e sintomas (dor, cansaço, estresse)
- 📊 Painel simples de saúde semanal

---

## 3. Validação com usuários

- [ ] Questionário com 5 a 10 motoboys
- [ ] Resultados e conclusões (a preencher)

---

## 4. Tecnologias

| Camada | Tecnologia |
|---|---|
| Aplicativo | PWA (app web instalável no celular) com React + Vite |
| Estilo | Tailwind CSS |
| Backend e banco de dados | Firebase (Authentication + Firestore) |
| Mapas | Leaflet + OpenStreetMap (gratuito, sem chave de API) |
| Localização e emergência | Geolocalização do navegador + link `tel:192` (SAMU) + compartilhamento da localização por WhatsApp |
| Hospedagem | GitHub Pages ou Vercel |
| Dados públicos | DATASUS, Infosiga SP, CNES (estabelecimentos de saúde) |
| Design | Figma |
| Versionamento | Git + GitHub |

---

## 5. Identidade visual

- **Nome:** Motoboy Saúde
- **Slogan:** *Rode com saúde. Volte pra casa.*
- **Conceito:** um escudo (proteção) com um batimento cardíaco (saúde); o ponto laranja representa movimento e alerta.
- **Logo:** `docs/identidade-visual/logo.svg`

| Cor | Hex | Uso |
|---|---|---|
| Verde Saúde | `#00A86B` | Cor principal, botões e destaques |
| Laranja Alerta | `#FF7A00` | Ações importantes e emergência |
| Grafite | `#1F2933` | Textos e títulos |
| Cinza Claro | `#F5F7FA` | Fundos |
| Vermelho SOS | `#D7263D` | Botão de emergência |

**Tipografia:** Poppins (títulos) e Inter (textos), ambas gratuitas no Google Fonts.

---

## 6. Pitch inicial

[Link do vídeo ou slides em `/docs/pitch`]

---

## 7. Cronograma

| Entrega | Período | Status |
|---|---|---|
| Checkpoint 1 — Ideação | 19/10 a 30/10 | 🟡 Em andamento |
| Checkpoint 2 — Protótipo + vídeo de demonstração | 09/11 a 27/11 | ⚪ Pendente |
| Apresentação final (pitch de 5 min) | 07/12 e 08/12 | ⚪ Pendente |

---

## 8. Estrutura do repositório

```
motoboy-saude/
├── README.md
├── docs/
│   ├── problema.md
│   ├── requisitos.md
│   ├── identidade-visual/
│   └── pitch/
├── src/
└── LICENSE
```

## 9. Equipe

| Nome | Função |
|---|---|
| Gabriel Ruiz de Farias | Montar e Planejar |
| David Kenzo Iamaguti | Montar e Idealizar |
| Gustavo Florencio dos Anjos | Montar e apresentar |
