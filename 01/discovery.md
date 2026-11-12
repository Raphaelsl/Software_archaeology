# 1. O que é o Software?

## 1.1. Definição Geral
O **Seven23** é um aplicativo de gerenciamento de finanças pessoais de código aberto, projetado para registrar despesas e receitas. 

* **Problema que o software resolve:** A falta de privacidade em aplicativos financeiros tradicionais, que frequentemente utilizam ou vendem dados bancários dos usuários. O Seven23 resolve isso implementando criptografia de ponta a ponta (E2EE), garantindo que apenas o usuário tenha acesso aos dados reais de suas transações.
  * *Evidência:* Descrito no parágrafo introdutório do `README.md` oficial do repositório:
  * <img width="864" height="388" alt="image" src="https://github.com/user-attachments/assets/c2e00cde-dba8-4bc3-8f60-d25e535d726a" />

* **Público-alvo:** Indivíduos preocupados com a privacidade de seus dados digitais, defensores do código aberto e pessoas que desejam controle estrito sobre seu orçamento pessoal sem rastreamento de terceiros.
* **Principais Usuários:** Trabalhadores independentes, estudantes universitários gerenciando orçamentos limitados e entusiastas de tecnologia que preferem hospedar seus próprios serviços (self-hosting).
* **Principais Funcionalidades:**
  * Registro de transações (despesas e receitas).
  * Categorização customizável de gastos.
  * Sincronização multi-dispositivo com criptografia de ponta a ponta.
  * Suporte a múltiplas moedas.
  * *Evidência:* [procurar alguma lista de features na doc]

## 1.2. Aspectos Técnicos
* **Tecnologias utilizadas:** O backend do projeto é construído em Python utilizando o *framework* Django e o Django REST Framework para fornecer uma API robusta.
  * *Evidência:* A stack tecnológica é comprovada pela presença do arquivo `requirements.txt` <img width="1919" height="953" alt="image" src="https://github.com/user-attachments/assets/a465e521-779f-457d-8dee-ed9407c52383" />
 que lista o `Django` como dependência principal.
* **Licença:**
*  <img width="921" height="500" alt="image" src="https://github.com/user-attachments/assets/c27e7c65-2fed-49b2-886c-04d595cdcb22" />

* **Versão/Release analisada:** Versão [2.2.1] lançada em [04/08/2026].
  *<img width="1220" height="465" alt="image" src="https://github.com/user-attachments/assets/13986e81-ddb1-40e1-a68f-1438c6daebb6" />


---

## 1.3. Personas e Jobs to Be Done (JTBD)

**Carlos**, 45 anos.
* Perfil: Trabalhador que prefere anotar manualmente cada gasto para manter total consciência e domínio sobre o orçamento.
* Comportamento:
Não confia em aplicativos bancários com sincronização automática, pois costumam falhar na categorização e expõem dados sensíveis.
Prefere o ato consciente de digitar cada compra para evitar gastos por impulso.
* Uso no Seven23: Utiliza a plataforma como um "caderninho digital" privado, seguro e organizado por categorias simples, sem distrações ou propagandas.
* **Jobs to Be Done:**
  *Quando* eu realizo uma compra no meu dia a dia, *quero* registrar esse gasto manualmente em um ambiente privado e sem sincronização bancária automática, *para que* eu mantenha total consciência sobre meus gastos e evite que meus dados sejam expostos.

**Mariana**, 22 anos.
* Perfil: Pessoa que lida rotineiramente com diferentes moedas (seja em viagens, compras internacionais ou trabalhos freelancer) e precisa de clareza em seus saldos.
* Comportamento:
Sofre com conversores automáticos imprecisos em ferramentas tradicionais.
Precisa registrar transações estrangeiras aplicando a taxa de câmbio real e exata do dia da compra.
* Uso no Seven23: Aproveita o suporte a múltiplas moedas para gerenciar fluxos financeiros complexos e consolidar diferentes saldos em um único painel seguro.
* **Jobs to Be Done:**
  *Quando* eu realizo transações em moedas estrangeiras, *quero* registrar o valor na moeda original aplicando a taxa de câmbio exata do dia, *para que* eu tenha um painel consolidado e preciso do meu saldo real, sem depender de conversores automáticos falhos.
