# Guia do Bolsa Família - Consulta e Recuperação

Web app mobile-first para consulta de situação do Bolsa Família com foco em recuperação de valores atrasados.

## 🚀 Deploy no Vercel via GitHub

### Passo 1: Criar Repositório no GitHub
1. Acesse [github.com](https://github.com) e faça login
2. Clique em "New repository"
3. Nome: `bolsa-familia-guia` (ou outro nome)
4. Deixe como público ou privado
5. NÃO adicione README, .gitignore ou license
6. Clique em "Create repository"

### Passo 2: Fazer Push do Código

Abra o terminal nesta pasta e execute:

```bash
git init
git add .
git commit -m "Initial commit - Guia do Bolsa Familia"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/bolsa-familia-guia.git
git push -u origin main
```

**Nota:** Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub.

### Passo 3: Deploy no Vercel

1. Acesse [vercel.com](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "Add New Project"
4. Selecione seu repositório `bolsa-familia-guia`
5. Clique em "Import"
6. Mantenha as configurações padrão
7. Clique em "Deploy"

🎉 Pronto! Seu site estará no ar em segundos!

## 📱 Características

- ✅ Mobile-first design
- ✅ 3 espaços para AdSense (Topo, Meio, Rodapé)
- ✅ Quiz de 2 etapas
- ✅ Tela de processamento com spinner (3 segundos)
- ✅ Resultados personalizados
- ✅ Cores Brasil (Verde/Amarelo/Branco)
- ✅ 100% em Português do Brasil

## 📈 Configurar Google Analytics

O site já está preparado para Google Analytics! Siga estes passos:

### Passo 1: Criar Conta no Google Analytics
1. Acesse [analytics.google.com](https://analytics.google.com)
2. Faça login com sua conta Google
3. Clique em "Começar a medir"
4. Crie uma conta (nome: ex: "Meus Sites")
5. Crie uma propriedade (nome: ex: "Bolsa Familia Guia")
6. Configure informações básicas (moeda, fuso horário)
7. Aceite os termos

### Passo 2: Obter o ID de Medição
1. Após criar a propriedade, você verá um **ID de Medição** (formato: `G-XXXXXXXXXX`)
2. Copie esse ID

### Passo 3: Adicionar o ID no Código
1. Abra o arquivo `index.html`
2. Procure por `G-XXXXXXXXXX` (aparece 2 vezes)
3. Substitua `G-XXXXXXXXXX` pelo seu ID real
4. Salve o arquivo

**Exemplo:**
```html
<!-- Antes -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
gtag('config', 'G-XXXXXXXXXX');

<!-- Depois (com seu ID real) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-ABC123XYZ"></script>
gtag('config', 'G-ABC123XYZ');
```

### O que será rastreado:
- ✅ Número de visitantes
- ✅ Páginas visualizadas
- ✅ Taxa de conclusão do quiz
- ✅ Cliques em botões
- ✅ Tipo de resultado do quiz
- ✅ Tempo no site
- ✅ Dispositivos utilizados (mobile/desktop)

Após adicionar o ID, faça commit e push. Os dados começarão a aparecer em 24-48 horas no Google Analytics.

## 🎯 Configurar AdSense

Após o deploy, substitua os placeholders de anúncios:

```html
<!-- Substitua isto: -->
<div id="ad-top" class="ad-banner">
    [ESPAÇO PARA ANÚNCIO ADSENSE - TOPO]
</div>

<!-- Por isto (código do AdSense): -->
<div id="ad-top">
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
    <!-- Seu código de anúncio aqui -->
</div>
```

Repita para `#ad-middle` e `#ad-bottom`.

## 📊 Estrutura

- **Home:** Headline chamativa + botão de início
- **Passo 1:** Pergunta sobre mensagem do app Caixa Tem
- **Passo 2:** Pergunta sobre situação de moradia
- **Processamento:** Spinner + anúncio grande
- **Resultado:** Informações personalizadas + mensagem verde de boa notícia + botão calendário

## 🔧 Tecnologias

- HTML5
- CSS3 (Flexbox, Grid, Animations)
- JavaScript Vanilla
- Design Responsivo

## 📝 Licença

Projeto livre para uso comercial.