# Missão Aurora Siger — Sistema de Verificação de Pré-Decolagem

Atividade Integradora — Fase 1 (Decolagem da Missão) | Curso Ignition Zero

Sistema de verificação pré-decolagem para telemetria espacial — algoritmo em Python que valida temperatura, integridade estrutural, energia, pressão dos tanques e módulos críticos antes de autorizar o lançamento.


## Explicação do projeto

Este projeto implementa um sistema de verificação de pré-decolagem para a nave fictícia Aurora
Siger, desenvolvido como atividade integradora da Fase 1 do curso Ignition Zero. O objetivo é
decidir, de forma automatizada, entre autorizar ("PRONTO PARA DECOLAR") ou abortar ("DECOLAGEM
ABORTADA") a decolagem, com base na comparação de dados de telemetria contra faixas de segurança
predefinidas. O desenvolvimento integra conceitos de oito capítulos do curso, do histórico da
computação até inteligência artificial e eficiência energética, aplicando cada um deles a uma
parte concreta do sistema.

**Capítulo 1 — Ignition Zero: O Início da Aurora.** Este capítulo apresentou o cenário da missão
Aurora Siger e o desafio da atividade integradora, servindo como ponto de partida narrativo e
técnico para todo o projeto: a necessidade de um sistema confiável de decisão GO/NO-GO antes da
decolagem.

**Capítulo 2 — Mercado e Tecnologia.** Trouxe os fundamentos de responsabilidade social
empresarial (ISO 26000) e sustentabilidade tecnológica (Green IT, Triple Bottom Line). Esses
conceitos foram diretamente aplicados na seção 1.6 (Reflexão crítica), ao discutir accountability
e transparência do algoritmo de decisão, e ao analisar o impacto social e ambiental da missão sob
a ótica do tripé *People, Planet, Profit*.

**Capítulo 3 — Os Fundamentos que Despertam o Universo da Computação.** O histórico da computação
(do ábaco aos processadores modernos) contextualizou por que sistemas embarcados como o da nave
Aurora Siger são capazes de tomar decisões automatizadas em tempo real — a evolução de máquinas de
calcular mecânicas até circuitos integrados é o que torna viável rodar o algoritmo de verificação
a bordo.

**Capítulo 4 — A Lógica que Define Cada Decisão no Cérebro Digital da Nave.** O estudo de sistemas
numéricos (decimal, binário) fundamentou o uso de valores booleanos (0/1) na telemetria — como os
campos de integridade estrutural e status dos módulos críticos — que são a base das comparações
lógicas do algoritmo.

**Capítulo 5 — Os Primeiros Traços que Estruturam o Pensamento Algorítmico.** Os conceitos de
algoritmos, fluxogramas e operadores lógicos deste capítulo foram aplicados diretamente na
construção do pseudocódigo da seção 1.2, definindo a sequência de verificações (SE...ENTÃO) que
decide o veredito da missão.

**Capítulo 6 — As Estruturas Lógicas que Sustentam as Primeiras Escolhas da Missão.** Estruturas
condicionais e de repetição mais avançadas, estudadas neste capítulo, foram implementadas na
função `verificar_leitura()` (seção 1.3), que percorre múltiplos tanques e módulos críticos usando
laços (`for`) e condicionais (`if`) para consolidar todas as falhas antes de gerar o veredito
final.

**Capítulo 7 — O Surgimento da Inteligência que Apoia a Tomada de Decisão.** Os conceitos de
classificação de dados e identificação de padrões (aprendizado de máquina) fundamentaram a seção
1.5, na qual uma IA foi utilizada para classificar as leituras de telemetria por categoria de
risco e identificar anomalias, como o salto de temperatura interna e a queda simultânea de
integridade e pressão no Cenário 2.

**Capítulo 8 — A Energia que Sustenta o Primeiro Impulso da Missão.** Os princípios físicos de
eficiência energética (incluindo a Segunda Lei da Termodinâmica e indicadores como o PUE)
embasaram tanto o cálculo de autonomia da seção 1.4 quanto a discussão sobre sustentabilidade
tecnológica da seção 1.6, relacionando as perdas energéticas da nave a métricas reais de
eficiência usadas em data centers.

A integração dos oito capítulos permitiu construir um sistema completo: da lógica binária que
representa o estado dos sensores, passando pelo algoritmo de decisão estruturado em pseudocódigo e
código Python, até a análise energética e a reflexão crítica fundamentada em normas e conceitos
reais de sustentabilidade. O resultado é um projeto que não apenas simula uma verificação técnica
de pré-decolagem, mas também discute as implicações éticas e sociais de sistemas de decisão
automatizada — validado nos dois cenários testados (sucesso e falha), nos quais o algoritmo
respondeu corretamente em todas as situações propostas.

## Prints da execução

Execução do Cenário 1 (sucesso)
<img width="442" height="147" alt="Screenshot 2026-09-12 083541" src="https://github.com/user-attachments/assets/a90b0c80-7dc2-45cd-bc78-4ebe2ef9c8ca" />

Execução do Cenário 2 (falha)
<img width="541" height="237" alt="Screenshot 2026-09-12 083549" src="https://github.com/user-attachments/assets/42a9dea5-4878-4ef0-8e5b-500340836d01" />

Resultado da análise energética
<img width="388" height="100" alt="Screenshot 2026-09-12 083714" src="https://github.com/user-attachments/assets/52b7a41d-a078-45e7-9ac8-4f57ea75ea36" />


## Instruções de execução do código

Para executar este projeto, abra o arquivo `Relatorio_Operacional_De_PreDecolagem.ipynb` no Google
Colab ou Jupyter Notebook e execute todas as células em ordem (**Ambiente de execução → Executar
tudo**, ou `Ctrl+F9`). O notebook não depende de bibliotecas externas além das padrão do Python,
portanto nenhuma instalação adicional é necessária. Os resultados de cada verificação (Cenário 1 e
Cenário 2) e o cálculo de autonomia energética serão impressos automaticamente após a execução.

---

**Autora:** Maria Luiza Costa Araujo
**Curso:** Ciências da Computação — FIAP
**Data:** Setembro, 2026
