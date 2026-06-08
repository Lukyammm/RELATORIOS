# RELATORIOS

Web App em Google Apps Script para geração do Relatório Analítico COSEP com dados em Google Sheets.

## Estrutura da planilha

A planilha do relatório deve conter, no mínimo:

- `BASE_DADOS(NÃOEDITAR)`: base principal CRP com cabeçalhos de `A` até `AQ`.
- `CRO`: base futura/alternativa para CRO, quando disponível.
- `COSEP_REL_CONFIG`: aba criada automaticamente pelo app para guardar configurações editáveis do relatório.
- `COSEP_REL_CONFIG_LOG`: aba criada automaticamente para histórico de alterações administrativas.

## Aba de configuração

A aba `COSEP_REL_CONFIG` armazena:

- meta institucional;
- ID da planilha do relatório;
- nome da aba da base CRP;
- termos de classificação (`Conforme`, `Não conforme`, `Não se aplica`);
- nomes editáveis dos indicadores da CRP;
- dados da última atualização.

A edição recomendada é pela tela **Administração do relatório**, mas a aba existe na própria planilha para auditoria, manutenção e portabilidade.
