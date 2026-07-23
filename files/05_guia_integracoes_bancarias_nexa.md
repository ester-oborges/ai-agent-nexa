# Guia de Integrações Bancárias e Open Finance — Nexa Finanças

## O que é a conciliação automática

A Nexa Finanças utiliza o padrão Open Finance regulamentado pelo Banco Central do Brasil para conectar, com o consentimento do cliente, as contas bancárias da empresa à plataforma. Isso permite que os extratos sejam importados automaticamente e comparados com os lançamentos financeiros já registrados, reduzindo o trabalho manual de conciliação.

## Bancos e fintechs suportados

| Instituição | Tipo de conexão | Disponível desde |
|---|---|---|
| Banco do Brasil | Open Finance | 2023 |
| Itaú | Open Finance | 2023 |
| Bradesco | Open Finance | 2023 |
| Santander | Open Finance | 2024 |
| Caixa Econômica Federal | Open Finance | 2024 |
| Nubank | Open Finance | Q3 2026 |
| Banco Inter | Open Finance | Q3 2026 |
| Sicoob | Open Finance | Q3 2026 |
| C6 Bank | Importação de OFX | Em avaliação |

## Como conectar uma conta bancária

1. Acesse Financeiro > Contas Bancárias > Nova Conexão.
2. Selecione a instituição financeira desejada.
3. Você será redirecionado ao ambiente autenticado do próprio banco para autorizar o compartilhamento de dados, conforme as regras do Open Finance.
4. Após a autorização, os lançamentos dos últimos 90 dias são importados automaticamente, e novas movimentações passam a ser sincronizadas a cada 4 horas.

## Segurança da integração

A Nexa Finanças nunca armazena login ou senha bancária dos clientes. A autorização é feita diretamente no ambiente do banco, seguindo o protocolo OAuth 2.0 definido pelo Open Finance Brasil, e pode ser revogada pelo cliente a qualquer momento, tanto pela Nexa Finanças quanto diretamente no aplicativo do banco.

## Conciliação e regras automáticas

O sistema sugere automaticamente o pareamento entre lançamentos importados e lançamentos já registrados, com base em valor, data e histórico de descrições semelhantes. É possível criar regras de conciliação automática por palavra-chave (por exemplo, categorizar automaticamente todo lançamento com a palavra "aluguel" como despesa fixa de ocupação).

## Limitações conhecidas

A conciliação automática via Open Finance está disponível apenas para contas correntes e contas digitais em nome da pessoa jurídica contratante. Contas de investimento, cartões de crédito de bandeiras internacionais emitidos fora do Brasil e contas em nome de pessoa física não são suportadas no momento.
