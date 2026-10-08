# Processo V2 de inteligência de candidaturas

## Objetivo

Este processo transforma a busca em um funil controlado: encontrar vagas ativas, separar as que são realmente elegíveis, personalizar somente o que tem chance real e acompanhar cada etapa até o resultado. A meta não é enviar o maior número possível de currículos; é aumentar entrevistas e propostas sem inventar informação, perder prazos ou expor dados desnecessários.

O processo usa plataformas como fonte de descoberta e de ganho de velocidade, mas mantém a decisão humana sobre elegibilidade, texto, testes, dados pessoais e envio final.

O comparativo que motivou esta versão está em [LAUDO AIApply](LAUDO_AIAPPLY_2026-10-07.md). A busca centralizada, a biblioteca de respostas, o rastreador e a adaptação inicial de documentos são ideias aproveitadas. Autoenvio, conexão ampla de dados e assistência durante avaliações não são.

## Princípios que não mudam

1. **Fatos antes de palavras-chave.** Currículo, apresentação e respostas só podem afirmar experiência, formação, idioma, disponibilidade e tecnologias comprováveis.
2. **Bolsa ou salário não é o pacote inteiro.** Registrar separadamente remuneração-base, VR/VA, transporte, auxílio remoto e benefícios não mensuráveis. Nunca chamar benefício de salário.
3. **Elegibilidade vem antes da adaptação.** Formação exigida, previsão real de conclusão, local, jornada, senioridade e prazo são verificados antes de escrever um texto personalizado.
4. **Uma candidatura, uma decisão registrada.** Cada envio tem link oficial, data de verificação, versão de currículo, motivo de aderência e próximo passo.
5. **Avaliações pessoais continuam pessoais.** Teste técnico, teste cognitivo, mapeamento comportamental, entrevista, áudio, vídeo, câmera, microfone, CAPTCHA e declarações pessoais não são automatizados.
6. **Revisão antes de envio.** Nenhum modo de autoenvio, preenchimento autônomo ou resposta de IA decide uma candidatura sem checagem humana.
7. **Privacidade por padrão.** CPF, RG, endereço, senhas, tokens, dados bancários, links autenticados e conteúdo de e-mail ficam fora do repositório público.

## Funil operacional

```text
Descoberta → Validação → Elegibilidade → Priorização → Personalização
→ Revisão → Envio confirmado → Monitoramento → Resultado → Aprendizado
```

### 1. Descoberta

Pesquisar diariamente fontes oficiais de empresas, Gupy, Greenhouse, Lever, Workday, LinkedIn, Indeed, Catho, InfoJobs e alertas de carreira. Para bancos e fintechs, pesquisar também adquirência, pagamentos, crédito, antifraude, dados de risco, seguros, investimentos, infraestrutura financeira e tecnologia regulatória.

Toda vaga nova entra como `Encontrada`, nunca como candidatura, até ser validada.

### 2. Validação da vaga

Antes de investir tempo, registrar:

| Campo | Regra |
| --- | --- |
| Link | Preferir a página oficial da empresa ou da recrutadora contratada. |
| Estado | Confirmar que a página carrega e aceitar inscrições na data da checagem. |
| Duplicidade | Comparar empresa, cargo, local, código e descrição com a base. |
| Data e prazo | Registrar data de publicação, encerramento e última checagem. |
| Remuneração | Separar divulgado, estimado e não divulgado. |
| Modelo | Presencial, híbrido, remoto; cidade e frequência presencial. |
| Tipo | Estágio, CLT, PJ, trainee ou temporário. |

Uma vaga fechada, duplicada, sem empresa identificável ou com descrição incompatível sai da fila antes da personalização.

### 3. Checagem de elegibilidade

Usar quatro portas, nesta ordem:

1. **Formação e duração:** para estágio, conferir matrícula ativa, cursos aceitos, previsão real de conclusão e tempo mínimo restante. Não alterar a previsão acadêmica para caber em programa.
2. **Escopo e senioridade:** preferir desenvolvimento, dados, automação, IA aplicada, integrações, produto técnico e operações financeiras orientadas por tecnologia. Excluir venda, atendimento comercial, suporte ao cliente, QA como foco principal, liderança e vagas sênior.
3. **Condições de trabalho:** São Paulo/Grande São Paulo, remoto ou híbrido; jornada compatível; mudança somente quando a remuneração justifica.
4. **Remuneração:** referência de R$ 3.000 mensais para emprego. Para estágio, classificar a bolsa e o pacote com transparência, sem somar benefícios à bolsa.

Para programas de estágio, uma vaga pode ter ótima remuneração e ainda assim ficar como `Não elegível agora` se exigir formatura em 2028/2029 ou período mínimo que a data acadêmica real não atende. Isso evita candidaturas descartadas por requisito objetivo.

## Pontuação de prioridade

Depois de passar pelas portas de elegibilidade, cada vaga recebe uma pontuação de 0 a 100. A nota organiza o trabalho; ela não substitui a leitura da descrição.

| Dimensão | Pontos | Como avaliar |
| --- | ---: | --- |
| Aderência técnica real | 0–30 | Stack, responsabilidades, projetos demonstráveis e possibilidade de executar o trabalho. |
| Elegibilidade objetiva | 0–25 | Formação, prazo, experiência exigida, local e jornada. |
| Remuneração e pacote | 0–15 | Valor-base divulgado, benefícios mensuráveis e relação com o piso definido. |
| Carreira e aprendizagem | 0–15 | Exposição a engenharia, dados, produtos financeiros, mentoria e possibilidade de efetivação. |
| Urgência e fonte | 0–15 | Prazo, anúncio recente, fonte oficial e ausência de duplicidade. |

Classificação:

| Faixa | Fila | Ação |
| --- | --- | --- |
| 85–100 | P0 | Revisar e enviar primeiro, antes do prazo. |
| 70–84 | P1 | Personalizar e enviar após revisão. |
| 55–69 | P2 | Manter como candidatura válida ou stretch explícito. |
| Abaixo de 55 | P3 | Monitorar ou encerrar, sem gastar esforço de personalização. |
| Requisito eliminatório não atendido | Bloqueada | Registrar o motivo e não enviar. |

## Pacote de candidatura personalizado

Para cada P0/P1, preparar somente o necessário:

1. Selecionar a versão correta do currículo mestre: full stack, backend/fintech ou integrações.
2. Atualizar título, resumo e palavras-chave apenas com termos verdadeiros presentes na vaga.
3. Escrever apresentação de até 1.500 caracteres que conecte Performance Lab, NOW PRO, projetos próprios e repertório de negócio B2B ao problema da vaga, sem atribuir resultados não comprovados.
4. Destacar até três habilidades que aparecem tanto no currículo quanto na descrição da vaga.
5. Preencher respostas reutilizáveis a partir de uma biblioteca factual aprovada: formação, disponibilidade, modalidade, pretensão, idiomas, experiência CNPJ e links públicos.
6. Fazer uma última leitura comparando cada afirmação com o currículo e o GitHub.

O pacote fica associado a uma `versão de currículo`, `texto de apresentação`, `habilidades destacadas` e `respostas específicas`. Isso evita respostas genéricas e permite aprender qual mensagem gera retorno.

## Monitoramento de processos

Estados padronizados:

```text
Encontrada → Validada → Elegível → Rascunho → Revisão → Enviada
→ Confirmação recebida → Próxima etapa → Entrevista → Oferta
→ Recusada / Encerrada / Pausada / Não elegível
```

Pendência só existe quando há uma ação concreta. Cada pendência precisa de `motivo`, `dono`, `prazo`, `link oficial` quando público e `próxima ação`. Não confundir “aguardar retorno” com pendência de execução.

E-mails são monitorados por gatilhos: confirmação, finalizar candidatura, teste, prazo, entrevista, documento, atualização de status e proposta. Ao surgir uma mensagem, cruzar empresa + vaga + código antes de abrir uma nova candidatura para evitar duplicidade.

## Métricas que importam

O processo mede qualidade, não apenas quantidade:

| Métrica | Pergunta respondida |
| --- | --- |
| Vagas validadas por fonte | Onde aparecem vagas reais e aderentes? |
| Taxa de elegibilidade | Quanto do encontrado atende formação, local e remuneração? |
| Tempo até candidatura revisada | Onde existe gargalo operacional? |
| Retorno por versão de currículo | Qual narrativa gera mais contato? |
| Convite para próxima etapa por fonte e área | Que canal e cargo convertem melhor? |
| Pendências vencidas | Que prazos exigem rotina mais rápida? |
| Vagas com salário/pacote confirmado | Onde o esforço tem melhor retorno financeiro? |

Uma fonte que gera muitas vagas, mas poucas elegíveis ou muitos formulários ruins, perde prioridade. Uma fonte menor que gera entrevistas recebe mais atenção.

## Diferença em relação a ferramentas de autoaplicação

| Automação de volume | Processo V2 |
| --- | --- |
| Confia em match automático e palavras-chave. | Valida requisito, remuneração, formação e etapa real. |
| Pode usar currículo/carta genérica em escala. | Mantém versões factuais e personalização curta por vaga. |
| Mede candidaturas enviadas. | Mede elegibilidade, conversão, prazo e retorno. |
| Pode repetir vagas ou enviar para cargo incompatível. | Deduplica e registra motivo de escolha ou descarte. |
| Centraliza dados em ferramenta externa. | Mantém fonte oficial na planilha privada e publicação sanitizada no Git. |
| Pode automatizar etapas inadequadas. | Separa claramente o que exige participação pessoal. |

## Recursos que incorporamos e como ficam melhores no fluxo

| Recurso observado em plataformas de candidatura | Implementação no Processo V2 | Controle adicional |
| --- | --- | --- |
| Busca e pontuação de compatibilidade | Fila por área, local, senioridade, remuneração e fonte oficial. | A nota usa requisitos lidos, não apenas título ou palavras-chave. |
| Biblioteca de respostas | Respostas factuais reutilizáveis para cadastro, disponibilidade, formação e histórico profissional. | Cada resposta tem fonte no currículo e revisão antes de ser usada. |
| Currículo e carta por vaga | Três versões factuais do currículo e apresentação curta adaptada ao desafio descrito. | Não altera anos, diploma, idiomas ou tecnologias para melhorar score ATS. |
| Rastreador de candidaturas | Base privada com status, prazo, versão de currículo, próximo passo e resultado. | E-mail e vaga são cruzados por empresa, cargo e código antes de mudar o status. |
| Alertas e follow-up | Triagem diária de prazos, confirmações, pedidos de completar cadastro e mudanças de fase. | "Aguardar retorno" não vira pendência sem data ou ação concreta. |
| Auto Apply e assistência de entrevista | Não entram no fluxo. | Evita repetição, dados imprecisos, envio sem revisão e interferência em avaliações pessoais. |

## Rotina de execução

- **Todo dia útil:** verificar alertas, e-mails de prazo e vagas P0; atualizar o status antes de procurar novas vagas.
- **Duas vezes por semana:** varrer carreiras de bancos, fintechs, pagamentos, seguros, dados de crédito, adquirência e empresas de produto financeiro.
- **Semanalmente:** revisar fontes que geraram resposta, salários/pacotes observados e pendências vencidas; ajustar palavras-chave e prioridades.
- **Após cada candidatura ou resposta:** atualizar a planilha privada e, quando material, o diário público sanitizado.

## Próxima evolução prática

1. Criar uma lista privada de respostas factuais reutilizáveis, com data de revisão e fonte de cada afirmação.
2. Acrescentar à planilha as colunas `bolsa/salário-base`, `VR/VA`, `auxílios mensuráveis`, `pacote mensurável`, `formatura exigida`, `elegibilidade acadêmica` e `pontuação P0–P3`.
3. Manter uma fila exclusiva de bancos, fintechs, crédito, pagamentos, antifraude, dados e produto financeiro.
4. Manter o modo de operação em revisão humana: automação pode pesquisar, resumir e preparar; o candidato confirma informações pessoais, faz avaliações e decide o envio final.
