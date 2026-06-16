# Central de Ponto ⏱

Dashboard de gestão de ponto e ocorrências — arquivo HTML único, sem dependências locais.

---

## 🚀 Publicar no GitHub Pages (passo a passo)

### 1. Crie um repositório no GitHub

- Acesse [github.com](https://github.com) → clique em **New repository**
- Dê um nome (ex: `central-de-ponto`)
- Deixe como **Public**
- Clique em **Create repository**

### 2. Suba o arquivo

Na tela do repositório recém-criado, clique em **uploading an existing file** e envie o `index.html`.

Ou via terminal:
```bash
git init
git add index.html
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/central-de-ponto.git
git push -u origin main
```

### 3. Ative o GitHub Pages

- No repositório → **Settings** → **Pages** (menu lateral)
- Em **Source**, selecione: `Deploy from a branch`
- Branch: `main` · Pasta: `/ (root)`
- Clique em **Save**

### 4. Acesse seu link

Após ~1 minuto, seu app estará em:

```
https://SEU_USUARIO.github.io/central-de-ponto/
```

---

## 🔐 Credenciais de acesso

| Perfil | ID de usuário | Senha |
|---|---|---|
| Administrador | `admin` | `admin123` |
| Colaborador N | `func_N` (2 a 26) | matrícula em minúsculo |

Exemplos de colaborador: `func_2` / `ic-001` · `func_7` / `pc-001`

---

## 📋 Funcionalidades

- **Dashboard admin** — KPIs, monitor de esquecimentos, pendências recentes
- **Funcionários** — lista completa com filtros, adicionar e excluir
- **Perfil individual** — histórico de ocorrências, criar pendências
- **Painel de verificação** — aprovar ou rejeitar correções dos colaboradores
- **Relatórios** — por tipo, por status, top funcionários, exportação XLSX
- **Mural de recados** — recados fixados, reações com emojis
- **Portal do colaborador** — ver pendências, marcar como corrigido, enviar print EasyMob
- **Sincronização entre abas** — via `localStorage` com polling em tempo real
- **Notificações toast** — alertas em tempo real para admin e colaboradores
