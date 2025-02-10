# 🛡️ BunkerWeb Top Security

🚀 **Protegendo seu servidor contra ataques DDoS e exploits!**  
Este projeto nasceu após enfrentar **uma invasão hacker seguida de um ataque DDoS** no meu HomeLab baseado em Proxmox. A experiência me levou a aprofundar meus conhecimentos em **segurança cibernética, firewalls e proteção de servidores**, resultando neste **Docker Compose** altamente seguro, usando **BunkerWeb** e outras camadas de proteção.

📖 **História completa da invasão e solução** no LinkedIn:  
🔗 [Como sobrevivi a um ataque DDoS no Proxmox](https://www.linkedin.com/pulse/como-sobrevivi-um-ataque-ddos-proxmox-seguido-por-invas%C3%A3o-heberty-ti7xf)

---

## 🔥 Motivação

Durante minha jornada com um **servidor caseiro (HomeLab)**, aprendi da pior forma sobre os riscos de **expor portas críticas (HTTP, SSH, etc.) na internet sem camadas adicionais de segurança**. Após sofrer diversas tentativas de invasão e um ataque massivo de **DDoS**, implementei **BunkerWeb**, um firewall baseado em contêineres, para bloquear ataques e proteger meu servidor.

💡 Com este repositório, compartilho um **Docker Compose otimizado**, incluindo:
- 🔒 **BunkerWeb** (proxy reverso seguro e firewall HTTP)
- 🌍 **Regras para bloquear acessos por país e User-Agent**
- 🚫 **Proteção contra Exploits conhecidos**
- ⚙️ **Configuração fácil e modular para qualquer servidor**

---

## 📦 Tecnologias Utilizadas

- **[BunkerWeb](https://github.com/bunkerity/bunkerweb)** - Firewall OpenSource de proteção para servidores web
- **Nginx Proxy Manager** - Para gerenciar domínios e certificados SSL
- **Docker & Docker Compose** - Para facilitar a implantação
---

## 🚀 Como Usar

### 1️⃣ **Clone o Repositório**
```sh

git clone https://github.com/JohnHeberty/BunkerWeb-Top-Security.git
cd BunkerWeb-Top-Security
```

### 2️⃣ **Alterando a Senha do Banco de Dados**
```sh
nano docker-compose.yaml
Alt + R # Para alterar a senha padrão
changeme # Tag para alterar a senha
<Your-Passworkd> # Digite a Sua Senha
Enter # Para fazer o replace
Y # Para confirmar o replace
Ctrl + X # Para Salvar e Sair
Y # Para confirmar a Saida
Enter # Salvar e Sair
```
Agora sua senha foi alterada com sucesso! 🚀

### 3️⃣ **Suba o Container**
```sh
docker compose up -d
```
### 4️⃣ **Verifique os Logs para garantir que tudo está rodando**
```sh
docker logs -f bunkerweb
```

---
### 🤝 Contribuições
---

Sinta-se à vontade para abrir issues, enviar comits e sugerir melhorias! 🚀

Toda ajuda é bem-vinda para aprimorar essa solução e fortalecer a segurança da comunidade.

---
### 📞 Contato
---
🧑‍💼 **Linkedin**: [John Heberty](https://www.linkedin.com/in/john-heberty/)

✉️ **E-mail**: john.7heberty@gmail.com

🔥 Proteja seu servidor e evite passar pelo mesmo que eu passei! 🔥

