# WebGuard_Scanner
Ferramenta que verifica aplicações web em busca de vulnerabilidades comuns, como XSS, SQL Injection, diretórios expostos e configuração de headers de segurança.


## Projeto



```mermaid

graph TD
    subgraph Backend
        A[Python Backend] --> B[Verificador de SQL Injection]
        A --> C[Testador de XSS]
        A --> D[Scanner de Diretórios]
        A --> E[Analisador de Headers HTTP]
        A --> F[Varredura de Portas com Socket e Nmap]
    end

    subgraph Frontend
        G[React Front-end] --> H[Interface de Entrada de URL]
        G --> I[Botão de Iniciar Varredura]
        G --> J[Painel de Relatórios de Vulnerabilidades]
        G --> K[Histórico de Varreduras]
        G --> L[Exportação de Relatório em PDF/CSV]
    end

    subgraph Integração
        M[API Flask/FastAPI] --> A
        G --> M
        M --> N[Banco de Dados SQLite/MongoDB]
    end

```

## Front-end 

```mermaid

graph TD
    A[React Front-end] --> B[Interface de Entrada de URL]
    A --> C[Botão de Iniciar Varredura]
    A --> D[Painel de Relatórios de Vulnerabilidades]
    A --> E[Histórico de Varreduras]
    A --> F[Exportação de Relatório em PDF/CSV]

    subgraph Tecnologias
        G[HTML/CSS]
        I[Gráficos e Visualização]
    end

    B --> G
    C --> G
    D --> G
    E --> G
    F --> G
    D --> I
    E --> I

```

##  Back-end
```mermaid
graph TD
    A[Python Backend] --> B[Verificador de SQL Injection]
    A --> C[Testador de XSS]
    A --> D[Scanner de Diretórios]
    A --> E[Analisador de Headers HTTP]
    A --> F[Varredura de Portas com Socket e Nmap]

    subgraph Biblioteca
        G[Requests]
        H[BeautifulSoup]
        I[Socket]
        J[Nmap]
    end

    B --> G
    C --> G
    D --> G
    E --> G
    F --> I
    F --> J

```
