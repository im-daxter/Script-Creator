# 🛠️ script_creator

**A shell script generator for quick and standardized Bash script scaffolding.**

*Part of the debxp Introductory Shell Script Course*

![Shell Script](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![License](https://img.shields.io/badge/License-GPL%20v3-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen?style=flat-square)

---

## 🌐 Language / Idioma
* 🇺🇸 [English Version](#-english-version)
* 🇧🇷 [Versão em Português](#-versão-em-português)

---

## 🇺🇸 English Version

### About

`script_creator` is a simple yet practical Bash utility that automates the creation of new shell scripts with a standardized header. Developed as part of the **debxp Introductory Shell Script Course**, it ensures every new script starts with a consistent structure — including metadata such as description, version, author, date, and license — and immediately opens the file in your preferred editor.

### Features

- ✅ Generates a new `.sh` file with a pre-filled header template
- ✅ Automatically injects the current date into the header
- ✅ Sets the new file as executable (`chmod +x`) on creation
- ✅ Opens the file directly in your configured editor (default: `vim`)
- ✅ Guards against missing arguments and accidental file overwrites

### Requirements

- Bash (or any POSIX-compatible shell environment)
- `vim` (or replace the `editor` variable with your preferred editor)

### Installation

Clone this repository and give the script execution permission:

```bash
git clone https://github.com/im-daxter/script_creator.git
cd script_creator
chmod +x script_creator
```

Optionally, place it in a directory on your `$PATH` to use it globally:

```bash
sudo cp script_creator /usr/local/bin/script_creator
```

### Usage

```bash
./script_creator <filename>
```

**Example:**

```bash
./script_creator my_new_script.sh
```

This will:
1. Create `my_new_script.sh` with a pre-filled Bash header
2. Make it executable
3. Open it in `vim` (or your configured editor)

### Generated Header Preview

```bash
#!/usr/bin/env bash

# ---------------------------
# Script   :
# Descrição:
# Versão   :
# Autor    : im-daxter
# Data     : 01/01/2001
# Licença  : GNU/GPL v3.0
# ---------------------------
# Uso:
# ---------------------------
```

### Customization

You can change the default editor by editing the `editor` variable at the top of the script:

```bash
editor="nano"   # or "code", "gedit", "emacs", etc.
```

### License

This project is licensed under the **GNU General Public License v3.0**.
See the [LICENSE](LICENSE) file or visit [gnu.org/licenses/gpl-3.0](https://www.gnu.org/licenses/gpl-3.0.html) for details.

---

## 🇧🇷 Versão em Português

### Sobre

`script_creator` é um utilitário Bash simples e prático que automatiza a criação de novos scripts shell com um cabeçalho padronizado. Desenvolvido como parte do **Curso Introdutório de Shell Script da debxp**, ele garante que todo novo script comece com uma estrutura consistente — incluindo metadados como descrição, versão, autor, data e licença — e abre imediatamente o arquivo no editor de sua preferência.

### Funcionalidades

- ✅ Gera um novo arquivo `.sh` com um template de cabeçalho preenchido
- ✅ Injeta automaticamente a data atual no cabeçalho
- ✅ Define o novo arquivo como executável (`chmod +x`) na criação
- ✅ Abre o arquivo diretamente no editor configurado (padrão: `vim`)
- ✅ Protege contra argumentos ausentes e sobrescrita acidental de arquivos

### Requisitos

- Bash (ou qualquer ambiente de shell compatível com POSIX)
- `vim` (ou substitua a variável `editor` pelo editor de sua preferência)

### Instalação

Clone este repositório e conceda permissão de execução ao script:

```bash
git clone https://github.com/im-daxter/script_creator.git
cd script_creator
chmod +x script_creator
```

Opcionalmente, mova-o para um diretório no seu `$PATH` para uso global:

```bash
sudo cp script_creator /usr/local/bin/script_creator
```

### Uso

```bash
./script_creator <nome_do_arquivo>
```

**Exemplo:**

```bash
./script_creator meu_novo_script.sh
```

Isso irá:
1. Criar `meu_novo_script.sh` com um cabeçalho Bash pré-preenchido
2. Torná-lo executável
3. Abri-lo no `vim` (ou no editor configurado)

### Prévia do Cabeçalho Gerado

```bash
#!/usr/bin/env bash

# ---------------------------
# Script   :
# Descrição:
# Versão   :
# Autor    : im-daxter
# Data     : 01/01/2000
# Licença  : GNU/GPL v3.0
# ---------------------------
# Uso:
# ---------------------------
```

### Personalização

Você pode alterar o editor padrão editando a variável `editor` no topo do script:

```bash
editor="nano"   # ou "code", "gedit", "emacs", etc.
```

### Licença

Este projeto está licenciado sob a **GNU General Public License v3.0**.
Consulte o arquivo [LICENSE](LICENSE) ou acesse [gnu.org/licenses/gpl-3.0](https://www.gnu.org/licenses/gpl-3.0.html) para mais detalhes.

---

<div align="center">

Made with ❤️ as part of the [debxp](https://debxp.org) Shell Script Course

</div>
