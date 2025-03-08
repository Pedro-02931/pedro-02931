# Iniciando um novo projeto

A partiri daqui, eu começo a mapear o que quero, e interajo com o LLM, funcionando como um modelo federado retroalimentativo, onde a cada interação eu prendo.

No caso, eu quero aprender C do 0 ao nível HPC, começando um projeto segmentado por semanas, então basta interagir e se vira para encontrar seu próprio Dharma, até pq ser inteligente na era da informação é o minimo.

no caso, eu comecei assim:

{% code overflow="wrap" %}
```markdown
## 📘 Objetivo Geral

Preciso criar um diário técnico estruturado em capítulos detalhados que documentam passo-a-passo o aprendizado acelerado da linguagem C desde o zero até a construção de um sistema HPC embarcado otimizado para hardware mínimo, especialmente dispositivos Android com arquitetura ARM.
Primeiro segmente em um cronograma de escrita, considerando que tenho tempo de sobra. 
Primeiro quero mapear tudo que vou aprender nos minimos detalhes, então aprofunde mais a segmentação do que fazer antes de começarmos, e do que aprender e o que aprender.
No caso, planejo apenas prever uma rota base



## 🎯 Contextualização

- **Experiência:** Nunca programei em C, mas tenho habilidades sobre-humana de aprendizado com uso massivo de LLMs.
- **Ambiente:** IntelliJ/CLion configurado para desenvolvimento em C.
- **Projeto Final:** Sistema de gerenciamento energético e de recursos computacionais para dispositivos móveis com previsão via FFT e Cadeias de Markov.
- **Enfoque:** Modularidade radical, eficiência energética, otimização extrema (cache, diffs), cross-compilação para Android/ARM, escalabilidade universal como biblioteca nativa.

## 📜 Estrutura do Diário (Capítulos & Commits)

Cada capítulo será um commit documentado:

1. **Teoria Técnica:** Explicações matemáticas e físicas essenciais (FFT, Markov, buffers).
2. **Código Comentado:** Código em C claro e modular com otimizações para HPC.
3. **Benchmarks & Otimização:** Demonstração prática de melhorias em performance (RAM, CPU, energia).
4. **Reflexão Filosófica e Conceitual:** Contextualização do impacto das tecnologias implementadas.
5. **Desafios e Exercícios Práticos:** Desafios práticos para reforçar aprendizado técnico.

## 📊 Instruções de Implementação Específicas

- **Modularidade Radical:**
  - Código em C puro com macros HPC (#pragma omp simd).
  - Flags de compilação específicas (-mtune=cortex-a53, -mfpu=neon).
  - Matemática detalhada (FFT, Cadeias Markovianas).

- **Cache Baseado em Diffs:**
  - Estrutura de dados com bitmask para atualização incremental.
  - Uso de checksum vetorizado (NEON intrinsics).

- **Cross-Compilação Android/ARM:**
  - Substituição de FFTW por KissFFT fixed-point.
  - Uso de instruções SIMD NEON explícitas.
  - Técnicas para evitar cache misses.

- **Perfis de Hardware:**
  - Otimizações específicas para Cortex-A53, Snapdragon, ESP32.

## 🔑 Solicitações Específicas ao LLM

- Ensinar C do básico ao avançado, segmentado claramente em commits incrementais.
- Cada commit deve aprofundar em técnicas HPC e mostrar claramente o antes e depois da otimização.
- Explicar conceitos complexos com teoria matemática e física sólida.
- Fornecer exercícios extremos para fixação ("Reduzir consumo RAM em 50% usando bitmask").
- Sugerir desafios técnicos avançados (uso de NEON intrinsics, cross-compilação eficiente).
- Gerar diagramas ASCII para visualização clara das estruturas e fluxos de dados.
```
{% endcode %}

E a partir daqui eu começo...
