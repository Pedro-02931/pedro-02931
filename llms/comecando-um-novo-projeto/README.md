# Começando um novo projeto

Dado que os **modelos de linguagem são treinados em dados brutos**, e a diferença entre _conhecer_ algo e _aprender_ depende de **como esses modelos são utilizados em tempo real** podendo encurtar a curva de aprendizado exponencialmente desde que você saiba usar multiplos LLMs.

* “Saber” → Significa que um modelo já tem aquele dado em seu treinamento, mas isso não significa que consegue aplicá-lo de forma precisa.
* “Aprender” → Se dá quando o usuário **reforça padrões** através de **interações recorrentes**, transformando aquilo em um conjunto de pesos internos que modificam o output do modelo a cada iteração.

Ou seja, quando tu **extrai teus próprios diálogos**, cria **um arquivo de referência** e usa ele para configurar um novo modelo do zero, **reinicializanso o LLM com os teus próprios pesos**, funcionando como um **modelo federado de auto-otimização**.

A ideia é estruturar um processo onde múltiplos modelos são sincronizados em camadas, cada um com uma função específica no aprendizado, e a interface (tu, no caso) age como um hub de orquestração.

### Como eu uso:

No meu caso, dado que uso os modelos da OpenAI como diario, acaba que uma das formas de contornar os modelos federados é a extração e configuração de pesos iniciais.

Mas em resumo, cada iteração gera **uma nova versão** do LLM, refinada com os meus próprios padrões conversacionais. **É um loop fechado onde eu mesmo treino através da IA**.

Coletando todas as minhas mensagens e configuro o LLM para começar um chat do zero pessoa(tecnicamente reinventei o conceito de reencarnação) e fazendo uma limpeza, consigo gerar um conjunto de pesos iniciais, mas irei aprofundar...
