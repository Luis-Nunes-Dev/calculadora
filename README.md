# 🧮 Calculadora de Precificação

Aplicação web desenvolvida para facilitar a formação de preços de venda, permitindo calcular os custos de produção, despesas fixas, mão de obra e margens de lucro de um produto.

O objetivo é ajudar pequenos empreendedores e produtores a entender melhor seus custos e definir preços de venda de forma mais organizada.

## ✨ Funcionalidades

- **Cadastro de produtos:** identificação do produto que será precificado.
- **Cálculo de insumos:** adição de ingredientes, materiais e embalagens, considerando valores e quantidades utilizadas.
- **Cálculo de mão de obra:** estimativa do custo de trabalho com base no valor da hora e no tempo de produção.
- **Assistente de mão de obra:** cálculo do valor da hora com base no salário mensal desejado e nas horas produtivas.
- **Despesas fixas:** cadastro de custos mensais, como aluguel, energia e internet.
- **Rateio de despesas:** aplicação de um percentual das despesas fixas no cálculo do preço.
- **Impostos, taxas e comissões:** inclusão de percentuais adicionais na formação do preço.
- **Custo por unidade:** cálculo do custo unitário conforme o rendimento do lote.
- **Simulação de preços:** comparação de diferentes margens de lucro.
- **Lucro estimado:** visualização do lucro em reais e em percentual.
- **Produtos salvos:** armazenamento, consulta, edição e exclusão de produtos salvos no navegador.
- **Atualização automática:** recálculo dos valores conforme os dados são alterados.
- **Interface responsiva:** estrutura preparada para diferentes tamanhos de tela.

## 🛠️ Tecnologias utilizadas

- **HTML5:** estrutura da aplicação.
- **CSS3:** estilização e organização visual da interface.
- **JavaScript:** cálculos, validações, atualização dinâmica dos elementos e gerenciamento dos produtos.
- **LocalStorage:** armazenamento local dos produtos salvos no navegador.
- **Google Fonts:** fontes Plus Jakarta Sans e JetBrains Mono.

## 📋 Como funciona

A calculadora é organizada em três etapas principais.

### 1. Produto e insumos

O usuário informa o nome do produto, os custos dos materiais utilizados, as quantidades compradas e consumidas, o rendimento do lote e os dados de mão de obra.

O custo de cada insumo é calculado proporcionalmente à quantidade utilizada:

`Custo do insumo = (Valor pago ÷ Quantidade comprada) × Quantidade utilizada`

O custo total dos insumos é dividido pelo rendimento para obter o custo unitário dos materiais.

### 2. Despesas fixas

Permite cadastrar despesas mensais e definir um percentual de rateio. Também é possível informar os percentuais de impostos, taxas de cartão e comissões aplicáveis.

### 3. Resultado

A aplicação apresenta:

- **Preço de custo:** custo unitário dos insumos, mão de obra e valor rateado das despesas fixas.
- **Preço mínimo de venda:** preço de custo ajustado pelos percentuais adicionais informados.
- **Preço de venda por unidade:** sugestão de preço unitário com a margem escolhida.
- **Cenários de margem:** duas simulações de preço ideal e lucro para facilitar a comparação.

Os resultados são atualizados automaticamente conforme os valores informados.

## 🚀 Como executar o projeto

Não é necessário instalar dependências ou configurar um servidor backend para utilizar a versão atual.

1. Faça o download ou clone este repositório.
2. Abra a pasta do projeto.
3. Abra o arquivo `index.html` em um navegador.
4. Preencha os campos e comece a calcular os preços.

Para facilitar o desenvolvimento, recomenda-se utilizar o [Visual Studio Code](https://code.visualstudio.com/) com a extensão **Live Server**.

## 📁 Estrutura do projeto

```text
calculadora-precificacao/
├── index.html    # Estrutura HTML e lógica JavaScript
├── style.css     # Estilos e layout da aplicação
└── README.md     # Documentação do projeto
```

## 💾 Armazenamento dos dados

Os produtos são salvos no `LocalStorage` do navegador, utilizando a chave `produtosSalvos`.

Isso significa que:

- Os produtos ficam armazenados localmente no navegador utilizado.
- Os dados não são sincronizados automaticamente entre dispositivos ou navegadores.
- A limpeza dos dados do navegador pode remover os produtos salvos.

A aplicação não utiliza um banco de dados remoto na versão atual.

## 🎯 Objetivo do projeto

Este projeto foi desenvolvido para praticar e aplicar conceitos de desenvolvimento web, manipulação do DOM, funções JavaScript, cálculos financeiros, validação de entradas e armazenamento local de dados.

## 👨‍💻 Autor

**Luis Nunes**

- GitHub: [@luisnunes](https://github.com/luisnunes)

---

Desenvolvido com HTML, CSS e JavaScript.
