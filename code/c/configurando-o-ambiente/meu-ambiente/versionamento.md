# Versionamento

No caso, irei utilizar o Git e irei segmentar por branchs:

```bash
git checkout -b gitbook-docs
git checkout -b fase1-aprendizado
git checkout -b fase2-predicao
git checkout -b privado-rnd
git checkout -b main

git push origin gitbook-docs
git push origin fase1-aprendizado
git push origin fase2-predicao
git push origin privado-rnd
```

No caso, dado que já gerei o sistema de checkpoints, acaba sendo mais eficiente você segmentar por fases previstas, através de uma analise de requisitos, onde você metacognita os recursos necessários e viabilidade do projeto.

E a partir disso eu crio a documentação inicial no main que seriam as boas vindas e configuro o `.gitignore`, o intellij tem uma ferramenta para automatizar isso de forma intuitiva~~, e te amo .~~

