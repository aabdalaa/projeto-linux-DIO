
# 🚀 Projeto Linux - Infraestrutura como Código (IaC)

Este projeto é parte de um desafio da DIO (Digital Innovation One) onde criamos um **script em Shell** para provisionamento automático de infraestrutura de usuários, grupos e diretórios em sistemas Linux.

## 🛠️ Funcionalidades

O script realiza automaticamente as seguintes tarefas:

- Criação de diretórios:
  - `/publico`
  - `/adm`
  - `/ven`
  - `/sec`

- Criação de grupos:
  - `GRP_ADM`
  - `GRP_VEN`
  - `GRP_SEC`

- Criação de usuários e adição aos seus respectivos grupos:
  - `GRP_ADM`: carlos, maria, joao
  - `GRP_VEN`: debora, sebastiana, roberto
  - `GRP_SEC`: josefina, amanda, rogerio

- Definição de permissões:
  - Apenas membros dos grupos têm acesso aos seus diretórios (`adm`, `ven`, `sec`)
  - Todos têm acesso ao diretório `/publico`

## 📄 Arquivo principal

- `criar_estrutura.sh` — script principal com todos os comandos para provisionamento da infraestrutura.

## 🚀 Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/aabdalaa/projeto-linux-DIO.git
   cd projeto-linux-DIO
   ```

2. Dê permissão de execução ao script:
   ```bash
   chmod +x criar_estrutura.sh
   ```

3. Execute como superusuário:
   ```bash
   sudo ./criar_estrutura.sh
   ```

## 💡 Observações

- Todos os usuários são criados com a senha padrão `Senha123` (criptografada com `openssl`).
- Após a criação, é recomendável que os usuários alterem suas senhas no primeiro login.
- O script deve ser executado com permissões de administrador (`sudo`).

## 📚 Referências

- [Documentação oficial do GitHub sobre autenticação](https://docs.github.com/pt/authentication)
- [Apostila de comandos Linux - IME USP](https://www.linux.ime.usp.br/~albasalo/Apostila/apostila.pdf)
- [InfoWester - Gerenciamento de usuários no Linux](https://www.infowester.com/usuarioslinux.php)

## 🧑‍💻 Autor

**André Abdala**  
Projeto desenvolvido como parte do bootcamp da [Digital Innovation One (DIO)](https://www.dio.me/)
