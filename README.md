# 🌺 Flores do Cariri — PWA

App web para reconhecimento de flores do Cariri cearense e da Caatinga.
Funciona **offline** após o primeiro acesso.

## Estrutura de arquivos

```
flores_pwa/
├── index.html          → site principal
├── manifest.json       → configuração do PWA
├── sw.js               → service worker (offline)
├── labels.txt          → nomes das flores
└── modelo/
    ├── model.json      → modelo TF.js
    ├── group1-shard1of3.bin
    ├── group1-shard2of3.bin
    └── group1-shard3of3.bin
```

## Como publicar no GitHub Pages (gratuito)

### 1. Criar conta no GitHub
Acesse github.com e crie uma conta gratuita.

### 2. Criar repositório
1. Clique em "New repository"
2. Nome: `flores-cariri`
3. Marque "Public"
4. Clique em "Create repository"

### 3. Fazer upload dos arquivos
1. Clique em "uploading an existing file"
2. Arraste TODOS os arquivos desta pasta
3. Atenção: a pasta `modelo/` precisa ser criada manualmente:
   - Clique em "create new file"
   - Digite: `modelo/model.json`
   - Cole o conteúdo do model.json
   - Repita para os arquivos .bin
4. Clique em "Commit changes"

### 4. Ativar GitHub Pages
1. Vá em Settings → Pages
2. Em "Source", selecione "Deploy from a branch"
3. Branch: main / (root)
4. Clique em Save

### 5. Acessar o site
Após alguns minutos, o site estará em:
`https://SEU_USUARIO.github.io/flores-cariri`

## Como usar no celular offline

1. Acesse o site pelo celular
2. Aguarde carregar completamente
3. No Chrome (Android): toque nos 3 pontos → "Adicionar à tela inicial"
4. No Safari (iPhone): toque em compartilhar → "Adicionar à Tela de Início"
5. A partir daí funciona offline!

## Flores reconhecidas (26)

### Cariri / Caatinga
- Mandacaru, Xique-xique, Facheiro, Coroa-de-frade, Palma
- Catingueira, Mororó, Jurema Preta, Mulungu, Pacotê, Juçá, Cumaru
- Chanana, Muçambê, Maracujá do Mato, Alamanda
- Macambira, Caroá

### Brasil geral
- Ipê Amarelo, Bromélia, Antúrio, Primavera
- Hibisco, Helicônia, Orquídea Cattleya, Vitória-régia
