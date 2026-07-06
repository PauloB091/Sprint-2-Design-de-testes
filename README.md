# Sprint-2-Design-de-testes
# Design de Testes - Urban Routes

## Descrição do Projeto

Este projeto consiste na elaboração de um documento de **Design de Testes** para a aplicação **Urban Routes**, desenvolvido como parte das atividades práticas de um bootcamp de Quality Assurance (QA). O foco do trabalho é a aplicação de técnicas sistemáticas de modelagem de testes funcionais, garantindo cobertura abrangente e rastreável das funcionalidades da aplicação.

O entregável principal é um conjunto de **Casos de Teste Detalhados**, construídos a partir da análise dos requisitos e da aplicação de técnicas clássicas de design de testes.

---

## Sobre a Aplicação

O **Urban Routes** é uma aplicação voltada ao planejamento e navegação de rotas urbanas. Em linhas gerais, a aplicação permite que o usuário:

- Informe pontos de origem e destino;
- Visualize rotas sugeridas entre os pontos informados;
- Selecione o modo de deslocamento de taxi;
- Visualize estimativas de tempo e distância para cada rota;

A natureza da aplicação envolve diversas regras de negócio e entradas com limites bem definidos, o que a torna um cenário adequado para a aplicação de técnicas estruturadas de design de testes.

---

## Objetivos do Design de Testes

Os objetivos deste projeto são:

1. **Aplicar técnicas sistemáticas de design de testes** para derivar casos de teste a partir dos requisitos funcionais da aplicação.
2. **Garantir cobertura abrangente** das funcionalidades do Urban Routes, evitando redundâncias e identificando cenários relevantes.
3. **Documentar casos de teste de forma detalhada**, com passos claros, dados de entrada, resultados esperados e priorização.
4. **Estabelecer rastreabilidade** entre requisitos, técnicas aplicadas e casos de teste gerados.
5. **Praticar o raciocínio analítico** necessário para a atividade de modelagem de testes em um contexto realista.

---

## Técnicas Aplicadas

Para a modelagem dos testes, foram aplicadas três técnicas clássicas de design de testes funcionais:

### 1. Particionamento de Equivalência

Consiste na divisão do domínio de entrada em classes de equivalência, nas quais se pressupõe que o comportamento da aplicação seja semelhante. A seleção de um representante de cada classe é suficiente para validar o comportamento esperado, reduzindo a quantidade de casos de teste sem perda significativa de cobertura.

**Exemplo de aplicação no Urban Routes:** definição de classes válidas e inválidas para o campo de endereço de destino (endereço válido, endereço inexistente, campo vazio, texto com caracteres especiais).

### 2. Análise de Valor Limite

Foca nos valores nas fronteiras das classes de equivalência, onde a probabilidade de ocorrência de defeitos costuma ser maior. Sao testados os valores exatamente no limite, imediatamente abaixo e imediatamente acima.

**Exemplo de aplicação no Urban Routes:** validação do número máximo e mínimo de paradas intermediárias permitidas em uma rota, considerando os valores limite e seus adjacentes.

### 3. Tabela de Decisão

Utilizada quando o comportamento da aplicação depende da combinação de múltiplas condições de entrada. As condições e suas combinações são organizadas em uma tabela, da qual são derivados os casos de teste correspondentes a cada regra de negócio.

**Exemplo de aplicação no Urban Routes:** combinação entre modo de deslocamento selecionado, disponibilidade da rota e presença de paradas intermediárias, resultando em diferentes comportamentos esperados da aplicação.
