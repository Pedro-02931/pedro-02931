# Apps Usados

Hoje em dia, na era da informação, clareza é poder, então quanto mais você documentar e mais ferramentas vc segmentar, melhor, pois reduz a carga de trabalho que você teria, pois sempre teria em mãos o que vc fez.

A minha ideia é **sincronizar GitHub, GitLab e GitBook**, criando um **pipeline integrado** onde **cada plataforma cumpre um papel específico**, sem precisar ficar copiando código manualmente. A ideia aqui é **automatizar o fluxo** pra que qualquer mudança no código/documentação seja propagada entre os sistemas.

#### **📌 1. GitHub → Repositório Público**

✅ Armazena o código-fonte e a documentação pública.\
✅ Permite que a comunidade acesse e contribua.\
✅ Se integra automaticamente ao **GitBook** para documentação viva.

#### **📌 2. GitLab → Repositório Privado + CI/CD + Automação**

✅ Gerencia código privado (ex.: features experimentais, módulos avançados).\
✅ Automatiza **testes, benchmarks e deploys contínuos** com CI/CD.\
✅ Sincroniza com o **GitHub** para espelhar atualizações públicas.

#### **📌 3. GitBook → Documentação Técnica**

✅ Conectado diretamente ao **GitHub**, qualquer commit em `gitbook-docs` reflete na documentação.\
✅ Pode ser atualizado automaticamente via **GitHub Actions** ou **GitLab CI/CD**.
