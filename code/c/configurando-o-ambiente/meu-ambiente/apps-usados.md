# Apps Usados

Meu propósito é usar as três ferramentas:

#### **1. GitHub → Repositório Público**

* &#x20;Armazena o código-fonte e a documentação pública.&#x20;
* Permite que a comunidade acesse e contribua.
* Se integra automaticamente ao **GitBook** para documentação viva.

#### **2. GitLab → Repositório Privado + CI/CD + Automação**

* Gerencia código privado (ex.: features experimentais, módulos avançados).
* Automatiza **testes, benchmarks e deploys contínuos** com CI/CD.
* Sincroniza com o **GitHub** para espelhar atualizações públicas.

#### &#x20;**3. GitBook → Documentação Técnica**

* Conectado diretamente ao **GitHub**, qualquer commit em `gitbook-docs` reflete na documentação.
* Pode ser atualizado automaticamente via **GitHub Actions** ou **GitLab CI/CD**.

O resultado é um **fluxo de versionamento modular**, onde cada commit é propagado entre as camadas de infraestrutura, garantindo que a evolução do código, a documentação e os testes sigam **uma progressão paralela**, sem redundâncias e sem gargalos operacionais.&#x20;

Isso transforma o próprio versionamento em um **sistema federado de aprendizado e desenvolvimento**, onde cada repositório opera como um **nó autônomo**, mas totalmente sincronizado dentro da tua arquitetura cognitiva de produção.
