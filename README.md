## Consultoria de TI - Solução Digital: Verificação de Idade e o ECA Digital  
## Projeto de Consultoria em Design Profissional  
  
## 1. Abertura  
**Nome da Consultoria:** ConectAge
-----------------------------------
**Dossiê Escolhido:** Dossiê 7 - Verificação de Idade e o ECA Digital.  
------------------------------------------------------------------------
**Recorte do Problema:** Verificação de idade em plataformas de jogos online e ambientes de comunicação interativa por voz e texto, com foco em comunidades virtuais semelhantes ao Discord e servidores de jogos multiplayer. Esses ambientes são os que ampliam os riscos para menores, como a possibilidade de interação com desconhecidos, a existência de servidores públicos, a comunicação em tempo real por voz e texto, as dificuldades de fiscalização de comunidades privadas e a exposição de crianças e adolescentes a contatos e conteúdos inadequados.  

    Integrantes:
    Gabriel da Silva Cesário - RGM: | Área: Ciência de Dados | GitHub:   
    Mariana Calderari - RGM: 48100072 | Área: Engenharia de Dados | GitHub:   
    Vitor Camilo de Santana - RGM: | Área: CiberSegurança | GitHub:   

## 2. Análise do Problema  
## Contexto e Impacto Social:  
  
As plataformas de comunicação interativa e servidores multiplayer, a exemplo do Discord, inserem-se no contexto de comunidades virtuais onde crianças e adolescentes interagem com usuários de diferentes localidades. Para dimensionar a relevância do problema no cenário nacional, a pesquisa TIC Kids Online Brasil 2024 (Cetic.br) aponta que 43% dos adolescentes de 15 a 17 anos já tiveram contato pela internet com pessoas que não conheciam pessoalmente (considerando o ambiente digital em geral), enquanto 9% dos usuários de 9 a 17 anos relataram esse tipo de contato especificamente por meio de jogos online. Embora tais indicadores nacionais reflitam a amplitude do fenômeno na rede, a escolha do Discord e de servidores interativos neste projeto constitui um recorte tecnológico, voltado a analisar os desafios práticos de moderação e proteção nesses ecossistemas.

Essas plataformas apresentam características que podem dificultar a proteção de menores, como servidores públicos, comunidades privadas e comunicação em tempo real por voz e texto. Embora essas funcionalidades favoreçam a interação entre usuários, também podem facilitar situações de cyberbullying, aliciamento, exposição a conteúdos inadequados e contatos abusivos. A fiscalização de comunidades privadas representa um desafio adicional para a identificação e prevenção dessas situações.

Outro problema está relacionado aos métodos tradicionais de verificação de idade. A autodeclaração, baseada apenas na informação fornecida pelo próprio usuário, não oferece comprovação efetiva e permite que menores informem idades falsas. Essa limitação é abordada pelo artigo 9º da Lei nº 15.211/2025 (ECA Digital), que exige mecanismos confiáveis de verificação de idade para impedir o acesso de menores a conteúdos e serviços inadequados, vedando a autodeclaração nesses casos.

Por outro lado, a utilização de documentos pessoais e dados biométricos para verificar a idade exige cuidados com a coleta, o processamento e o armazenamento dessas informações. A retenção desnecessária de documentos pode aumentar os riscos de vazamentos e acessos não autorizados. O Decreto nº 12.880/2026 estabelece que, na verificação por documentos, a coleta deve se limitar à informação necessária sobre a idade, determinando a eliminação imediata e irreversível da imagem ou cópia do documento após a extração dessa informação.  
  
## Causas Tecnológicas do Problema  
  
**1. Ineficácia dos Modelos Tradicionais:** A autodeclaração (*self-declaration*) permite que usuários informem qualquer idade sem apresentar comprovação. Como não existe uma validação efetiva, menores podem acessar plataformas e conteúdos restritos simplesmente alterando a data de nascimento no cadastro, tornando esse método pouco confiável.  
  
**2. Riscos da Centralização de Dados:** A exigência de documentos pessoais, como RG, CPF e fotografias, aumenta a quantidade de informações sensíveis coletadas e armazenadas pelas plataformas. A concentração desses dados em servidores cria alvos atrativos para ataques cibernéticos, vazamentos e acessos não autorizados. Além disso, o armazenamento prolongado ou o compartilhamento inadequado dessas informações pode comprometer a privacidade dos usuários.  
  
**3. Vulnerabilidades no Reconhecimento Facial:** Embora a biometria facial ofereça uma alternativa de verificação, sua utilização isolada apresenta limitações. Um menor pode utilizar o rosto de um adulto, como um responsável, para validar sua conta, especialmente quando o sistema não realiza verificações adicionais de identidade e autenticidade. Além disso, a coleta de características biométricas exige cuidados específicos, pois são dados pessoais sensíveis que, se expostos, não podem ser substituídos como uma senha convencional.  
  
## O que já existe e por que não basta  
  
1. **Verificação por Cartão de Crédito:** Utiliza a existência de um cartão bancário como indicativo de maioridade, mas apresenta limitações de acessibilidade e confiabilidade. Muitos adolescentes não possuem cartões próprios, especialmente aqueles em situação de vulnerabilidade socioeconômica. Além disso, o uso de cartões pertencentes aos pais ou responsáveis pode permitir que menores contornem a restrição, sem que a plataforma consiga confirmar quem está realmente utilizando o serviço.  
2. **Biometria Facial Isolada:** A utilização do reconhecimento facial pode facilitar a estimativa ou confirmação da idade, mas não garante, por si só, que a pessoa verificada seja a mesma que utilizará a conta. Um menor pode solicitar que um adulto realize a validação em seu lugar, utilizando o resultado para obter acesso à plataforma. Outro problema envolve a privacidade: imagens faciais e informações biométricas exigem proteção rigorosa, pois seu armazenamento e tratamento inadequados podem resultar em exposição de dados sensíveis e riscos permanentes aos usuários.  
  
## 3. Proposta Técnologica  
### Proposta Tecnológica e Arquitetura  
**Nome da solução:** GuardianGate-ZKP, plataforma federada de consentimento parental e verificação de idade com privacidade por design.  
**Resumo Executivo:** O GuardianGate-ZKP é uma proposta de arquitetura federada destinada a verificar a faixa etária de usuários e validar autorizações de responsáveis legais por meio de credenciais digitais verificáveis (Verifiable Credentials) e Provas de Conhecimento Zero (Zero-Knowledge Proofs – ZKP). A solução foi concebida para atuar como um middleware de interoperabilidade entre autoridades emissoras de identidade, carteiras digitais de usuários e plataformas consumidoras (como o Discord ou servidores de jogos multiplayer).

Para superar os desafios de segurança e privacidade, a arquitetura padroniza o uso de credenciais emitidas por autoridades confiáveis, o ecossistema OpenID4VP para transporte de apresentações, circuitos zk-SNARKs para provas criptográficas de elegibilidade sem exposição de dados civis, e um mecanismo híbrido de controle de tokens, sessões e revogação. A integração com plataformas consumidoras pressupõe a existência de APIs ou mecanismos de consentimento suportados pelas respectivas plataformas, garantindo a aplicação efetiva das regras de acesso.

#### 3.1 Faixas Etárias e Regras Adotadas 

| Faixa Etária | Regra no GuardianGate-ZKP | Fundamentação Legal / Decisão de Projeto |
| ------------------ | ------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------- |
| Menores de 13 anos | Acesso restrito por padrão a funcionalidades interativas abertas (chat global, voz com desconhecidos). Exige vincular a conta a um responsável legal e autorização expressa deste. | Decisão do projeto mais restritiva que a regra mínima, amparada pelo princípio da proteção integral da infância e pelas salvaguardas do Art. 21 da Lei nº 15.211/2025 (ECA Digital) para jogos e ambientes interativos, além da vinculação obrigatória do Art. 24.|
| 13 a 16 anos | Conta vinculada obrigatoriamente a um responsável legal, que autoriza permissões específicas. | Exigência direta do ECA Digital (Lei nº 15.211/2025, Art. 24). |
| 17 anos | Faixa etária validada por credencial verificável. Não há obrigação geral de vinculação da conta prevista no art. 24, mas permanecem aplicáveis as salvaguardas de interação previstas para jogos abrangidos pelo art. 21. | Distinção entre a regra de vinculação até 16 anos e as demais obrigações de proteção de adolescentes. |
| 18 anos ou mais | Prova criptográfica própria de maioridade (idade >= 18), sem vínculo parental. | Acesso liberado a ambientes restritos a adultos com privacidade. |
  
#### 3.2 Como Funciona para o Usuário (Passo a Passo)  
**1. Preparação Única (Emissão de Credenciais)**  
* **Emissão Confiável:** O adulto e o responsável obtêm suas credenciais digitais junto a uma autoridade emissora confiável (adotando o Gov.br como integração pretendida e arquiteturalmente planejada, cuja implementação efetiva depende de autorização institucional, acordos de interoperabilidade e disponibilidade de infraestrutura federada). O emissor valida em registros oficiais a filiação, a guarda/tutela e a data de nascimento, assinando digitalmente a credencial verificável. 
* **Comprovação do Vínculo:** Para emitir a credencial de responsabilidade parental, a entidade emissora deverá verificar a relação entre o menor e o responsável por meio de registros oficiais ou documentos legalmente aceitos, considerando também situações de guarda ou tutela. Após a validação, emitirá uma credencial assinada digitalmente, vinculando a autorização à relação jurídica comprovada.
* **Validade e Ciclo da Credencial do Emissor:** A credencial emitida possui um período de validade determinado e inclui referências a listas de revogação (Revocation Lists ou Status Lists 2025) mantidas pelo emissor. Caso ocorra alteração de guarda, tutela ou cancelamento cadastral, o emissor revoga a credencial de origem.
* **Armazenamento Seguro:** As credenciais ficam salvas exclusivamente no Aplicativo de Carteira Digital (*Wallet App*) do smartphone do usuário, protegidas pela biometria nativa do aparelho (FaceID/Impressão Digital), que jamais sai do dispositivo.  

**2. Fluxo para Usuários Adultos (18+)** 

1. A plataforma identifica a conta como não verificada e mantém as restrições de acesso aplicáveis.

2. O usuário seleciona a opção "Provar Maioridade" e acessa a solicitação de verificação por QR Code ou link seguro.

3. A carteira digital processa a solicitação OpenID4VP, valida localmente a assinatura do emissor e gera uma prova zk-SNARK demonstrando que idade é maior ou igual à 18 em relação à data atual, sem revelar a data de nascimento completa ou o documento de origem.

4. O verificador GuardianGate valida a prova criptográfica, verifica se o emissor é confiável, checa o status de revogação da credencial na lista do emissor e valida o nonce da transação para evitar ataques de repetição.

5. Após a validação, a plataforma recebe um atestado de maioridade e aplica as permissões correspondentes.erificador. A plataforma libera o acesso aos espaços de adultos.

**3. Fluxo de Autorização Parental (Menores de 17 Anos) e Aplicação do Art. 21 do ECA Digital**

1. **Tentativa de Acesso e Restrição Padrão (Privacy by Default):** Ao criar uma conta ou tentar acessar funcionalidades interativas, a plataforma mantém as restrições preventivas até que a verificação necessária seja concluída.

* **Integração com o Art. 21 do ECA Digital:** Em cumprimento ao Art. 21 — que exige salvaguardas e limitações padrão nas funcionalidades de interação em jogos e plataformas acessíveis a menores para assegurar o consentimento —, o acesso a chats diretos de voz/texto com desconhecidos, servidores abertos e canais não moderados permanece bloqueado preventivamente.

2. **Solicitação de Vínculo:** A plataforma gera um QR Code ou deep link seguro contendo um identificador de sessão único (nonce) e o client_id da plataforma, utilizando o protocolo OpenID4VP.

3. **Notificação, Painel Educativo e Autorização Parental:**

* O responsável recebe uma solicitação de autorização em seu próprio dispositivo.

* Ao autenticar-se localmente, visualiza um Painel Educativo de Riscos detalhando as funcionalidades solicitadas, os riscos associados e orientações de segurança.

* O responsável seleciona as permissões que deseja conceder, como chat de texto restrito a amigos ou desativação de comunicação por voz.

* A autorização é assinada digitalmente e vinculada à conta do menor, às permissões selecionadas e à validade da solicitação.

4. **Geração da Prova Criptográfica:** A carteira do responsável utiliza a credencial assinada pelo emissor e a autorização registrada para gerar uma prova criptográfica baseada em zk-SNARKs. A prova demonstra que:

* Existe uma credencial válida que comprova a relação de responsabilidade legal;

* O responsável autorizou as permissões solicitadas;

* As limitações padrão exigidas pelo Art. 21 foram revisadas e explicitamente consentidas pelo responsável;

* A autorização está vinculada à conta do menor e ao nonce da sessão, impedindo a reutilização de uma apresentação em outra transação.

* Os dados civis, como nomes, CPF e documentos de identificação, não são incluídos na apresentação enviada à plataforma.

5. **Validação e Liberação de Acesso:** O middleware GuardianGate valida a assinatura do emissor, a prova zk-SNARK, o status atualizado da credencial de filiação e o vínculo de sessão. Estando tudo correto, emite um Token de Autorização de curta duração (máximo de 15 minutos) contendo estritamente os escopos permitidos.

6. **Revogação Contínua:** O sistema diferencia a revogação da credencial-raiz (emitida pela autoridade) da revogação de permissões pontuais (realizada pelo responsável). O responsável pode alterar as permissões na carteira a qualquer momento, atualizando a versão da autorização no serviço de gestão e invalidando o token ativo.

#### 3.3 Arquitetura Técnica e Fluxo de Dados**  
**Componentes do Sistema**  
* **Emissor de Credenciais (Autoridade Federada):** Entidade responsável por verificar informações de identidade, idade e responsabilidade legal em fontes confiáveis e emitir credenciais digitais assinadas. O Gov.br é considerado uma possibilidade de integração futura, não uma integração já estabelecida pelo projeto.

* **Aplicativo de Carteira Digital (Wallet App):** Aplicativo no dispositivo móvel do usuário responsável pelo armazenamento seguro de credenciais, autenticação local (biometria) e execução de circuitos para geração de provas zk-SNARKs.

* **Verificador GuardianGate (Middleware API):** Serviço responsável por receber as apresentações OpenID4VP, validar assinaturas de emissores, verificar provas criptográficas, consultar o status de revogação e gerenciar nonces via Redis.

* **Plataforma Consumidora (Discord / Jogo Online):** Aplicação que solicita a verificação e recebe os atestados de idade e as permissões autorizadas, aplicando as regras de acesso aos seus próprios recursos.
A aplicação das regras de acesso depende de cooperação técnica e de integrações via API, Webhooks ou SDKs disponibilizados pela plataforma consumidora para impor o bloqueio de chats e canais de voz conforme as permissões validadas.

* **Serviço de Gestão de Autorizações:** Componente responsável por registrar as versões das permissões, processar alterações e revogações e comunicar as atualizações às plataformas integradas.

**Circuito zk-SNARKs**

* **Entradas Públicas (Public Inputs):**

    * Chave pública atual do emissor confiável (permitindo atualização e rotação de chaves).

    * O nonce da sessão e o identificador da plataforma (client_id).

    * O hash da política de permissões solicitadas.

    * O carimbo de data/hora (timestamp) atual para verificação de vigência.

* **Entradas Privadas (Private Inputs / Witness):**

    * A credencial digital assinada pelo emissor (contendo o identificador de filiação e faixa etária).

    * A assinatura digital do responsável que autorizou as permissões específicas.

* **Verificações Realizadas pelo Circuito:**

    * Verifica se a assinatura do emissor sobre a credencial é matematicamente válida utilizando a chave pública cadastrada.

    * Verifica se a data de validade da credencial é posterior ao timestamp atual e se a credencial não consta na lista de revogação do emissor.

    * Verifica se a assinatura da autorização parental corresponde à chave pública do responsável vinculado na credencial.

    * Agrega as restrições do Art. 21 e gera a prova de que as condições de idade e consentimento são verdadeiras, sem expor dados civis.

**Tokens, Sessões e Revogação**

  * **Nonce:** Identificador único de uso único (one-time) gerado por transação de verificação para prevenir ataques de repetição.

  * **Token de Autorização:** Credencial temporária de acesso emitida com validade restrita (configurada inicialmente para o teto de 15 minutos), entregue à plataforma consumidora após a validação bem-sucedida da prova zk-SNARK.

  * **Sessão:** Período de conexão do usuário na plataforma. Para mitigar o risco de o usuário manter acesso por 15 minutos após uma revogação, as plataformas consumidoras realizam checagens periódicas (heartbeat ou polling) ou recebem eventos via Webhook do Serviço de Gestão de Autorizações para revalidar o estado da autorização em tempo real.

**Revogação de Credencial-Raiz vs. Revogação de Permissão:**

  * **Revogação de Permissão:** O responsável altera as preferências na carteira; o GuardianGate invalida a versão anterior da autorização e encerra os escopos na plataforma.

 * **Revogação da Credencial de Filiação:** A autoridade emissora revoga a credencial de guarda/tutela na origem; ao tentar renovar o token ou passar pela verificação periódica, o circuito zk-SNARK falha por invalidação na lista de status do emissor, bloqueando imediatamente o acesso.

**Onde Ficam os Dados e Quem Acessa**

* **Dados de Identificação Civil (RG, CPF e documentos):** São utilizados pela entidade emissora durante a verificação da identidade e não são compartilhados diretamente com a plataforma de jogos ou com o verificador GuardianGate. Atendendo ao Art. 24, § 3º do Decreto nº 12.880/2026, garantindo que a infraestrutura não retenha cópias ou dados desnecessários.

* **Dados Biométricos:** Utilizados exclusivamente de forma local no hardware do dispositivo do usuário (Secure Enclave / Biometric API do smartphone) para desbloquear a carteira digital. Nenhuma imagem facial ou dado biométrico é transmitido aos servidores.

* **Credenciais Digitais:** Permanecem armazenadas na carteira digital do usuário, sob seu controle. O verificador recebe apenas as apresentações necessárias para validar cada solicitação.

* **Dados Temporários de Sessão (Tokens e Nonces):** Armazenados em instâncias Redis protegidas por criptografia e políticas de expiração automática (TTL de 5 minutos para sessões e 15 minutos para tokens). Em caso de indisponibilidade do Redis ou da API verificadora, o sistema adota comportamento de falha segura (fail closed), mantendo as restrições ativas até que a conectividade e a validação sejam restabelecidas.

**Política de Armazenamento Temporário e Segurança**

O Redis será configurado com políticas de expiração automática (TTL), controle de acesso por autenticação, comunicação protegida por criptografia e restrição de permissões aos serviços autorizados. Como parâmetro inicial de projeto, identificadores de sessão poderão expirar após cinco minutos, enquanto tokens de autorização poderão ter validade máxima de quinze minutos, com possibilidade de revogação antecipada. Esses períodos são parâmetros propostos e deverão ser ajustados conforme os requisitos de segurança e desempenho.

Os registros de aplicação não deverão armazenar credenciais completas, documentos ou conteúdos das provas criptográficas. Serão mantidos somente eventos técnicos indispensáveis para monitoramento e auditoria, com minimização de dados e controle de acesso.

Caso o Redis ou a API verificadora fiquem indisponíveis, novas autorizações e verificações não serão aprovadas automaticamente. O sistema adotará comportamento de falha segura (fail closed), mantendo as restrições até que a validação possa ser realizada novamente.

#### 3.4 Escolhas Técnicas e Justificativas**  
* **Por que utilizar ZKP:** As Provas de Conhecimento Zero permitem demonstrar que determinadas condições são verdadeiras sem revelar diretamente as informações utilizadas como base da comprovação. Entretanto, a confiabilidade depende da validade da credencial emitida e da segurança do mecanismo criptográfico.

* **Esquema zk-SNARKs:** A tecnologia foi escolhida como proposta para permitir provas compactas e verificações eficientes. O circuito criptográfico deverá validar as assinaturas e as condições necessárias, como maioridade, responsabilidade legal e autorização parental, considerando também a atualização das chaves dos emissores e o estado das credenciais.

* **Integração com OpenID4VP:** O protocolo organiza a solicitação e a apresentação das credenciais verificáveis. A geração e a validação das provas zk-SNARKs serão realizadas por componentes específicos da arquitetura GuardianGate, integrados ao fluxo de apresentação mediante formato criptográfico definido pelo projeto.

* **Gestão de Custo Computacional no Celular:** A credencial é armazenada na carteira e pode ser reutilizada enquanto permanecer válida. A geração da prova ocorre quando uma nova autorização ou apresentação é necessária, evitando processamento criptográfico desnecessário.

* **Tokens de Sessão e Proteção contra Rastreamento:** Os tokens possuem validade limitada, identificadores específicos por plataforma e vínculo com a transação correspondente. A utilização de identificadores distintos, provas não correlacionáveis e minimização de metadados busca reduzir a possibilidade de associação entre atividades realizadas em diferentes serviços. Essas medidas reduzem o risco de rastreamento, mas não garantem anonimato absoluto.

* **Revogação de Autorizações:** Cada autorização possui um identificador e uma versão. Quando o responsável revoga ou altera uma permissão, a versão anterior é invalidada e a plataforma consumidora recebe a atualização. As sessões ativas devem consultar o estado da autorização periodicamente ou receber notificações de revogação, impedindo a continuidade de permissões canceladas.

* **Padrões Abertos:** A arquitetura adota OpenID4VP para apresentação de credenciais verificáveis e considera OpenID Connect para autenticação federada. A escolha do formato de credencial e a integração com provas zk-SNARKs deverão seguir especificações técnicas compatíveis, com definição de interoperabilidade entre emissores, carteiras e verificadores.

* **Conformidade e Privacidade:** A proposta considera os princípios de finalidade, necessidade, segurança e prevenção da LGPD, além das exigências de proteção de crianças e adolescentes previstas no ECA Digital. A minimização do armazenamento, a proteção das credenciais e a possibilidade de revogação são medidas de segurança e privacidade que deverão ser acompanhadas de controles técnicos, organizacionais e jurídicos.

## 4. Análise Ética

**Matriz de riscos: (No mínimo 5, com classificação, impacto e controle)**

**Decisão de Implantação: ( implantar, implantar com controles ou não implantar ainda, em até 10 linhas.)**

**Controles antes de entrar em produção: no mínimo 6, cobrindo os seis eixos.**

**Seis eixos são: Transparência, Revisão Humana, Minimização de Dados, Segurança, Teste de Viés, Canal de Contestação**

**LGPD: dados tratados, finalidade, base legal, prazo, dados sensíveis ou de menores.**

**Comunicado público de até 600 caracteres, com a contagem.**

## 5. Acessibilidade e Inclusão Digital

**Quem pode ficar de fora? O que a proposta faz por cada grupo?**

**Requisitos com base na WCAG e na aula de Inclusão digital e Acessibilidade**

## 6. Sustentabilidade

**Impacto ambiental da solução, com
base na aula de TI Verde.**

**Quem mantém e quem paga depois
do primeiro ano.**

## 7. Impacto Esperado

**Indicadores mensuráveis, com
meta.**

**Como ouvir os usuários antes de
ampliar.**

**O que fazer se a solução não pegar.**

## 8. Quadro de Decisões do Projeto

**No mínimo 5 decisões do projeto.**

**Decisão, alternativas consideradas e por que esta.**

**Ex.: nuvem ou servidor próprio, app ou SMS.**

## 9. Capítulos Individuas
### 9.1 Capítulo Individual — Gabriel da Silva Cesário (Ciência de Dados)

* **Papel no Projeto:**

* **Plano de Desenvolvimento Profissional** (Metas SMART):

- **Específica (S):**

- **Mensurável (M):**

- **Atingível (A):**

- **Relevante (R):**

- **Temporal (T):**

* **Feedback Mariana Calderari:**

* **Feedback Vitor Camilo de Santana:**

### 9.2 Capítulo Individual — Mariana Calderari (Engenharia de Dados)

* **Papel no Projeto:**

* **Plano de Desenvolvimento Profissional** (Metas SMART):

- **Específica (S):**

- **Mensurável (M):**

- **Atingível (A):**

- **Relevante (R):**

- **Temporal (T):**

* **Feedback Gabriel da Silva Cesário:**

* **Feedback Vitor Camilo de Santana:**

### 9.3 Capítulo Individual — Vitor Camilo de Santana (CiberSegurança)

* **Papel no Projeto:**

* **Plano de Desenvolvimento Profissional** (Metas SMART):

- **Específica (S):**

- **Mensurável (M):**

- **Atingível (A):**

- **Relevante (R):**

- **Temporal (T):**

* **Feedback Gabriel da Silva Cesário:**

* **Feedback Mariana Calderari:**

## 10. Referências
