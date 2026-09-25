# 🐍 Roadmap Python 2026 — Rumo ao Domínio Mundial da Linguagem

### Do zero absoluto até o nível dos melhores desenvolvedores Python do planeta

> Filosofia deste roadmap: os melhores desenvolvedores Python do mundo não são os que decoram mais bibliotecas — são os que entendem a linguagem em profundidade (como o interpretador funciona, por que as coisas são como são), têm fundamentos de ciência da computação sólidos, e conseguem aplicar isso para construir qualquer coisa: automações, scrapers, bots, backends, pipelines de dados, ferramentas de sistema.
>
> Este caminho é universal — qualquer pessoa no mundo, em qualquer país, pode segui-lo. Cada etapa é uma "escada": não pule, porque as etapas avançadas dependem diretamente do domínio das anteriores.
>
> Regra de ouro: nenhuma etapa conta como concluída sem um projeto prático funcionando. Teoria sem prática não constrói nível de verdade.

---

## 🪜 ETAPA 0 — Preparação do Ambiente

- [ ] Instalar Python via `pyenv` (gerenciar múltiplas versões)
- [ ] Configurar `uv` (gerenciador de pacotes/ambientes mais rápido e moderno de 2026)
- [ ] Terminal, shell, editor (VS Code ou Neovim + LSP Pyright/Pylance + Ruff)
- [ ] Git e GitHub — versionar desde o primeiro script
- [ ] Entender `venv` e isolamento de ambientes

**Meta:** criar um venv, instalar um pacote, rodar um script `.py`, versionar num repositório Git.

---

## 🪜 ETAPA 1 — Fundamentos da Linguagem

- [ ] Tipos primitivos: `int`, `float`, `str`, `bool`, `None` (e como Python representa números internamente)
- [ ] Estruturas de dados: `list`, `tuple`, `dict`, `set`, `frozenset` — e a complexidade (Big O) de cada operação
- [ ] Operadores, precedência, mutabilidade vs imutabilidade
- [ ] Controle de fluxo: `if/elif/else`, `for`, `while`, `match/case`
- [ ] Funções: parâmetros, `*args`, `**kwargs`, valores default, closures, funções de primeira classe
- [ ] Escopo (LEGB: Local, Enclosing, Global, Built-in)
- [ ] Compreensões (list/dict/set/generator) e quando cada uma é apropriada
- [ ] Strings: f-strings, métodos, encoding/decoding (UTF-8 e afins), regex com `re`
- [ ] Exceções: hierarquia de `Exception`, `try/except/else/finally`, exceções customizadas
- [ ] Arquivos e context managers (`with`)

**Projeto:** parser de logs de texto que gera estatísticas e relatórios.

---

## 🪜 ETAPA 2 — Python Intermediário e Orientação a Objetos

- [ ] POO completa: classes, herança (simples e múltipla), MRO (Method Resolution Order), polimorfismo, encapsulamento
- [ ] Dunder methods (`__init__`, `__repr__`, `__eq__`, `__hash__`, `__len__`, `__call__`, etc.)
- [ ] `dataclasses` e `attrs`
- [ ] Iteradores e geradores (`yield`, `yield from`, protocolo de iteração)
- [ ] Decoradores — criar os seus próprios, decoradores com argumentos, `functools.wraps`
- [ ] Context managers customizados (`__enter__`/`__exit__`, `contextlib.contextmanager`)
- [ ] Type Hints avançados: `Optional`, `Union`, `Generic`, `Protocol`, `TypedDict`, `overload`
- [ ] Módulos e pacotes: estrutura de projeto real, imports relativos/absolutos
- [ ] `logging` profissional (nunca `print` em produção)
- [ ] `datetime`, `zoneinfo`, manipulação de tempo

**Projeto:** um pequeno framework de CLI orientado a objetos com persistência e logs.

---

## 🪜 ETAPA 3 — Como o Python Funciona por Dentro (o que separa bons de excelentes)

- [ ] O modelo de objetos do Python (tudo é objeto — inclusive funções e classes)
- [ ] Como a memória funciona: referência, contagem de referências, garbage collector
- [ ] O GIL (Global Interpreter Lock) — o que é, por que existe, e seus impactos reais
- [ ] Bytecode e o interpretador CPython (`dis` module para ver o bytecode gerado)
- [ ] Diferença entre CPython, PyPy, e outras implementações
- [ ] Mutabilidade profunda: identidade (`id`), `is` vs `==`, cópia rasa vs profunda (`copy`/`deepcopy`)
- [ ] Metaclasses e `__new__` vs `__init__`
- [ ] Descritores (`__get__`, `__set__`) — como `property` funciona por baixo dos panos
- [ ] O protocolo de dados (data model) do Python — por que ele é tão "hackável"

**Projeto:** implementar seu próprio mini-ORM ou biblioteca de validação de dados usando descritores e metaclasses, do zero.

---

## 🪜 ETAPA 4 — Estruturas de Dados e Algoritmos (fundamentos de Ciência da Computação)

- [ ] Complexidade de tempo/espaço (Big O) aplicada a estruturas nativas do Python
- [ ] Estruturas: pilhas, filas, listas ligadas, árvores, grafos, heaps, hash tables
- [ ] Algoritmos de busca e ordenação (e quando NÃO reinventar a roda usando `heapq`, `bisect`, `collections`)
- [ ] Recursão e programação dinâmica
- [ ] Módulo `collections` a fundo: `deque`, `Counter`, `defaultdict`, `OrderedDict`, `namedtuple`
- [ ] Prática de algoritmos para entender profundamente (LeetCode, Advent of Code, Project Euler)

**Projeto:** resolver 30-50 problemas de algoritmos com foco em entender complexidade, não decorar soluções.

---

## 🪜 ETAPA 5 — Ferramentas e Engenharia de Software Profissional

- [ ] Testes automatizados com `pytest`: fixtures, mocks, parametrize, cobertura de código
- [ ] TDD (Test-Driven Development) — um teste de cada vez, ciclo red-green-refactor
- [ ] Linters/formatadores: `ruff`, `black`, `mypy` (tipagem estática levada a sério)
- [ ] Estrutura de projeto profissional (`src/` layout, `pyproject.toml`, `pytest.ini`)
- [ ] Gerenciamento de dependências e empacotamento com `uv`/`poetry`, publicar no PyPI
- [ ] Documentação: docstrings (Google/NumPy style), `mkdocs` ou `Sphinx`
- [ ] Debugging: `pdb`, breakpoints, profiling (`cProfile`, `py-spy`)
- [ ] Git avançado: rebase interativo, bisect, hooks, workflow de PR em times reais
- [ ] CI/CD com GitHub Actions (testes, lint e deploy automáticos)

**Projeto:** publicar um pacote seu no PyPI, com testes, CI, documentação e versionamento semântico.

---

## 🪜 ETAPA 6 — Automação de Sistemas e Scripts do Mundo Real

- [ ] `os`, `pathlib`, `shutil` (manipulação de arquivos/pastas multiplataforma)
- [ ] `subprocess` — orquestrar comandos e outros programas a partir do Python
- [ ] Agendamento: `cron`, `schedule`, `APScheduler`
- [ ] Manipular Excel (`openpyxl`, `pandas`), PDF (`pypdf`, `pdfplumber`), Word (`python-docx`)
- [ ] Automação de e-mail (`smtplib`, `imaplib`)
- [ ] CLIs profissionais com `typer` ou `click`
- [ ] Empacotar como executável (`pyinstaller`) ou instalável (`pip install`)

**Projeto:** ferramenta de automação de escritório completa (organiza arquivos, gera relatórios, envia por e-mail, roda agendada).

---

## 🪜 ETAPA 7 — Coleta de Dados: Web Scraping e Consumo de APIs

- [ ] HTTP a fundo: métodos, headers, status codes, cookies, sessões
- [ ] `requests` e `httpx` (síncrono e assíncrono)
- [ ] Consumo de APIs REST: autenticação (API key, OAuth2, JWT), paginação, rate limiting
- [ ] Parsing de HTML com `BeautifulSoup` e seletores CSS/XPath
- [ ] Scraping de sites dinâmicos: `Selenium`, `Playwright`
- [ ] Ética e legalidade: `robots.txt`, termos de uso, boas práticas de scraping responsável
- [ ] Scraping em escala com `Scrapy` (framework profissional)
- [ ] Persistência: SQLite, PostgreSQL, MongoDB
- [ ] Scraping assíncrono de alta performance (`asyncio` + `aiohttp`)

**Projeto:** pipeline de coleta de dados que roda diariamente, salva histórico em banco e detecta mudanças/anomalias.

---

## 🪜 ETAPA 8 — Bots e Integrações entre Sistemas

- [ ] Bots de Telegram (`python-telegram-bot`) e Discord (`discord.py`)
- [ ] Webhooks e integração entre serviços diferentes
- [ ] RPA (automação de interface gráfica) com `pyautogui`
- [ ] Consumo de LLMs via API para criar bots inteligentes
- [ ] Filas de tarefas assíncronas: `Celery` + `Redis`/`RabbitMQ`

**Projeto:** bot que consulta uma API/banco de dados, processa a informação e interage de forma autônoma com usuários.

---

## 🪜 ETAPA 9 — Concorrência e Paralelismo (nível avançado de verdade)

- [ ] `asyncio` profundo: event loop, `async/await`, `Task`, `gather`, `TaskGroup`
- [ ] Diferença real entre concorrência e paralelismo
- [ ] `threading` (I/O bound) vs `multiprocessing` (CPU bound) — e o papel do GIL aqui
- [ ] `concurrent.futures`
- [ ] Sincronização: locks, semáforos, filas entre processos/threads
- [ ] O futuro do GIL: entender o modo "free-threaded" do CPython (PEP 703) e seu impacto

**Projeto:** reescrever um scraper síncrono em versão assíncrona e comparar performance com benchmarks reais.

---

## 🪜 ETAPA 10 — Backend, APIs e Bancos de Dados

- [ ] `FastAPI` (padrão de mercado global em 2026 — moderno, tipado, assíncrono)
- [ ] `Flask` (ainda relevante em projetos legados/simples)
- [ ] Autenticação/autorização (JWT, OAuth2, sessões)
- [ ] ORMs: `SQLAlchemy`, `SQLModel` — e SQL puro para entender o que o ORM abstrai
- [ ] Migrations (`Alembic`)
- [ ] Documentação automática de API (OpenAPI/Swagger)
- [ ] Docker: containerizar aplicações Python
- [ ] Deploy: VPS com `gunicorn`/`uvicorn` + Nginx, ou plataformas como Railway/Render/Fly.io

**Projeto:** transformar os dados coletados na Etapa 7 em uma API própria, documentada e dockerizada.

---

## 🪜 ETAPA 11 — Dados em Escala (Data Engineering aplicado)

- [ ] `pandas` avançado (limpeza, transformação, performance com grandes volumes)
- [ ] `numpy` (base matemática/vetorial de todo o ecossistema de dados)
- [ ] Pipelines de dados (ETL) com `Airflow` ou `Prefect`
- [ ] Noções de Big Data com `PySpark`
- [ ] Visualização: `matplotlib`, `plotly`

**Projeto:** pipeline automatizado ponta a ponta — coleta, transforma, armazena e exibe os dados em um dashboard.

---

## 🪜 ETAPA 12 — Arquitetura de Software e Engenharia de Elite

- [ ] Design Patterns em Python (Factory, Singleton, Strategy, Observer, Adapter)
- [ ] Princípios SOLID aplicados de forma "pythônica"
- [ ] Clean Architecture / Arquitetura Hexagonal
- [ ] Domain-Driven Design (DDD) — quando e por que usar
- [ ] Otimização de performance extrema: `Cython`, integração com `Rust` via `PyO3`
- [ ] Observabilidade em produção: métricas, tracing, `Sentry`, logs estruturados
- [ ] Segurança: SQL Injection, gestão de segredos, dependências vulneráveis (`pip-audit`, `bandit`)
- [ ] Ler código-fonte de projetos open source grandes (Django, FastAPI, Requests) para aprender com quem já domina

**Projeto:** reescrever seu maior projeto seguindo Clean Architecture, com observabilidade e segurança de nível produção.

---

## 🪜 ETAPA 13 — Especialização (escolha 1-2 trilhas conforme seu interesse)

- [ ] **Automação/RPA avançado** — orquestração de múltiplos bots, Selenium Grid
- [ ] **Data Science / Machine Learning** — `scikit-learn`, `pytorch`, fundamentos estatísticos
- [ ] **Backend distribuído sênior** — microsserviços, mensageria, arquitetura de sistemas em escala
- [ ] **Segurança ofensiva/defensiva** — scripts de pentest ético, análise de vulnerabilidades
- [ ] **Compiladores/linguagens** — entender como criar uma linguagem simples em Python (parser, AST, interpretador)

---

## 🪜 ETAPA 14 — Portfólio, Comunidade e Reconhecimento Global

- [ ] GitHub com projetos reais, bem documentados (README de qualidade, não só código)
- [ ] Contribuir com projetos open source relevantes internacionalmente
- [ ] Escrever sobre o que aprende (blog, artigos técnicos em inglês para alcance global)
- [ ] Participar de comunidades globais (PyCon, fóruns, Discord de Python, Stack Overflow)
- [ ] Resolver problemas de nível alto em plataformas competitivas (Codeforces, LeetCode, Advent of Code)
- [ ] Rede de contatos internacional (LinkedIn em inglês, contribuições visíveis)

---

## 📚 Recursos Que Todo Especialista Mundial Conhece

- **Livros:** _Fluent Python_ (Luciano Ramalho), _Effective Python_ (Brett Slatkin), _Python Tricks_ (Dan Bader), _Architecture Patterns with Python_, _Designing Data-Intensive Applications_ (não é só Python, mas todo engenheiro sênior leu)
- **Fonte primária:** documentação oficial do Python (docs.python.org) e PEPs (Python Enhancement Proposals) — ler as PEPs importantes é o que faz alguém entender o "porquê" das decisões da linguagem
- **Prática:** Advent of Code, Codewars, Exercism, LeetCode
- **Código-fonte:** ler o código do CPython em si (github.com/python/cpython) quando estiver em nível avançado — é o que os core developers fazem

---

## ⏱️ Ritmo Realista

Com 1-2h/dia de dedicação consistente: etapas 0-2 levam 4-8 semanas; etapas 3-9 (o "coração" do domínio técnico) levam de 3 a 6 meses; etapas 10-14 (nível de elite/especialização) são uma jornada contínua que nunca termina de verdade — os melhores do mundo continuam aprendendo a vida toda.

**Não existe atalho para maestria.** Existe consistência, prática deliberada e curiosidade genuína sobre "por que" as coisas funcionam, não só "como" usá-las.
