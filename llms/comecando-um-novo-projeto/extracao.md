# Extração

A primeira parte que executo é o mapeamento inicial, onde através do inspecionar, executo um código que permite a extração e limpeza dos dados, facilitando a analise do LLM, desabilitando tensores desnecessários.

Cada mensagem que passa é como se fosse um “bit de peso” acumulado, influenciando o treinamento incremental do modelo federado. É um efeito exponencial– quanto mais mensagens, mais o dispositivo sente o peso, tipo um payload que vai aumentando de massa, dependendo do uso do usuário.

Isso é uma **ótica computacional avançada**, porque ao tratar interações humanas da mesma forma que **uma rede neural trata gradientes** durante o aprendizado. No fundo, estou aplicando **um modelo de inferência probabilística** pra entender minha própria cognição através da IA.

### Script:

1. No caso, o script inicial foi gerado por IA, onde eu coleto a classe que identifica as tags que guandam os prompts produzido

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

2. Executo o script para a coleta dos blocos dentro da tag `div.whitespace-pre-wrap`&#x20;

{% code overflow="wrap" %}
```javascript
(() => {
  const a = [...document.querySelectorAll("div.whitespace-pre-wrap")] // Seleciona todas as mensagens
    .map(msg => msg.innerText.trim() // Remove espaços extras para compactação
    .replace(/\s+/g, " ")) // Normaliza quebras de linha
    .filter(msg => msg.length); // Filtra mensagens vazias

  // Itera e exibe no console, incluindo o título do chat
  a.forEach((msg, idx) => console.log(`Chat: ${document.title} | Mensagem ${idx + 1}: ${msg}`));
})();

```
{% endcode %}

3. Assim eu executo o script no console, gerando um conjunto de mensagens brutas para o meu mapeamento

Com isso, eu gero **um dataset personalizado** que pode ser usado para alimentar um novo modelo, configurando ele com **teus próprios padrões de linguagem e estilo**.

{% hint style="info" %}
No caso, sempre tento repetir esse snip manualmente para focar no reforço e aprendizado da lógica.
{% endhint %}
