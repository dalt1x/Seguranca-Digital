# Segurança Digital | Dashboard e Pesquisa — UNIG

Dashboard e materiais da pesquisa **Segurança Digital entre Estudantes Universitários**, desenvolvida no **Tema Integrador VII, Ciência da Computação, Universidade Iguaçu (UNIG), 2026**.

**Autores:** Dalton, Kaua e Caroline.

## Acessar o dashboard

O site é o arquivo [`index.html`](index.html). Após habilitar o GitHub Pages, o endereço público seguirá o formato `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

Ele contém quatro indicadores e cinco gráficos interativos sobre hábitos declarados de segurança digital. Funciona sem servidor, sem banco externo e sem bibliotecas JavaScript adicionais.

**Questionário:** https://forms.gle/LN3Hjy1jku2CddK28

## Visão dos resultados

| Indicador | Resultado |
|---|---:|
| Participantes com consentimento | 37 |
| Reutilizam senhas às vezes ou frequentemente | 97,3% |
| Nunca verificam remetentes e links | 67,6% |
| Não conhecem autenticação em duas etapas | 45,9% |
| Atribuíram nota 1 ou 2 ao conhecimento sobre LGPD | 75,7% |
| Não souberam associar segurança digital a ODS | 66,7% (n=36) |

**Atenção:** pesquisa exploratória de conveniência. Só 7 respondentes assinalaram vínculo estudantil, 1 marcou docente e 29 marcaram “Outro”. Os percentuais descrevem o grupo pesquisado, não toda a comunidade universitária.

## Estrutura do repositório

```text
index.html                                Site para GitHub Pages (raiz)
README.md                                 Esta apresentação
.nojekyll                                 Configuração de publicação estática
docs/
  Artigo_Seguranca_Digital.pdf            Artigo enviado
  Infografico.pdf                         Infográfico enviado
  Plano_de_Pesquisa.md                    Plano estruturado
  Relatorio_de_Devolutiva.pdf             Relatório educativo de 5 páginas
  Consentimento_e_Etica.md                Consentimento descrito no instrumento
  Portfolio_versao_em_desenvolvimento.pdf Documento original, ainda incompleto
  evidencias/README.md                    Evidências reais ainda pendentes
dados/
  brutos/README.md                        Por que a base individual é restrita
  tratados/dados_agregados.csv            Resultados dos 5 gráficos
  tratados/contagens_por_pergunta.csv     Resultados de todas as perguntas
  dicionario_variaveis.csv                Definição das variáveis
  procedimentos_limpeza.md                Conferência dos dados
analise/
  README.md                               Análise e instruções
  METODOLOGIA_E_DADOS.md                  Indicadores, fórmulas e limites
  verificar_dados.py                      Conferência matemática dos CSVs
  gerar_figuras.py                        Gráficos reproduzíveis
  requirements.txt                        Dependência opcional
figuras/
  01_autenticacao_2fa.png                 Gráfico 1
  02_reutilizacao_senhas.png              Gráfico 2
  03_verificacao_links.png                Gráfico 3
  04_conhecimento_lgpd.png                Gráfico 4
  05_associacao_ods.png                   Gráfico 5
instrumento/
  Questionario.pdf                        Perguntas e consentimento
```

## Fontes e tratamento dos dados

A equipe forneceu uma planilha com **37 respostas consentidas**. O cálculo usa porcentagens arredondadas a uma casa decimal, com n=36 somente na questão de ODS. A data de referência é **08/11/2026**. Os dados são um recorte estático, não um painel ao vivo.

A planilha com **linhas individuais e carimbos de hora não está publicada** neste repositório. O material público contém somente totais agregados. Consulte [procedimentos de limpeza](dados/procedimentos_limpeza.md), [dicionário](dados/dicionario_variaveis.csv) e [metodologia](analise/METODOLOGIA_E_DADOS.md).

## Documentação acadêmica

- [Artigo científico](docs/Artigo_Seguranca_Digital.pdf)
- [Questionário transcrito](instrumento/Questionario.pdf)
- [Infográfico educativo](docs/Infografico.pdf)
- [Plano de pesquisa](docs/Plano_de_Pesquisa.md)
- [Relatório de devolutiva (5 páginas)](docs/Relatorio_de_Devolutiva.pdf)
- [Gráficos para apresentação](figuras/)
- [Situação das evidências extensionistas](docs/evidencias/README.md)

## Como publicar no GitHub Pages

1. Crie um novo repositório **público** (por exemplo, `dashboard-seguranca-digital`).
2. Descompacte o ZIP do projeto e envie **todos os arquivos e pastas para a raiz** do repositório, sem criar uma pasta extra por cima.
3. No repositório, acesse **Settings → Pages → Build and deployment**.
4. Em **Source**, escolha `Deploy from a branch`.
5. Selecione a branch `main`, pasta `/(root)` e salve.
6. Abra o link exibido em **Settings → Pages** e teste os gráficos, links, CSV e visualização em celular.

Não é necessário usar Docker, Node.js ou publicar um banco de dados para executar este site estático.

## Pendências para a entrega acadêmica definitiva

- Confirmar e documentar coleta presencial/evento, se exigida; não há prova disso nos materiais recebidos.
- Registrar divulgação, testes reais e apresentação à comunidade; incluir pelo menos 4 imagens reais no portfólio.
- Obter feedback autorizado de participantes e documentar resultados sem identificação.
- Completar o portfólio e verificar com o professor diagramas UML, testes e requisitos de defesa.
- Atualizar no portfólio o link do GitHub Pages após a publicação.

**Importante:** o repositório foi preparado para publicação, mas os documentos não comprovam atividades que ainda não foram realizadas.
