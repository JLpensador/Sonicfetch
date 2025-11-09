# 🌀 SonicFetch
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

Uma personalização completa do **Fastfetch**, com tema inspirado no **Sonic the Hedgehog**.  
Inclui ícones coloridos, divisórias ASCII e exibição organizada das informações do sistema Linux.

<img width="1920" height="1005" alt="sonicfetch" src="https://github.com/user-attachments/assets/65e2bc6b-fc37-49a8-96c8-03dc998731e0" />

---

## 📦 Sobre o projeto

O **SonicFetch** foi criado para deixar o terminal com um visual único e autêntico, destacando informações do sistema como:
- 🖥️ Sistema operacional, kernel e uptime  
- 💻 Ambiente gráfico, tema, ícones e terminal  
- ⚙️ CPU, GPU, memória e armazenamento  
- 🎨 Paleta de cores do sistema  

Tudo isso com uma **logo do Sonic renderizada diretamente no terminal** (usando `kitty-direct`).

## 🚀 Pré-requisitos

Antes de começar, você precisa ter instalado:

```bash
sudo apt install fastfetch
```
---

## ⚙️ Instalação

1️⃣ Clone este repositório:

```bash
git clone https://github.com/JLpensador/Sonicfetch.git
```

2️⃣ Crie (caso não exista) a pasta de configuração do Fastfetch:

```bash
mkdir -p ~/.config/fastfetch
```

3️⃣ Copie os arquivos de personalização:

```bash
cp SonicFetch/config.json ~/.config/fastfetch/
cp SonicFetch/Sonic.png ~/.config/fastfetch/
```

4️⃣ Execute:

```bash
fastfetch
```
---

## 🎨 Estrutura do layout

O layout exibe informações separadas em blocos, com ícones para fácil identificação:

```yaml
╭───────────── 󰣙  user
│  System Information
│ 󰍹 OS: ...
│ 󰒋 Kernel: ...
│ 󰅐 Uptime: ...
│ ...
│  Desktop Environment
│ ...
│  Hardware Information
│ ...
│ ◇◇◇ Color Palette
╰───────────────────────────────╯
```
---

## 🖼️ Personalização

O arquivo principal de configuração é o config.json.
Você pode editar livremente os módulos, ícones e cores.
A imagem do Sonic é carregada via protocolo kitty-direct (funciona em terminais como Kitty e WezTerm).

Para usar outra imagem:


```json
"logo": {
  "source": "~/.config/fastfetch/MinhaImagem.png",
  "type": "kitty-direct",
  "width": 40,
  "height": 19
}
```
---

## 💙 Créditos
- [Fastfetch CLI](https://github.com/fastfetch-cli/fastfetch "Fastfetch CLI")
- Tema e logo inspirados em Sonic the Hedgehog
- Customização criada por João Luiz B. Morais
