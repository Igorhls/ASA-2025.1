# ASA-Entrega-02

Infraestrutura com Docker Compose contendo:

- Servidor DNS (Bind9) com zona primária `asa.br`
- Proxy reverso (Nginx) com redirecionamento baseado no host
- Dois servidores web com páginas personalizadas

## Como executar

1. Clone o repositório:

```bash
git clone <URL-do-repo>
cd ASA-Entrega-02
```

2. Suba os containers:

```bash
docker-compose up --build
```

3. Acesse no navegador:

- http://beta.asa.br
- http://alpha.asa.br

## Estrutura

```
ASA-Entrega-02/
├── dns/
│   ├── Dockerfile
│   ├── db.asa.br
│   └── named.conf.local
├── proxy/
│   ├── Dockerfile
│   ├── default.conf
│   └── index.html
├── web/
│   ├── Dockerfile
│   └── index.html
└── docker-compose.yml
```

---

**Autor:** Igor 
**Data:** Junho de 2025