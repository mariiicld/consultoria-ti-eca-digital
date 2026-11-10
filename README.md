## Consultoria de TI - Solução Digital: Verificação de Idade e o ECA Digital  
## Projeto de Consultoria em Design Profissional  
  
## 1. Abertura  
**Nome da Consultoria:** ConectAge
-----------------------------------
**Dossiê Escolhido:** Dossiê 7 - Verificação de Idade e o ECA Digital.  
------------------------------------------------------------------------
**Recorte do Problema:** Verificação de idade em plataformas de jogos online e ambientes de comunicação interativa por voz e texto, com foco em comunidades virtuais semelhantes ao Discord e servidores de jogos multiplayer. Esses ambientes são os que ampliam os riscos para menores, como a possibilidade de interação com desconhecidos, a existência de servidores públicos, a comunicação em tempo real por voz e texto, as dificuldades de fiscalização de comunidades privadas e a exposição de crianças e adolescentes a contatos e conteúdos inadequados.  
9. Capítulos Individuais

9.1 Capítulo Individual — Matheus Souza Lima (Redes)

Papel no Projeto: Redes & Comunicação de Dados

No desenvolvimento da nossa solução de verificação de idade e moderação (Dossiê 7), meu foco principal foi a área de Redes, com atenção à comunicação, integração e troca de informações entre os diferentes componentes do sistema.

Minha contribuição esteve relacionada ao entendimento de como os dados são transmitidos, compartilhados e recebidos, buscando garantir uma comunicação eficiente e organizada entre os usuários e a plataforma. Também considerei a importância da conectividade e da segurança durante a transmissão das informações, evitando falhas de comunicação e possíveis vulnerabilidades.

Como o sistema envolve o tratamento de informações de crianças, adolescentes e responsáveis, é fundamental que a troca de dados aconteça de maneira confiável, protegida e eficiente, contribuindo para o funcionamento adequado da solução.

Plano de Desenvolvimento Profissional (Metas SMART)

Para continuar evoluindo após as entregas do projeto e ampliar minhas competências na área de Redes, estabeleci um plano de desenvolvimento profissional baseado na metodologia SMART, com objetivos específicos, mensuráveis e prazos definidos para alcançar uma evolução técnica e profissional.

Específica (S): Aprofundar meus conhecimentos na área de Redes, estudando conceitos de comunicação de dados, protocolos de comunicação, conectividade, integração entre sistemas e segurança na transmissão de informações. Também pretendo desenvolver conhecimentos sobre como diferentes sistemas se comunicam e compartilham dados de maneira eficiente.

Mensurável (M): Concluir pelo menos 3 cursos relacionados à área de Redes, estudar os principais protocolos de comunicação, como TCP/IP, HTTP e DNS, e desenvolver 1 projeto prático que demonstre a comunicação e a troca de informações entre diferentes sistemas. O progresso será acompanhado por meio da conclusão dos cursos e da documentação do projeto.

Atingível (A): Dedicar aproximadamente 5 horas semanais aos estudos, utilizando cursos online, materiais acadêmicos, videoaulas e exercícios práticos. A rotina será organizada para permitir o aprendizado gradual dos conteúdos, começando pelos conceitos fundamentais e avançando para aplicações práticas.

Relevante (R): Esse desenvolvimento é importante para minha formação acadêmica e profissional, pois o conhecimento em Redes é essencial para compreender como as informações circulam entre sistemas e dispositivos. Além disso, o domínio desses conceitos poderá ampliar minhas oportunidades no mercado de Tecnologia da Informação, principalmente em áreas relacionadas à infraestrutura, comunicação de dados, integração de sistemas e segurança da informação.

Temporal (T): Estabelecer o prazo de 6 meses para concluir os três cursos, aprofundar os estudos sobre os protocolos de comunicação e desenvolver o projeto prático. Ao final desse período, pretendo ter adquirido uma base de conhecimentos mais sólida na área de Redes e estar preparado para aplicar esses conhecimentos em projetos acadêmicos e profissionais.
**Integrantes:**
    
    Gabriel da Silva Cesário - RGM: 47784105 | Área: Ciência de Dados | GitHub: https://github.com/gabrielsilce
    Mariana Calderari - RGM: 48100072 | Área: Engenharia de Dados | GitHub: https://github.com/mariiicld  
    Vitor Camilo de Santana - RGM: 47807458 | Área: CiberSegurança | GitHub: https://github.com/vitorcamilodesantana-del 

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

#### 3.3 Arquitetura Técnica e Fluxo de Dados
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

#### 3.4 Escolhas Técnicas e Justificativas  
* **Por que utilizar ZKP:** As Provas de Conhecimento Zero permitem demonstrar que determinadas condições são verdadeiras sem revelar diretamente as informações utilizadas como base da comprovação. Entretanto, a confiabilidade depende da validade da credencial emitida e da segurança do mecanismo criptográfico.

* **Esquema zk-SNARKs:** A tecnologia foi escolhida como proposta para permitir provas compactas e verificações eficientes. O circuito criptográfico deverá validar as assinaturas e as condições necessárias, como maioridade, responsabilidade legal e autorização parental, considerando também a atualização das chaves dos emissores e o estado das credenciais.

* **Integração com OpenID4VP:** O protocolo organiza a solicitação e a apresentação das credenciais verificáveis. A geração e a validação das provas zk-SNARKs serão realizadas por componentes específicos da arquitetura GuardianGate, integrados ao fluxo de apresentação mediante formato criptográfico definido pelo projeto.

* **Gestão de Custo Computacional no Celular:** A credencial é armazenada na carteira e pode ser reutilizada enquanto permanecer válida. A geração da prova ocorre quando uma nova autorização ou apresentação é necessária, evitando processamento criptográfico desnecessário.

* **Tokens de Sessão e Proteção contra Rastreamento:** Os tokens possuem validade limitada, identificadores específicos por plataforma e vínculo com a transação correspondente. A utilização de identificadores distintos, provas não correlacionáveis e minimização de metadados busca reduzir a possibilidade de associação entre atividades realizadas em diferentes serviços. Essas medidas reduzem o risco de rastreamento, mas não garantem anonimato absoluto.

* **Revogação de Autorizações:** Cada autorização possui um identificador e uma versão. Quando o responsável revoga ou altera uma permissão, a versão anterior é invalidada e a plataforma consumidora recebe a atualização. As sessões ativas devem consultar o estado da autorização periodicamente ou receber notificações de revogação, impedindo a continuidade de permissões canceladas.

* **Padrões Abertos:** A arquitetura adota OpenID4VP para apresentação de credenciais verificáveis e considera OpenID Connect para autenticação federada. A escolha do formato de credencial e a integração com provas zk-SNARKs deverão seguir especificações técnicas compatíveis, com definição de interoperabilidade entre emissores, carteiras e verificadores.

* **Conformidade e Privacidade:** A proposta considera os princípios de finalidade, necessidade, segurança e prevenção da LGPD, além das exigências de proteção de crianças e adolescentes previstas no ECA Digital. A minimização do armazenamento, a proteção das credenciais e a possibilidade de revogação são medidas de segurança e privacidade que deverão ser acompanhadas de controles técnicos, organizacionais e jurídicos.

#### 3.5 Atuação por Área de Carreira no Projeto
* **Engenharia de Dados (Mariana Calderari):** Responsável pela arquitetura do fluxo de ingestão, processamento e organização dos eventos gerados pelo sistema, garantindo a comunicação eficiente entre os componentes. Atua no gerenciamento do armazenamento temporário em memória por meio do Redis, utilizando políticas de expiração (TTL) e descarte de dados (data purge) para reduzir a retenção de informações sensíveis e contribuir para a aplicação dos princípios de minimização e proteção de dados previstos na LGPD.

* **Ciência de Dados (Gabriel da Silva Cesário):** Responsável pelo desenvolvimento de mecanismos de monitoramento e análise dos eventos processados pelo sistema, identificando padrões anormais de utilização, como picos atípicos de solicitações de autorização ou tentativas de uso indevido. Também atua na avaliação dos mecanismos de análise, utilizando dados minimizados ou pseudonimizados, sem necessidade de acesso direto a documentos pessoais ou identidades civis.

* **Cibersegurança (Vitor Camilo de Santana):** Responsável pela modelagem de ameaças (Threat Modeling) e pela definição dos mecanismos de segurança criptográfica, incluindo a utilização de provas de conhecimento zero (zk-SNARKs). Atua na proteção das credenciais, na validação das provas criptográficas e na implementação de mecanismos contra ataques de repetição (Replay Attacks), garantindo a autenticidade das operações e contribuindo para a proteção das informações dos usuários, em conformidade com os requisitos de segurança e privacidade da LGPD e do ECA Digital (Lei nº 15.211/2025).

#### 3.6 O que a Tecnologia NÃO Resolve

**Supervisão Parental Contínua:** A tecnologia permite verificar a faixa etária e registrar o consentimento dos responsáveis, mas não substitui o acompanhamento da rotina digital, das interações e das amizades do menor. A autorização de acesso a determinada funcionalidade não significa que todas as interações realizadas nela serão seguras.

**Engenharia Social e Manipulação Psicológica:** A verificação de idade e o controle de permissões reduzem a possibilidade de acesso indevido a funcionalidades restritas, mas não impedem comportamentos inadequados praticados por outros usuários em espaços de interação autorizados. Situações de manipulação, assédio e aliciamento ainda exigem moderação, canais de denúncia e medidas de proteção complementares.

**Educação Digital e Empréstimo de Aparelhos:** O sistema não impede que um responsável autentique a carteira e entregue o dispositivo desbloqueado a um menor. Da mesma forma, não substitui a orientação sobre segurança digital, privacidade e comportamento adequado em ambientes virtuais.  

### 4. Análise Ética
#### 4.1 Matriz de Riscos Éticos

| ID | Risco Identificado | Severidade | Impacto | Mecanismo de Controle / Mitigação |
|---|---|---|---|---|
| R1 | Vazamento de dados de menores em servidores de jogos | Alta | Crítico | Adoção de ZKP e minimização rigorosa de dados; a plataforma consumidora recebe apenas atributos booleanos de autorização e escopos permitidos, sem armazenamento de documentos de identidade, CPFs ou datas de nascimento completas. |
| R2 | Burla por biometria de terceiros (menor usa rosto do pai) | Alta | Alto | Exigência de fluxo de consentimento no aplicativo próprio do responsável, protegido por biometria local do dispositivo, precedido de Painel Educativo de Riscos e vinculado à integração pretendida com autoridades autenticadoras (como o Gov.br, condicionada a acordos institucionais). Reforça-se que a autenticação tecnológica reduz, mas não anula totalmente o risco de conivência ou empréstimo de dispositivos, exigindo conscientização parental.|
| R3 | Rastreamento da atividade de navegação dos menores | Alta | Alto | Utilização de identificadores efêmeros (Ephemeral DIDs) e tokens rotativos por sessão; redução significativa da possibilidade de correlação de atividades entre jogos e plataformas diferentes, mitiga-se o rastreamento cruzado sem afirmar anonimato absoluto.|
| R4 | Exclusão de jovens cujos pais não possuem smartphones | Média | Alto | Proposta de parceria institucional com órgãos públicos de atendimento presencial (como CRAS, postos de atendimento integrado ou escolas públicas) para validação e emissão assistida de credenciais offline ou alternativas, concebida como modelo de cooperação pretendida.|
| R5 | Bloqueio Indevido de contas legítimas por falha de API ou Interrupção do Sistema | Média | Média | Adoção de arquitetura de falha segura (fail closed) para novas validações de segurança, combinada com uma janela temporária controlada e restrita para sessões já ativadas (sem concessão de novos privilégios durante a indisponibilidade), além de canal humano de contestação rápida.|

#### 4.2 Decisão de Implantação

**Decisão:** Implantar com Controles.

A solução resolve o gargalo de privacidade do ECA Digital (Lei 15.211/2025) e impede fraudes por biometria de terceiros ao combinar ZKP com o consentimento legal rastreável e informado do responsável, garantindo proteção a menores sem criar repositórios centralizados vulneráveis.

#### 4.3 Controles Antes da Entrada em Produção (6 Eixos)

**Transparência:** Publicação do código da biblioteca ZKP em open-source e política de privacidade com linguagem simplificada para adolescentes e pais.

**Revisão Humana:** Atendimento humano garantido em caso de contestação de bloqueio de acesso ou falha de vínculo parental.

**Minimização de Dados:** Arquitetura orientada estritamente aos princípios da LGPD (finalidade e necessidade), limitando o fluxo de dados entre o GuardianGate e as plataformas consumidoras a atestados de elegibilidade e escopos de permissão necessários.

**Segurança:** Testes de invasão (Pentest) periódicos na API do middleware e criptografia TLS 1.3 ponta a ponta.

**Teste de Viés:** Realização de auditorias e testes regulares para avaliar a taxa de sucesso de autenticação e usabilidade em diferentes faixas socioeconômicas e modelos de smartphones, prevenindo barreiras tecnológicas desproporcionais.

**Canal de Contestação:** Aba dedicada dentro da plataforma para contestar falhas de verificação em até 48h.

#### 4.4 LGPD (Lei Geral de Proteção de Dados Pessoais)

##### 4.4.1 Matriz de Governança e Operações de Tratamento de Dados (LGPD)

| Dado Tratado | Finalidade do Tratamento | Local de Processamento | Agente / Responsável | Prazo de Retenção | Base Legal Aplicável |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Dados Civis e de Filiação** *(RG, CPF, Certidão)* | Validação da identidade do responsável e da relação de dependência legal do menor. | Infraestrutura da Autoridade Emissora (ex.: Gov.br). | Controlador (Emissor de Identidade). | Retido na fonte emissora conforme legislação própria de identificação civil. | **Cumprimento de Obrigação Legal** (Art. 7º, II, LGPD e Decreto nº 12.880/2026). |
| **Credenciais Verificáveis e Chaves Privadas** | Armazenamento local para geração de provas criptográficas no dispositivo do usuário. | *Wallet App* (Armazenamento local protegido por biometria no smartphone). | Operador (Usuário / Carteira Digital). | Permanente no dispositivo até exclusão manual ou revogação. | **Consentimento do Responsável / Melhor Interesse** (Art. 14, § 1º, LGPD). |
| **Identificadores de Sessão (`Nonces` e `Client_ID`)** | Garantia de segurança contra ataques de repetição (*replay attacks*) e vinculação à solicitação. | Memória Cache do Verificador (Redis). | Co-controlador (GuardianGate Middleware). | Temporário (expiração em até 5 minutos via TTL). | **Garantia da Prevenção à Fraude e Segurança** (Art. 7º, IX, LGPD). |
| **Tokens de Autorização Pseudonimizados** | Liberação e controle granular de escopos e permissões ativas nas plataformas consumidoras. | Memória Cache do Middleware e Plataforma Consumidora. | Co-controladores (GuardianGate e Plataforma Consumidora). | Temporário (validade máxima de 15 minutos). | **Cumprimento de Obrigação Legal** (Art. 7º, II c/c Art. 14 da LGPD e Art. 9º da Lei nº 15.211/2025). |
| **Registros Técnicos de Aplicação (`Application Logs`)** | Auditoria técnica de segurança, monitoramento de disponibilidade e prevenção de acessos indevidos. | Servidores de Aplicação do Middleware GuardianGate. | Controlador (GuardianGate Middleware). | Até 6 meses (conforme exigência do Marco Civil da Internet). | **Cumprimento de Obrigação Legal** (Art. 15 da Lei nº 12.965/2014 - MCI). |

##### Princípios da LGPD Aplicados à Arquitetura

1. **Princípio do Melhor Interesse do Menor (Art. 14, *caput*):** Todas as escolhas tecnológicas visam assegurar o desenvolvimento saudável e a proteção contra abordagens inadequada em ambientes virtuais, equilibrando a tutela parental com a privacidade digital do adolescente.

2. **Minimização e Necessidade (Art. 6º, III):** A plataforma consumidora recebe apenas atestados booleanos e escopos de permissão necessários à prestação do serviço interativo, eliminando o compartilhamento de documentos ou dados de qualificação civil.

3. **Segurança e Prevenção (Art. 6º, VII e VIII):** O uso de Provas de Conhecimento Zero (zk-SNARKs), aliado à eliminação de bases centralizadas de dados pessoais, impede o vazamento massivo de informações de crianças e adolescentes.

4. **Livre Acesso e Transparência (Art. 6º, IV e VI):** O responsável possui gestão contínua sobre as permissões concedidas por meio da carteira digital, podendo consultar, alterar ou revogar os escopos autorizados a qualquer momento.

#### 4.5 Comunicado Público à Sociedade

"Na ConectAge, proteger nossas crianças no ambiente digital não significa abrir mão da privacidade das famílias. Nossa nova solução para jogos online e plataformas como o Discord conecta o consentimento dos pais à verificação de idade sem armazenar fotos, RG ou históricos de navegação. Utilizando criptografia de Prova de Zero Conhecimento e autenticação legal via Gov.br com alertas de riscos informados, garantimos o cumprimento rigoroso do ECA Digital, mantendo os ambientes virtuais seguros para os jovens e totalmente privados para todos." (545 Caracteres)

## 5. Acessibilidade e Inclusão Digital  
#### 5.1 Quem pode ficar de fora?  
**1. Pessoas com Deficiência Visual ou Baixa Visão:** Responsáveis ou menores que utilizam leitores de tela e navegação por voz podem ser excluídos se a interface do aplicativo de carteira (*Wallet App*) não seguir diretrizes estritas de marcação acessível.  
2. **Famílias em Situação de Vulnerabilidade Socioeconômica e Alfabetização Digital Reduzida:** Pais com baixa escolaridade ou sem familiaridade com autenticação em duas etapas, como aqueles que não possuem conta Ouro/Prata no Gov.br.  
3. **Pessoas com Deficiência Motora:** Dificuldades de manuseio e navegação em telas sensíveis ao toque sem suporte a acionadores externos ou comandos de voz.  
4. **Exclusão Tecnológica por Dispositivos Antigos ou Conectividade Limitada:** Famílias que utilizam smartphones de baixo custo (sem leitor biométrico nativo) ou residem em áreas com sinal de internet instável.  
  
#### 5.2 Soluções de Inclusão e Requisitos de Acessibilidade (WCAG 2.1)  
  
Para garantir que nenhum grupo seja marginalizado no cumprimento das exigências do ECA Digital, a plataforma tem os requisitos baseados na WCAG 2.1 (Nível AA).  
  
* **Acessibilidade Visual (Perceptível - WCAG Nível AA):**  
    * **Compatibilidade Total com Leitores de Tela:** Implementação rigorosa de atributos ARIA (*Accessible Rich Internet Applications*) e rótulos legíveis (*labels*) para NVDA, TalkBack e VoiceOver em toda a interface do *Wallet App* e do Painel Educativo.  
    * **Contraste Mínimo e Adaptabilidade:** Razão de contraste mínima de 4,5:1 para textos normais e 3:1 para textos grandes. Para componentes visuais e elementos gráficos necessários à identificação de controles, será adotado contraste mínimo de 3:1 em relação às cores adjacentes, conforme os critérios aplicáveis da WCAG 2.1. A interface também oferecerá suporte a modo de alto contraste e redimensionamento de texto de até 200% sem perda de conteúdo ou funcionalidade.  
    * **Navegação por Código de Cores Não Exclusivo:** Avisos e status de restrição não dependem exclusivamente da cor (utilizando ícones e texto descritivo concomitante).  
* **Acessibilidade Motora e Operável:**  
    * **Áreas de Toque Expandidas:** Botões de aprovação e seleção terão dimensões mínimas de 48x48 dp, como requisito adicional de acessibilidade adotado pelo projeto para facilitar a interação de pessoas com dificuldades motoras.  
    * **Atalhos e Comandos por Voz:** Integração com assistentes nativos para permitir a navegação e leitura do Painel Educativo sem necessidade de digitação complexa.  
* **Inclusão Digital para Famílias Conectadas por Dispositivos Simples:**  
    * **Sistemas de Fallback Sem Biometria:** Para aparelhos sem leitor de impressão digital/FaceID, permite-se o desbloqueio local da *wallet* via PIN numérico forte vinculado ao hardware seguro (Keystore/Keychain).  
    * **PWA / Aplicativo Leve (*Lite*):** Desenvolvimento de uma versão otimizada do aplicativo, com consumo de dados reduzido e compatibilidade com redes 2G/3G. O sistema poderá armazenar temporariamente a credencial e os dados necessários no dispositivo para permitir o acesso às informações já carregadas durante períodos sem conexão. Entretanto, a validação da autorização será realizada online, sempre que necessária, para verificar a autenticidade da prova, a validade da credencial, possíveis revogações, a expiração do token e a proteção contra reutilização de nonces. Caso não exista conexão, operações que dependam dessa validação ficarão pendentes até o restabelecimento da internet, sem liberar indevidamente o acesso.  
* **Inclusão Presencial e Atendimento Físico:**  
    * **Postos de Validação Auxiliada:** Para responsáveis sem smartphone ou conta no Gov.br, firma-se parceria com postos de atendimento público (ex.: Poupatempo, CRAS, escolas públicas) para emissão e validação presencial do vínculo de dependência e emissão de credenciais impressas em QR Code seguro/offline  
    * **Credenciais Impressas em QR Code:** Possibilidade de emissão de credenciais impressas contendo QR Code com dados mínimos e assinatura digital verificável. Para reduzir riscos de cópia e reutilização, serão adotados mecanismos de validade limitada, identificação única, controle de utilização e consulta de revogação quando houver conexão. A assinatura digital permitirá verificar a autenticidade e detectar alterações no conteúdo, mas não impedirá, isoladamente, a cópia do código. Portanto, a validação offline terá limitações e não será considerada suficiente para operações que exijam confirmação de revogação ou controle de uso em tempo real.

## 6. Sustentabilidade
#### 6.1 Impacto Ambiental e Práticas de TI Verde

A infraestrutura e o software da solução foram desenhados com base nos princípios de TI Verde e Software Verde (Green Software Foundation), reconhecendo que a computação digital gera emissões reais de carbono e demanda de recursos energéticos e hídricos:

**Computação em Borda (Edge Computing) e Redução de Carga de Processamento:**
A geração das provas criptográficas ZKP é processada localmente nos dispositivos dos usuários. Isso evita o tráfego contínuo e a sobrecarga computacional em servidores centrais, diminuindo a demanda de CPUs/GPUs nos data centers e reduzindo a pegada de carbono por requisição.

**Infraestrutura Nuvem Hyperscale Eficiente (Otimização de PUE):**
A camada de API do verificador é hospedada exclusivamente em provedores de nuvem hyperscale comprometidos com o uso de 100% de energia renovável (eólica e solar) e com baixo PUE (Power Usage Effectiveness). Isso reduz o consumo elétrico associado aos sistemas de refrigeração e servidores em comparação com data centers convencionais.

**Software Sustentável e Mitigação de Lixo Eletrônico (E-Waste):**

**Arquitetura Event-Driven sem Polling:** Utilização de conexões assíncronas WebSockets e mensageria orientada a eventos para eliminar chamadas redundantes (HTTP polling), reduzindo o desperdício de ciclos de processamento e banda.

**Preservação da Vida Útil do Hardware:** Algoritmos leves de verificação minimizam a carga térmica nos smartphones dos usuários e servidores, retardando o desgaste dos componentes eletrônicos e combatendo o acúmulo de lixo eletrônico.

**Métricas de Carbono e Transparência:**
Adoção das bibliotecas da Green Web Foundation no ambiente de CI/CD para medir e auditar as emissões estimadas por requisição, mantendo um arquivo público na raiz do domínio da solução.

#### 6.2 Sustentabilidade Financeira (Manutenção Pós-Ano 1)

**Modelo B2B (Business to Business):**
A plataforma adota um modelo de licenciamento de API cobrado diretamente das empresas operadoras de jogos online, plataformas de comunicação e comunidades virtuais (ex.: Discord, Epic Games, Roblox). As famílias e usuários finais têm acesso 100% gratuito.

**Estrutura de Custo por Volume de Verificações:**
A manutenção do serviço a partir do segundo ano é custeada por contratos corporativos baseados em pacotes de chamadas de verificação de sessão (pay-per-verification).

**Custos Operacionais Enxutos:**
Devido à arquitetura descentralizada (onde o custo de armazenamento de credenciais fica no dispositivo do usuário), os custos operacionais da consultoria reduzem-se à manutenção da API Verificadora efêmera, auditorias de segurança e suporte a usuários.

## 7. Impacto Esperado

#### 7.1 Indicadores Mensuráveis e Fundamentação de Metas

A avaliação do impacto do GuardianGate-ZKP é orientada por indicadores-chave de desempenho (KPIs) com metas fundamentadas em testes de arquitetura e validação contínua:

* **Eficácia na Restrição de Acessos Indevidos:**
    * **Meta Projetada:** Redução estimada de até 85% a 90% na presença de menores não autorizados em canais restritos.
    * **Justificativa e Linha de Base:** Em contraste com o modelo tradicional de autodeclaração de idade (que possui efetividade próxima de zero em impedir falsificação de data de nascimento), a exigência de prova criptográfica derivada de fonte confiável elimina a criação de contas sem validação. A margem residual não nula (10% a 15%) considera cenários de conivência parental direta (empréstimo voluntário do dispositivo/conta do adulto ao menor) e eventuais limitações de cobertura inicial do sistema.

* **Eficiência do Fluxo de Aprovação Parental:**
   * **Meta Projetada:** Tempo médio de resposta e aprovação parental inferior a 15 segundos (após abertura da notificação no dispositivo do responsável).
   * **Justificativa e Plano de Testes:** A meta baseia-se na otimização dos componentes do fluxo: autenticação biométrica local no smartphone (aprox. 1 a 2 segundos), exibição da interface do Painel Educativo pré-carregada e geração do circuito zk-SNARK em hardware móvel (estimada em menos de 3 a 5 segundos em processadores móveis intermediários/avançados), somada à latência de rede da API efêmera (Redis/AWS). A viabilidade do tempo de resposta será aferida por meio de testes sintéticos de carga de benchmarking e testes de usabilidade com grupos de usuários em ambiente de testes (sandbox).

* **Indicador de Segurança da Informação e Privacidade:**
    * **Meta Projetada:** Zero incidentes confirmados de vazamento de dados civis de menores ou responsáveis na infraestrutura da plataforma durante os ciclos de operação monitorada.
    * **Justificativa e Monitoramento:** O indicador é sustentado pelo princípio de Privacy by Design, dado que a arquitetura não armazena repositórios centralizados de RG, CPF, fotos ou documentos. A meta não é apresentada como uma garantia absoluta infalível de software, mas como um objetivo de controle auditável, respaldado por varreduras de vulnerabilidade contínuas, programas de recompensa por falhas (bug bounty), testes anuais de intrusão (Pentest) por auditorias independentes e monitoramento de logs de segurança.

##### 7.2 Escuta dos Usuários e Plano de Contingência

* **Plano de Escuta e Governança Participativa:**
   * **Pesquisas de Usabilidade e Satisfação:** Avaliação contínua da experiência de uso no Wallet App e nas interfaces integradas, medindo o índice de facilidade de aprovação e clareza do Painel Educativo.
   * **Canal de Diálogo Institucional:** Criação de um conselho consultivo e canal de diálogo recorrente com associações de pais, educadores, especialistas em segurança digital e entidades de defesa dos direitos da infância e juventude, coletando relatórios periódicos de percepção de risco e usabilidade.

* **Plano de Contingência Operacional (Resiliência sem Quebra de Confiança):**
   * **Mecanismo de Falha Segura (Fail-Closed):** Em caso de indisponibilidade temporária ou instabilidade nos serviços de emissão e verificação primários (como a infraestrutura do Gov.br), a plataforma não libera acessos não validados preventivamente, priorizando a proteção integral do menor.
   * **Emissores de Backup e Autoridades Federadas Homologadas:** Em vez de recorrer a chaves descentralizadas sem governança definida, o chaveamento de contingência opera exclusivamente entre Autoridades Certificadoras e Emissores Oficiais previamente homologados na federação de identidades da plataforma (como identidades digitais emitidas por órgãos estaduais ou entidades governamentais equivalentes). Para que um emissor alternativo seja aceito no fluxo de contingência, ele deve possuir cadeia de custódia pública validada, suporte a checagem de listas de revogação em tempo real e comprovação documental da relação de responsabilidade legal nos mesmos padrões de confiabilidade do emissor principal.

## 8. Quadro de Decisões do Projeto

| # | Decisão do Projeto | Alternativas Consideradas | Justificativa da Escolha |
|---|---|---|---|
| 1 | Arquitetura ZKP com Consentimento Parental e Painel Educativo | Biometria Facial Simples no Login | Elimina a burla em que o menor usa o rosto do responsável, conscientiza os pais dos riscos e evita armazenamento invasivo de biometria. |
| 2 | Computação em Borda (Edge) no App Mobile | Processamento em Nuvem Centralizado | Reduz custos de infraestrutura, aumenta a privacidade e melhora a sustentabilidade energética (TI Verde). |
| 3 | Autenticação Federada via Gov.br | Banco de Dados Próprio com Fotos de RG | Elimina a necessidade de a consultoria guardar documentos de cidadãos, utilizando a infraestrutura pública existente. |
| 4 | Modelo Comercial B2B (Plataformas Pagam) | Cobrança por Usuário / Anúncios | Garante acesso universal e gratuito para famílias de qualquer classe social. |
| 5 | Tokens de Sessão Efêmeros (Curta Duração) | Tokens de Acesso Permanentes | Impede que a atividade de navegação do usuário seja rastreada entre diferentes jogos ou servidores. |

## 9. Capítulos Individuais
### 9.1 Capítulo Individual — Gabriel da Silva Cesário (Ciência de Dados)

* ** Papel no Projeto: Ciência de Dados & Ética Algorítmica**
No desenvolvimento da nossa solução de verificação de idade e moderação (Dossiê 7), meu foco principal foi a criação, treinamento e avaliação dos modelos de detecção de anomalias operacionais dentro do fluxo de verificação.

Além disso, atuei diretamente na auditoria do sistema para garantir a ausência de viés algorítmico. Como o sistema lida com o cumprimento do ECA Digital e atende crianças, adolescentes e responsáveis de diferentes
perfis, era indispensável garantir que os modelos de checagem e detecção funcionassem com a mesma precisão e equidade para diferentes faixas populacionais, tons de pele e condições de iluminação.
(Todo o progresso, experimentos de modelos e pipelines de validação estão registrados e confirmados via commits e Pull Requests no repositório do projeto no GitHub).

* **Plano de Desenvolvimento Profissional (Metas SMART)**
Para continuar evoluindo após as entregas do projeto e expandir minhas competências na área de dados voltada à segurança, estruturei meu plano de carreira no modelo SMART:

- **Específica (S)**: Aprofundar meus conhecimentos em Aprendizado de Máquina com foco em Privacidade (Privacy-Preserving Machine Learning e Federated Learning), entendendo como treinar modelos seguros sem expor dados
sensíveis de usuários.

- **Mensurável (M)**: Concluir 2 cursos especializados na plataforma Coursera e desenvolver/publicar 1 projeto prático open-source no GitHub aplicando aprendizagem federada.

- **Atingível (A)**: Organizar uma rotina de estudo dedicada de 5 horas semanais nos fins de semana, ao longo de 5 meses.

- **Relevante (R)**: Aumentar minha empregabilidade e diferencial no mercado de Ciência de Dados, especializando-me em ética algorítmica, privacidade de dados e segurança da informação.

- **Temporal (T)**: Conclusão total das etapas e publicação do projeto no repositório no prazo limite de 6 meses.

* **Feedback Mariana Calderari:** Demonstrou comprometimento com a proposta do projeto, contribuindo com a perspectiva da Ciência de Dados e sua relação com o monitoramento e a análise de informações. Sua área de atuação é importante para identificar padrões, acompanhar indicadores e auxiliar na avaliação da eficácia da solução, especialmente na identificação de possíveis comportamentos anômalos e na análise dos resultados. Na área de desenvolvimento, acredito que possa aprofundar seus conhecimentos em análise de dados, desenvolvimento de modelos de detecção de anomalias e avaliação de métricas, buscando transformar os dados gerados pelo sistema em informações úteis para aprimorar a segurança e a experiência dos usuários.

* **Feedback Vitor Camilo de Santana:** O trabalho do Gabriel foi fundamental para o projeto, contribuindo para a prevenção de falhas no sistema e evitando possíveis preconceitos nos algoritmos, garantindo que a solução fosse justa e acessível para todos os usuários. Também é importante destacar sua preocupação com a confiabilidade dos modelos e com a responsabilidade no uso da inteligência artificial, aspectos essenciais para o sucesso da solução.

### 9.2 Capítulo Individual — Mariana Calderari (Engenharia de Dados)

* **Papel no Projeto:** Responsável pela estruturação do fluxo de dados responsável por receber, organizar e processar, em tempo real, os eventos relacionados à verificação de idade e ao consentimento parental. Minha atuação está voltada à definição dos processos de ingestão e processamento, ao gerenciamento do armazenamento temporário em Redis e ao estabelecimento de políticas de expiração (TTL) e descarte automático (data purge). Essas atividades contribuem para manter o sistema eficiente, com baixa latência e tratamento adequado das informações, respeitando os princípios de privacidade e proteção de dados estabelecidos pela LGPD.

* **Plano de Desenvolvimento Profissional** (Metas SMART):

- **Específica (S):** Aprofundar meus conhecimentos em Engenharia de Dados, com foco no desenvolvimento de pipelines ETL/ELT, processamento de dados em tempo real, banco de dados Redis e serviços de computação em nuvem,
-  especialmente AWS.

- **Mensurável (M):** Concluir pelo menos 2 cursos relacionados à área e desenvolver 1 projeto prático no GitHub envolvendo ingestão, processamento e armazenamento temporário de dados, com aplicação de políticas TTL e
descarte automático de informações.

- **Atingível (A):** Dedicar aproximadamente 5 horas semanais aos estudos, utilizando cursos online, documentação oficial e desenvolvimento de projetos práticos para consolidar os conhecimentos adquiridos.

- **Relevante (R):** Desenvolver competências técnicas necessárias para atuar profissionalmente como Engenheira de Dados, especialmente na construção de pipelines eficientes, escaláveis e seguros, capazes de processar grandes volumes de informações sem comprometer a privacidade dos usuários.

- **Temporal (T):** Concluir os cursos e desenvolver o projeto prático no prazo de 6 meses, utilizando os resultados como parte do meu portfólio profissional.

* **Feedback Gabriel da Silva Cesário:** A Mariana foi responsável pela arquitetura e estruturação dos fluxos de dados do sistema. Graças à organização dos fluxos em tempo real e ao uso inteligente do
*  Redis com as políticas de TTL e descarte automático , garantiu ao sistema alta performance, baixa latência e rigorosa observância aos preceitos da LGPD.

* **Feedback Vitor Camilo de Santana:** O papel exercido pela Mariana e sua liderança foram fundamentais para o projeto, principalmente na organização do fluxo de dados, contribuindo para a otimização dos processos e garantindo maior segurança das informações. Além disso, sua atuação foi importante para manter a qualidade e a eficiência no tratamento dos dados, proporcionando uma estrutura mais organizada e confiável para o funcionamento da solução.

### 9.3 Capítulo Individual — Vitor Camilo de Santana (CiberSegurança)

* **Papel no Projeto:** Responsável pela análise e definição das diretrizes de cibersegurança aplicadas à solução digital de verificação de idade, considerando os riscos relacionados ao tratamento de dados pessoais, especialmente aqueles pertencentes a crianças e adolescentes. Sua atuação envolve a elaboração de estratégias para proteger as informações dos usuários, prevenir acessos não autorizados e garantir a integridade e a confidencialidade dos dados durante todo o processo de validação.
Outra responsabilidade importante é estabelecer diretrizes de conformidade com a Lei Geral de Proteção de Dados (LGPD), considerando os princípios de finalidade, necessidade, transparência, segurança e melhor interesse da criança e do adolescente. Também são consideradas medidas de proteção para as APIs utilizadas na comunicação entre os componentes da plataforma, incluindo autenticação, controle de acesso, criptografia e monitoramento de atividades suspeitas.

* **Plano de Desenvolvimento Profissional** (Metas SMART):

- **Específica (S):** Desenvolver conhecimentos avançados em cibersegurança, com foco em proteção de dados pessoais, segurança de APIs, análise de vulnerabilidades, arquitetura de sistemas seguros e conformidade com a LGPD. Buscar uma certificação profissional reconhecida na área, como CompTIA Security+, aprofundando também os estudos sobre criptografia e tecnologias de preservação da privacidade, como Zero-Knowledge Proofs.

- **Mensurável (M):** Concluir pelo menos dois cursos especializados em segurança da informação e proteção de dados, realizar dez simulados preparatórios para a certificação CompTIA Security+, buscando alcançar uma média mínima de 85% de acertos, e desenvolver um projeto prático documentado no GitHub envolvendo análise de vulnerabilidades, proteção de APIs e aplicação de boas práticas de segurança.

- **Atingível (A):** Estabelecer uma rotina de estudos de quatro a cinco horas semanais durante seis meses, utilizando cursos online, documentação técnica, materiais especializados e laboratórios práticos de cibersegurança. Aplicar os conhecimentos adquiridos por meio de pequenos projetos, exercícios de identificação de vulnerabilidades e estudos de casos relacionados à proteção de dados.

- **Relevante (R):** Fortalecer a formação profissional para atuar na área de Segurança da Informação, especialmente em atividades relacionadas à proteção de dados, segurança de aplicações e governança de TI. O desenvolvimento dessas competências permitirá contribuir para a construção de sistemas digitais mais seguros, confiáveis e alinhados às exigências da LGPD e às necessidades de proteção de crianças e adolescentes no ambiente digital.

- **Temporal (T):** Concluir os cursos e o projeto prático em até seis meses, realizar a preparação completa para a certificação e buscar sua aprovação em um prazo máximo de dez meses.

* **Feedback Gabriel da Silva Cesário:** A atuação do Vitor foi determinante para a segurança e a conformidade jurídica da solução. A definição rigorosa das diretrizes de cibersegurança, a proteção avançada das APIs e a estrita observância à LGPD — com foco especial na proteção de crianças e adolescentes — garantiram a integridade, a confidencialidade e a confiabilidade de todo o fluxo de verificação de idade

* **Feedback Mariana Calderari:** Demonstrou comprometimento na definição das estratégias de cibersegurança do projeto, contribuindo para a análise de riscos e para a elaboração dos mecanismos de proteção das informações dos usuários. Sua participação foi importante principalmente na abordagem de segurança das credenciais digitais, utilização de provas de conhecimento zero (zk-SNARKs), proteção das APIs e prevenção de ataques de repetição (Replay Attacks). Também considero positiva sua preocupação com a conformidade da solução em relação à LGPD e à proteção de crianças e adolescentes. Na sua área de desenvolvimento, acredito que possa aprofundar ainda mais os conhecimentos sobre implementação prática de mecanismos criptográficos e testes de vulnerabilidade, fortalecendo a capacidade de transformar as estratégias de segurança propostas em soluções tecnicamente aplicáveis.

## 10. Referências

BRASIL. Lei nº 13.709, de 14 de agosto de 2018. Lei Geral de Proteção de Dados Pessoais (LGPD). Brasília, DF, 2018. Disponível em: https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm. Acesso em: 28 out. 2026.

BRASIL. Lei nº 12.965, de 23 de abril de 2014. Estabelece princípios, garantias, direitos e deveres para o uso da Internet no Brasil (Marco Civil da Internet). Brasília, DF, 2014. Disponível em: https://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/lei/l12965.htm. Acesso em: 27 out. 2026.

BRASIL. Lei nº 15.211, de 17 de setembro de 2025. Dispõe sobre a proteção de crianças e adolescentes em ambientes digitais (ECA Digital). Brasília, DF, 2025. Disponível em: https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2025/lei/l15211.htm. Acesso em: 27 out. 2026. 
Senado Federal

BRASIL. Decreto nº 12.880, de 18 de março de 2026. Regulamenta a Lei nº 15.211/2025. Brasília, DF, 2026. Disponível em: https://www.gov.br/mj/pt-br/assuntos/arquivos-imprensa/sedigi/decretos-eca-digital.pdf. Acesso em: 27 out. 2026. 

AUTORIDADE NACIONAL DE PROTEÇÃO DE DADOS (ANPD). Radar Tecnológico: Mecanismos de Aferição de Idade. 2026. Disponível em: https://www.gov.br/anpd/pt-br/centrais-de-conteudo/documentos-tecnicos-orientativos/radar-tecnologico-5-mecanismos-de-afericao-de-idade.pdf. Acesso em: 29 out. 2026. 

AUTORIDADE NACIONAL DE PROTEÇÃO DE DADOS (ANPD). Guia orientativo para definições dos agentes de tratamento de dados pessoais e do encarregado. 2024. Disponível em: https://www.gov.br/anpd/pt-br/centrais-de-conteudo/materiais-educativos-e-publicacoes/guia-orientativo-para-definicoes-dos-agentes-de-tratamento-de-dados-pessoais-e-do-encarregado. Acesso em: 4 nov. 2026. 

OPENID FOUNDATION. OpenID for Verifiable Presentations 1.0. Final Specification, 2025. Disponível em: https://openid.net/specs/openid-4-verifiable-presentations-1_0-final.html. Acesso em: 4 nov. 2026.

INTERNATIONAL TELECOMMUNICATION UNION (ITU-T). Recommendation X.1285: OpenID Connect Core 1.0 – Errata Set 2. 2025. Disponível em: https://www.itu.int/rec/T-REC-X.1285-202505-I. Acesso em: 2 nov. 2026. 

9. WORLD WIDE WEB CONSORTIUM (W3C). Verifiable Credentials Data Model v2.0. W3C Recommendation, 15 maio 2025. Disponível em: https://www.w3.org/TR/vc-data-model-2.0/. Acesso em: 2 nov. 2026. 

WORLD WIDE WEB CONSORTIUM (W3C). Decentralized Identifiers (DIDs) v1.1. Candidate Recommendation Snapshot, 5 mar. 2026. Disponível em: https://www.w3.org/TR/did-1.1/. Acesso em: 8 nov. 2026. 
W3C+1

WORLD WIDE WEB CONSORTIUM (W3C). Bitstring Status List v1.0: Privacy-preserving status information for Verifiable Credentials. W3C Recommendation, 15 maio 2025. Disponível em: https://www.w3.org/TR/2025/REC-vc-bitstring-status-list-20250515/. Acesso em: 2 nov. 2026. 

NATIONAL INSTITUTE OF STANDARDS AND TECHNOLOGY (NIST). Digital Identity Guidelines. NIST SP 800-63-4. 2025. Disponível em: https://doi.org/10.6028/NIST.SP.800-63-4. Acesso em: 4 nov. 2026. 

NATIONAL INSTITUTE OF STANDARDS AND TECHNOLOGY (NIST). Digital Identity Guidelines: Identity Proofing and Enrollment. NIST SP 800-63A-4. 2025. Disponível em: https://doi.org/10.6028/NIST.SP.800-63A-4. Acesso em: 4 nov. 2026. 

NATIONAL INSTITUTE OF STANDARDS AND TECHNOLOGY (NIST). Digital Identity Guidelines: Authentication and Authenticator Management. NIST SP 800-63B-4. 2025. Disponível em: https://doi.org/10.6028/NIST.SP.800-63B-4. Acesso em: 2 nov. 2026. 

NATIONAL INSTITUTE OF STANDARDS AND TECHNOLOGY (NIST). Digital Identity Guidelines: Federation and Assertions. NIST SP 800-63C-4. 2025. Disponível em: https://doi.org/10.6028/NIST.SP.800-63C-4. Acesso em: 2 nov. 2026. 

LIANG, Junkai et al. SoK: Understanding zk-SNARKs: The Gap Between Research and Practice. Cryptology ePrint Archive, 2025/172, 2025. Disponível em: https://eprint.iacr.org/2025/172. Acesso em: 2 nov. 2026. 

INTERNET ENGINEERING TASK FORCE (IETF). Best Current Practice for OAuth 2.0 Security. RFC 9700, 2025. Disponível em: https://www.rfc-editor.org/rfc/rfc9700.html. Acesso em: 4 nov. 2026. 

RESCORLA, Eric. The Transport Layer Security (TLS) Protocol Version 1.3. RFC 9846. Internet Engineering Task Force, 2026. Disponível em: https://www.rfc-editor.org/rfc/rfc9846.html. Acesso em: 4 nov. 2026. 

NATIONAL INSTITUTE OF STANDARDS AND TECHNOLOGY (NIST). Implementing a Zero Trust Architecture: High-Level Document. NIST SP 1800-35. 2025. Disponível em: https://doi.org/10.6028/NIST.SP.1800-35. Acesso em: 30 out. 2026. 

REDIS LTD. EXPIRE. Redis Documentation. Disponível em: https://redis.io/docs/latest/commands/expire/. Acesso em: 4 nov. 2026. 
Docs

WORLD WIDE WEB CONSORTIUM (W3C). Web Content Accessibility Guidelines (WCAG) 2.2. W3C Recommendation, atualização de 12 dez. 2024. Disponível em: https://www.w3.org/TR/WCAG22/. Acesso em: 1 nov. 2026. 
W3C

WORLD WIDE WEB CONSORTIUM (W3C). Accessible Rich Internet Applications (WAI-ARIA) 1.3. W3C Working Draft, 4 jun. 2026. Disponível em: https://www.w3.org/TR/wai-aria-1.3/. Acesso em: 1 nov. 2026. 

GREEN SOFTWARE FOUNDATION. Software Carbon Intensity (SCI) Specification. Disponível em: https://greensoftware.foundation/standards/sci/. Acesso em: 28 out. 2026.

GREEN WEB FOUNDATION. Tools. Disponível em: https://www.thegreenwebfoundation.org/tools/. Acesso em: 29 out. 2026. 

NÚCLEO DE INFORMAÇÃO E COORDENAÇÃO DO PONTO BR (NIC.br). TIC Kids Online investiga, pela primeira vez, frequência do uso de plataformas digitais por crianças e adolescentes. 23 out. 2024. Disponível em: https://nic.br/noticia/releases/tic-kids-online-investiga-pela-primeira-vez-frequencia-do-uso-de-plataformas-digitais-por-criancas-e-adolescentes/. Acesso em: 24 out. 2026. 
