# 🚀 EdgeBets - Deploy Vercel

## ⚡ SOLUÇÃO DO ERRO 404

O erro acontece porque o Vercel precisa da estrutura correta. Use estas instruções:

---

## 📦 Opção 1: Via ZIP (MAIS FÁCIL)

1. **Descompacte** o arquivo `edgebets-vercel.zip`
2. **Acesse** [vercel.com/new](https://vercel.com/new)
3. **Arraste** a pasta `edgebets-vercel`
4. **Deploy!** ✅

---

## 💻 Opção 2: Via CLI

```bash
# 1. Descompactar
unzip edgebets-vercel.zip
cd edgebets-vercel

# 2. Deploy
vercel --prod

# 3. Pronto! ✅
```

---

## 📁 Estrutura Correta

```
edgebets-vercel/
├── index.html          # Versão na raiz
├── public/
│   └── index.html      # Versão na pasta public (Vercel usa esta)
├── vercel.json         # Configuração do Vercel
├── package.json        # Metadados
└── .vercelignore       # Arquivos ignorados
```

---

## 🔧 Se Ainda Assim Der Erro 404:

### No Dashboard do Vercel:

1. Vá em **Settings**
2. **General** → **Root Directory**
3. Deixe em branco ou coloque `public`
4. **Save**
5. **Redeploy**

---

## 🎯 Após Deploy Funcionar:

### Migrar Dados:

1. **Na versão antiga**: Clique em **💾 Backup**
2. Salve o arquivo `.json`
3. **Na versão nova (Vercel)**: Clique em **📂 Restaurar**
4. Selecione o arquivo `.json`
5. ✅ Pronto!

---

## 🆘 Troubleshooting

### Erro: "Build Failed"
→ Ignore, não precisa de build. Use pasta `public/`

### Erro: "404 NOT_FOUND"
→ Certifique-se que `index.html` está em `public/`

### Tela branca
→ Abra Console do navegador (F12) e veja erros

### localStorage vazio
→ Normal! Use Backup/Restore para migrar dados

---

## ✅ Checklist

- [ ] Descompactei o ZIP
- [ ] Arrastei pasta no Vercel
- [ ] Deploy concluído com sucesso
- [ ] Acessei a URL
- [ ] Fiz backup dos dados antigos
- [ ] Importei dados via Restaurar
- [ ] Tudo funcionando! 🎉

---

**URL de exemplo**: `https://edgebets.vercel.app`

**Dúvidas?** Confira [docs.vercel.com](https://vercel.com/docs)
