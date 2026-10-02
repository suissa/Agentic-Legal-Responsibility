> ***Qual a sua opinião sobre E quem deve ser a responsabilidade legal pelas ações dos agentes de IA na internet e se puder cite/link os artigos  conceitos que você usou***


A responsabilidade legal por ações de agentes de IA **não deve recair sobre o agente em si**. Deve ser atribuída às pessoas e organizações que o projetam, colocam em circulação, configuram, controlam e se beneficiam dele — com divisão conforme o grau de controle, previsibilidade do dano e capacidade de prevenção.

Minha posição é: para o lesado, deve haver sempre um responsável humano ou empresarial identificável; internamente, os envolvidos podem discutir direito de regresso segundo sua contribuição para a falha. Isso evita que a “autonomia” do agente vire uma lacuna de responsabilização.

## Ponto de partida

Um agente de IA pode executar tarefas, usar ferramentas, navegar, contratar serviços, publicar conteúdo ou iniciar transações. Mas ele não tem patrimônio próprio, capacidade moral, intenção jurídica comprovável, cidadania nem condições reais de cumprir uma condenação.

Chamá-lo de “agente” é útil tecnicamente, mas não deve induzir uma ficção: ele não é um **sujeito jurídico autônomo** como uma pessoa física ou empresa. A proposta jurídica mais robusta é tratar sua conduta como atribuível a uma cadeia humana/organizacional, de maneira semelhante ao que o Direito já faz com funcionários, representantes, softwares automatizados e atividades empresariais de risco.

A literatura recente sobre IA sustenta justamente que não devemos deixar a ausência de intenção humana da máquina eliminar a responsabilização: podem-se usar padrões objetivos de conduta e risco previsível para atribuir responsabilidade a quem criou, disponibilizou ou operou o sistema.[1]

## Quem responde — matriz prática

Eu adotaria uma responsabilidade em camadas, não uma regra simplista como “sempre o desenvolvedor” ou “sempre o usuário”.

| Ator | Deve responder quando | Tipo de dever |
|---|---|---|
| Usuário/principal | Instrui o agente a praticar ato ilícito, aprova uma ação relevante ou escolhe delegação incompatível com o risco | Responsabilidade primária por comando, finalidade e autorização |
| Operador/deployer | Configura, integra, fornece credenciais, define limites, ativa autonomia e deixa de supervisionar | Responsabilidade primária perante terceiros em uso profissional ou comercial |
| Empresa que oferece o agente | Coloca produto/serviço defeituoso no mercado, promete segurança que não entrega, falha em mitigação, logs, controle de acesso ou correção | Responsabilidade por produto/serviço, informação e segurança |
| Desenvolvedor/integrador | Introduz vulnerabilidade, código malicioso, integração insegura ou ignora falha previsível | Responsabilidade por culpa técnica, contrato e, dependendo do caso, solidariedade |
| Provedor do modelo-base | Contribui causalmente por defeito estrutural, treinamento/avaliação negligente, violação de deveres regulatórios ou ocultação de risco conhecido | Responsabilidade proporcional e mais forte em riscos sistêmicos |
| Plataforma ou ferramenta externa | Participa materialmente do dano, permite abuso previsível ou ignora notificações/deveres próprios | Responsabilidade conforme sua contribuição e dever de controle |
| Vítima | Não deve arcar com a incerteza da cadeia tecnológica | Deve ter canal de reparação simples, com responsável identificável |

A boa regra é: **quem decide delegar poder de agir a um agente deve responder pelos riscos normais dessa delegação**. Quanto maior a autonomia, o acesso a dinheiro, dados, contas, infraestrutura ou direitos de terceiros, maior deve ser o dever de diligência.

Isso é consistente com uma análise recente específica sobre agentes que realizam transações em plataformas: instruções explícitas do usuário para violar a lei devem gerar responsabilidade primária do próprio usuário.[2]

## Regra por nível de autonomia

A responsabilidade deveria escalar com a capacidade operacional do agente.

| Nível do agente | Exemplo | Regime que eu defenderia |
|---|---|---|
| Assistivo | Redige e-mail; sugere código; resume documentos | Usuário responde pelo uso final; fornecedor responde por defeitos, privacidade e segurança |
| Executa sob aprovação | Agente prepara compra, pagamento ou publicação, mas exige confirmação humana | Quem aprova responde pelo ato; operador e fornecedor respondem por falhas do sistema |
| Autônomo limitado | Reposição de estoque até R$ 500; resposta automática a clientes; execução de playbook | Operador/empresa responde primariamente; precisa de limites, logs e mecanismos de interrupção |
| Autônomo de alto impacto | Concede crédito, define preço individual, contrata, faz transferências, seleciona candidatos, atua sobre infraestrutura | Responsabilidade objetiva ou quase objetiva do operador; auditoria, seguro e supervisão humana qualificada |
| Crítico | Saúde, segurança pública, mobilidade, energia, Justiça, direitos fundamentais | Autonomia fortemente limitada; decisões sensíveis devem ter revisão humana real e trilha de auditoria |

Para atividades de alto impacto, eu aplicaria uma lógica próxima à **responsabilidade objetiva**: a vítima não deveria precisar provar como ocorreu a falha dentro de uma arquitetura opaca de modelo, agentes, RAG, ferramentas, filas e APIs. Caberia à empresa demonstrar que adotou controles adequados e, se houver vários participantes, repartir depois o custo entre si.

No Brasil, isso já conversa com o Código de Defesa do Consumidor: o fornecedor de serviços responde independentemente de culpa por danos decorrentes de defeitos do serviço ou de informação insuficiente/inadequada sobre uso e riscos.  O próprio regime civil brasileiro também prevê obrigação de reparar sem culpa quando a atividade, por sua natureza, cria risco para direitos de terceiros.[3][4]

## O que conta como diligência

Não basta inserir nos Termos de Uso: “a IA pode errar” ou “o usuário é integralmente responsável”. Para agentes com capacidade de agir na internet, a diligência deveria ser técnica, operacional e documental.

Eu exigiria, proporcionalmente ao risco:

- Identidade verificável do responsável pelo agente em operações comerciais, profissionais ou de alto impacto.
- Declaração explícita do escopo: o que o agente pode fazer, em nome de quem, em quais sistemas e com quais limites.
- Permissões mínimas e temporárias: credenciais com escopo reduzido, expiração, rotação e isolamento por tenant.
- Limites financeiros, geográficos, de volume, de destinatários e de frequência.
- Aprovação humana para atos irreversíveis ou de alto impacto, como pagamentos, contratação, exclusão de dados, publicação em massa e mudanças de produção.
- Logs imutáveis de intenção, contexto, ferramentas chamadas, parâmetros, resultados, intervenções humanas e decisões de bloqueio.
- Kill switch e revogação imediata de credenciais.
- Testes de abuso: prompt injection, exfiltração de dados, fraude, escalada de privilégios, automação de spam e execução fora de escopo.
- Monitoramento contínuo e resposta a incidentes.
- Comunicação clara a terceiros de que estão interagindo com um agente automatizado, quando isso for relevante.
- Seguro obrigatório ou fundo de garantia para categorias de alto risco.

Esse desenho não é só “boa engenharia”; é a infraestrutura que torna possível determinar causalidade e distribuir responsabilidade. Sem logs e rastreabilidade, a empresa acaba tentando transformar sua própria opacidade em defesa jurídica.

O AI Act europeu adota uma lógica semelhante: provedores têm deveres de gestão de risco, documentação, logs, robustez, cibersegurança e monitoramento pós-mercado; quem implanta sistemas de alto risco deve assegurar supervisão humana, acompanhar a operação e comunicar/suspender o uso diante de risco relevante.[5][6]

## Aplicação a cenários reais

### Fraude financeira por agente

Se uma empresa dá a um agente acesso para pagar fornecedores e ele é induzido por prompt injection a transferir R$ 80 mil para um golpista, a empresa operadora deve responder inicialmente perante a vítima ou contratante.

Depois, a responsabilidade pode ser repartida:

- O integrador, se expôs credenciais sem segregação ou não validou o destinatário.
- O fornecedor do agente, se vendeu autonomia financeira sem controles mínimos previsíveis.
- O usuário, se autorizou expressamente uma operação ilícita ou desativou salvaguardas de modo imprudente.
- A instituição financeira, se falhou em seus deveres próprios de prevenção a fraude.

Não seria aceitável dizer: “o modelo decidiu”. A decisão operacional foi habilitada por uma arquitetura de permissões, políticas e integrações humanas.

### Agente que difama ou gera deepfake

Se um usuário manda o agente criar uma campanha difamatória, ele é o principal responsável. Mas a plataforma pode responder também se participou materialmente da distribuição, ignorou notificações válidas, facilitou a falsificação de identidade ou não implementou controles compatíveis com risco previsível.

### Agente que viola dados pessoais

Se um agente consulta CRM, perfis comportamentais e históricos de compra para tomar decisões ou realizar contatos, entram os deveres da LGPD. O controlador e o operador que causarem dano por tratamento irregular têm obrigação de reparação; a lei já prevê responsabilidade solidária em hipóteses específicas e direito de regresso entre os envolvidos.[7]

Isso torna particularmente importante diferenciar, no desenho técnico:

- Quem é o **controlador**: define finalidades e decisões principais sobre os dados.
- Quem é o **operador**: trata dados em nome do controlador e segundo suas instruções.
- Quem é apenas fornecedor de infraestrutura/modelo, mas pode assumir deveres maiores se efetivamente determina finalidades, reutiliza dados ou descumpre suas obrigações.

## Brasil: o caminho mais adequado

O Brasil não precisa esperar reconhecer “personalidade jurídica da IA” para lidar com isso. Na minha avaliação, essa seria uma solução prematura e perigosa: poderia funcionar como uma blindagem patrimonial para quem realmente lucra, controla e projeta sistemas de alto risco.

O país já possui peças jurídicas relevantes:

- **CDC**, para relações de consumo e defeitos de serviços digitais.
- **Código Civil**, para dano, culpa, nexo causal e atividades de risco.
- **LGPD**, para danos ligados a tratamento de dados pessoais.
- Direito societário, contratual, concorrencial, penal e regulatório, conforme o setor.

Além disso, o PL 2.338/2023, que trata do uso de IA, foi remetido à Câmara dos Deputados em 17 de março de 2025, segundo o acompanhamento oficial do Senado.  Uma regulamentação específica deveria complementar, não substituir, os regimes já existentes.[8]

Eu defenderia cinco princípios legislativos brasileiros:

1. **Sem lacuna de reparação**: todo agente que atue perante terceiros deve ter um responsável jurídico identificável.
2. **Responsabilidade proporcional ao controle**: quem configura objetivos, permissões e implantação responde mais.
3. **Responsabilidade objetiva em alto risco**: especialmente para finanças, saúde, trabalho, serviços públicos, biometria e infraestrutura crítica.
4. **Solidariedade externa, regresso interno**: a vítima cobra de um responsável solvente; os participantes repartem o custo depois conforme evidências.
5. **Rastreabilidade como dever legal**: sem logs mínimos, presume-se desfavoravelmente a falha de governança do operador ou fornecedor.

## Minha síntese

A pergunta certa não é “o agente é culpado?”, mas:

> Quem criou ou assumiu o risco de permitir que esse sistema atuasse, com quais poderes, quais controles, qual benefício e qual capacidade de evitar o dano?

Em geral:

- **Usuário** responde por instrução ilícita e uso manifestamente abusivo.
- **Empresa que implanta o agente** responde pela delegação operacional e pelos efeitos perante clientes e terceiros.
- **Fornecedor e integrador** respondem por defeitos técnicos, segurança, informações enganosas e falhas que estavam sob seu controle.
- **Plataformas** respondem quando têm participação causal, dever específico de agir ou ignoram riscos previsíveis.
- **O agente não responde como pessoa**; ele é evidência e instrumento da cadeia decisória.

Para quem constrói sistemas agentic, a consequência prática é forte: tratar governança, logs, limites de capacidade, aprovação humana e isolamento de credenciais como requisitos de produto — não como itens de compliance adicionados depois.

Citações:
[1] The Law of AI is the Law of Risky Agents Without Intentions https://lawreview.uchicago.edu/online-archive/law-ai-law-risky-agents-without-intentions
[2] Who bears the responsibility? Legal liability allocation for ... https://www.tandfonline.com/doi/full/10.1080/23311886.2026.2691325
[3] L8078compilado - planalto.gov.br https://www.planalto.gov.br/ccivil_03/leis/l8078compilado.htm?gad=1
[4] Mensagem nº 424 - Planalto http://www.planalto.gov.br/ccivil_03/veto_total/2002/mv424-02.htm
[5] AI Act | Shaping Europe's digital future - European Union https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai
[6] Article 26: Obligations of deployers of high-risk AI systems https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-26
[7] L13709 - Planalto https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm
[8] PL 2338/2023 - Senado Federal https://www25.senado.leg.br/web/atividade/materias/-/materia/157233
[9] Deconstructing 'Responsible AI': An Examination of Legal and ... https://link.springer.com/article/10.1007/s11196-025-10388-4?error=cookies_not_supported&code=72c1b572-3611-42f3-b5f0-a90711cb1275
[10] Liability for AI Agents https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5236649
[11] [PDF] On the legal responsibility of artificially intelligent agents https://techreg.org/article/download/10985/11959
[12] AI Systems and Liability: An Assessment of the Applicability of ... https://ojs.st-andrews.ac.uk/index.php/STALJ/article/download/2645/2032/10760
[13] Legal Liability and Agentic AI: How the Law Applies When ... https://law.duke.edu/news/legal-liability-and-agentic-ai-how-law-applies-when-bots-go-rogue
[14] [PDF] The Phantom Agent: Artificial Intentionality and Legal Responsibility https://law.stanford.edu/wp-content/uploads/2026/05/Gervais-Nay-2026-ThePhantomAgent-ArtificialIntentionalityLegalResponsibility.pdf
[15] Inherent and emergent liability issues in LLM-based ... https://arxiv.org/html/2504.03255v1
[16] High-level summary of the AI Act | EU Artificial Intelligence Act https://artificialintelligenceact.eu/high-level-summary/
[17] Article 26: Obligations of Deployers of High-Risk AI Systems https://artificialintelligenceact.eu/article/26/
[18] Nexus https://www.journals.kmanpub.com/index.php/aitechbesosci/article/download/3682/5806/17704
[19] L13709compilado https://www.planalto.gov.br/ccivil_03/%5C_ato2015-2018/2018/Lei/L13709compilado.htm
[20] pl-5276-16 - Planalto https://www.planalto.gov.br/ccivil_03/projetos/pl/2016/pl-5276-16.htm
[21] Agência Nacional de Defesa do Consumidor - Planalto https://www.planalto.gov.br/ccivil_03/consulta_publica/agencia_nacion.htm
[22] D2181 - Planalto https://www.planalto.gov.br/ccivil_03/decreto/d2181.htm
[23] L3071 - Planalto https://www.planalto.gov.br/ccivil_03/leis/l3071.htm
[24] L12965 - Planalto https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/lei/l12965.htm
[25] L13853 - Planalto https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2019/lei/l13853.htm
[26] Mensagem nº 424 - Planalto https://www.planalto.gov.br/ccivil_03/VETO_TOTAL/2002/Mv424-02.htm
[27] Mensagem nº 664-L8078-90 - Planalto https://www.planalto.gov.br/ccivil_03/leis/Mensagem_Veto/anterior_98/vep664-L8078-90.htm
[28] geral_index - Planalto https://www.planalto.gov.br/ccivil_03/
[29] ...............................................................................................................................................................................” (NR) https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2026/lei/l15352.htm
[30] L14133 - Planalto https://www.planalto.gov.br/ccivil_03/_ato2019-2022/2021/lei/l14133.htm
