<h1 align="center">Olá, eu sou o Luan Vieira 👋</h1>

<p align="center">
  <b>Backend & Dados</b> · Go · Python · SQL · PostgreSQL · MongoDB · IA<br>
  Estudante de Ciência da Computação (Universidade La Salle, 7º semestre) · Canoas/RS
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/luuanvieira/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:luuan.vieira@hotmail.com"><img src="https://img.shields.io/badge/E--mail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail"></a>
</p>

---

## Sobre mim

Sou estudante de Ciência da Computação e trabalho com **desenvolvimento backend, bancos de dados e dados/IA**. Gosto de sistemas que precisam estar corretos: concorrência, consistência e integridade dos dados.

Antes da tecnologia, trabalhei 6 anos na indústria (DuPont / IFF) como operador de processos, monitorando produção, usando SAP e tomando decisões com base em dados. Dessa experiência trouxe disciplina, atenção a processos e o hábito de investigar a causa dos problemas.

**Busco minha primeira oportunidade como desenvolvedor (estágio ou júnior) em backend ou dados.**

---

## Projetos em destaque

### 💰 [Wager Wallet](https://github.com/luuanvieira/wager-wallet): processamento distribuído de apostas em Go
`Go` `Uber Fx` `PostgreSQL` `AWS SQS` `Keycloak (OIDC)` `Docker Compose`

Serviço que movimenta carteiras de jogadores a partir de operações de provedores de jogos, recebidas por HTTP ou fila SQS, com as mesmas garantias nos dois canais.

- Dinheiro em `int64` de centavos (sem ponto flutuante) e **ledger append-only** protegido por constraints e triggers
- **Idempotência persistente** (chave + hash canônico) e inbox para mensagens repetidas
- **Lock por carteira**, testado com 3 instâncias independentes disputando o mesmo saldo
- **Transactional outbox** com publishers concorrentes e recuperação após crash
- Autenticação OIDC com Keycloak e isolamento entre provedores
- Testes de integração com infraestrutura real (sem mocks), `go test -race` e simulações de falha

### 📦 Sistema de Estoque e Análise de Dados
`Python` `MongoDB` `PyMongo` `Power BI` · *projeto em grupo*

Gestão de produtos e estoque de uma loja de artigos de pesca: modelagem no MongoDB, back-end em Python com CRUD completo e dashboard no Power BI com estoque, demanda, mais vendidos e evolução das vendas.


### 🔤 [Analisador Léxico e Sintático: linguagem Elgol](https://github.com/leonunes58/analisador-lexico-sintatico)
`Python` `PLY (Lex-Yacc)` · *projeto em grupo, Compiladores*

Analisador para uma linguagem com regras próprias de identificadores, números e palavras reservadas, com tabela de símbolos, lista de tokens e testes com programas válidos e inválidos.

### 🧪 Laboratório Virtual de Química 3D (TCC)
`Unity` `C#`

Simulador 3D em primeira pessoa para apoiar o ensino de Química em escolas com pouco acesso a laboratórios físicos, com interações com vidrarias e simulação de experimentos.

---

## Tecnologias

**Backend:** Go · Python · FastAPI · APIs REST · Uber Fx
**Dados:** SQL · PostgreSQL · MySQL · Oracle · MongoDB · Power BI · Databricks · PySpark · Pandas · NumPy
**Infra:** Docker · Docker Compose · AWS SQS (LocalStack) · Keycloak · Git
**IA:** OpenAI API · LLMs · integração de IA em aplicações
**Front-end:** JavaScript · TypeScript · Angular · HTML · CSS
**Outros:** C# · Unity

<p>
  <img src="https://skillicons.dev/icons?i=go,python,postgres,mysql,mongodb,docker,aws,fastapi,ts,angular,cs,unity,git" alt="Tecnologias">
</p>

---

## No momento

- 🔧 Aprofundando em Go e sistemas distribuídos (concorrência, mensageria, consistência)
- 📊 Engenharia de dados com Databricks e PySpark
- 🎓 Finalizando o TCC e o analisador da linguagem Elgol
