## 📄 Visão Geral do Conjunto de Dados
Este conjunto de dados contém informações sobre **empresas sancionadas com base na Lei Anticorrupção (Lei Federal nº 12.846/2013)** no âmbito do Estado de Minas Gerais. Os registros documentam processos administrativos conduzidos pela Controladoria-Geral do Estado de Minas Gerais (CGE/MG), em parceria com a Advocacia-Geral do Estado (AGE/MG) e com apoio do Ministério Público de Minas Gerais (MPMG).

## 🏛️ Contexto Legal
A Lei Anticorrupção (Lei nº 12.846/2013) estabelece a responsabilidade objetiva de pessoas jurídicas por atos lesivos contra a administração pública, prevendo sanções administrativas e civis para empresas envolvidas em:
- Atos de corrupção
- Fraudes em licitações e contratos
- Outras irregularidades contra a administração pública

## 📊 Estrutura dos Dados

### Arquivo Principal
- **Formato**: CSV (valores separados por vírgula)
- **Codificação**: UTF-8
- **Delimitador**: Ponto e vírgula (;) ou vírgula (,)
- **Cabeçalho**: Incluído

### Descrição dos Campos

| Campo | Tipo | Descrição | Exemplo |
|-------|------|-----------|---------|
| `sei` | String | Número do Processo no Sistema Eletrônico de Informações | "00001.000000/2024-00" |
| `numero` | String | Número identificador do processo administrativo | "APAC 001/2024" |
| `ano` | Inteiro | Ano de instauração do processo | 2024 |
| `portaria` | String | Número da portaria de instauração | "Portaria CGE nº 100/2024" |
| `data_publicacao` | Date | Data de publicação no diário oficial | "2024-03-15" |
| `orgao_instaurador` | String | Órgão responsável por instaurar o processo | "Controladoria-Geral do Estado (CGE/MG)" |
| `orgao_lesado` | String | Órgão ou entidade prejudicada pela conduta | "Secretaria de Estado de Saúde" |
| `empresa_processada` | String | Razão social da empresa sancionada | "Construtora XYZ Ltda." |
| `tipo_societario` | String | Tipo societário da empresa | "Sociedade Limitada", "S/A" |
| `cnpj` | String | CNPJ da empresa (com ou sem formatação) | "00.000.000/0001-00" |
| `contua` | String | ContUA (Controle de Unidades Administrativas) - identificador interno | "CONTA20240001" |
| `data_decisao` | Date | Data da decisão final do processo | "2024-06-20" |
| `decisao` | String | Decisão aplicada (tipo de sanção) | "Aplicação de multa", "Acordo de Leniência" |
| `fase` | String | Fase atual do processo | "Encerrado", "Em recurso", "Cumprimento de acordo" |
| `valor_multa` | Decimal | Valor da multa aplicada (se houver) | 1500000.00 |

