<h1 align="center">Olá, eu sou o Luan Vieira 👋</h1>

<p align="center">
  <b>Backend & Dados</b> · Go · Python · SQL · PostgreSQL · MongoDB · IA<br>
  Estudante de Ciência da Computação (Universidade La Salle, 7º semestre) · Canoas/RS
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/luuanvieira/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:luuan.vieira@hotmail.com"><img src="https://img.shields.io/badge/E--mail-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="E-mail"></a>
</p>

---

## Sobre mim

Sou estudante de Ciência da Computação e trabalho com **desenvolvimento backend, bancos de dados e dados/IA**. Gosto de sistemas que precisam estar corretos: concorrência, consistência e integridade dos dados.

Antes da tecnologia, trabalhei 6 anos na indústria (DuPont / IFF) como operador de processos, monitorando produção, usando SAP e tomando decisões com base em dados. Dessa experiência trouxe disciplina, atenção a processos e o hábito de investigar a causa dos problemas. Vários dos meus projetos nascem dela: monitoramento de processo, gestão de alarmes, OEE e rastreabilidade de lotes.

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

### 🏭 [Monitor de Processo Industrial](https://github.com/luuanvieira/monitor-processo): gestão de alarmes em tempo real
`Go` `PostgreSQL` `Server-Sent Events` `Prometheus` `Docker`

Simulador de uma unidade industrial (tanque, bomba e reator) com motor de alarmes no padrão ISA-18.2 e dashboard ao vivo. Dá para injetar falhas (perda de resfriamento, desarme de bomba, sensor travado) e ver a cascata de alarmes.

- Banda morta, atraso de ativação, taxa de variação, detecção de sensor travado e supressão por qualidade ruim do sinal
- **Carta de controle EWMA** que avisa sobre o desgaste da bomba cerca de **1 hora antes** do alarme de vibração alta
- Alarmes falsos medidos em 40 simulações de 12 h e reduzidos a zero
- Pipeline concorrente com gravação em lote, backpressure e encerramento sem perda de dados

### 🌧️ [Clima no RS](https://github.com/luuanvieira/inmet-rs-pipeline): pipeline de dados do INMET
`Python` `DuckDB` `dbt` `Streamlit` `GitHub Actions`

Pipeline de ponta a ponta com os dados públicos das estações meteorológicas do Rio Grande do Sul (2020–2026), em camadas bronze, silver e gold, com testes de qualidade e dashboard.

- Parser robusto para os arquivos do INMET, cujo formato muda ao longo dos anos
- Tratamento de qualidade: sensores com defeito, dias incompletos e efeito do fuso horário
- Mostra com dados as **enchentes de maio de 2024**: mais de 500 mm no mês em Porto Alegre e 216 mm em um único dia em Soledade

### 🧪 [SQL na Fábrica](https://github.com/luuanvieira/fabrica-sql): data warehouse de uma indústria de aromas
`PostgreSQL` `PL/pgSQL` `Python` `pytest`

Banco de um ano de operação de uma fábrica (dados fictícios), com as regras de negócio dentro do banco e 11 consultas analíticas respondendo perguntas de chão de fábrica.

- Triggers e *exclusion constraints*: não consome lote vencido ou em quarentena, não expede lote reprovado
- **Rastreabilidade com CTE recursiva**: um lote de matéria-prima suspeito chega a 34 lotes e 11 clientes
- OEE, Pareto de paradas, MTBF/MTTR, Cpk e *gaps and islands* com funções de janela e `range_agg`

### Outros projetos

- 📦 **Sistema de Estoque e Análise de Dados**: Python, MongoDB e Power BI para uma loja de artigos de pesca *(em grupo)*
- 🔤 **[Analisador Léxico e Sintático da linguagem Elgol](https://github.com/leonunes58/analisador-lexico-sintatico)**: Python e PLY, para a disciplina de Compiladores *(em grupo)*
- 🧪 **Laboratório Virtual de Química 3D (TCC)**: simulador em Unity e C# para apoiar o ensino de Química em escolas sem laboratório

---

## Tecnologias

- **Backend:** Go · Python · FastAPI · APIs REST · Uber Fx
- **Dados:** SQL · PostgreSQL · PL/pgSQL · DuckDB · dbt · MySQL · Oracle · MongoDB · Power BI · Databricks · PySpark · Pandas
- **Infra:** Docker · Docker Compose · GitHub Actions · AWS SQS (LocalStack) · Keycloak · Git
- **IA:** OpenAI API · LLMs · integração de IA em aplicações
- **Front-end:** JavaScript · TypeScript · Angular · HTML · CSS
- **Outros:** C# · Unity

<p>
  <img src="https://skillicons.dev/icons?i=go,python,postgres,mysql,mongodb,docker,githubactions,aws,fastapi,ts,angular,cs,unity,git" alt="Tecnologias">
</p>

---

## No momento

- 🔧 Aprofundando em Go e sistemas distribuídos (concorrência, mensageria, consistência)
- 📊 Engenharia de dados com dbt, Databricks e PySpark
- 🎓 Finalizando o TCC e o analisador da linguagem Elgol
