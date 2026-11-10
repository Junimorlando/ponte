# CLAUDE.md — PONTE

Mapa curto para o agente. Leia o que a tarefa pede, não tudo "por via das dúvidas".
Base: o documento de entrada "PONTE para o Juninho", de 09/11/2026. Ele é interno e
fica fora do git. Quando este arquivo e o Leo discordarem, vale o Leo.

## Quem sou eu aqui

- **Orlando (Juninho):** sócio da PONTE. Cuida de vendas, operação e trabalho com agentes de IA.
- **Leo (Leo Resende):** fundador e dono único do código, na organização PONTETECH do GitHub. Contato: leo@ponte.dev.
- Fale comigo em **português do Brasil** e em linguagem simples. Não sou programador: explique cada termo técnico na primeira vez em que ele aparecer.
- A clínica odontológica (Shine / Dr. Orlando Reis) é **outro negócio**. Não misture os dois.
- A frente de cinema fica fora deste arquivo. Ela é com o Leo.

## A PONTE em poucas linhas

- **Tese:** "Software com IA para quem ainda trabalha no papel."
- **Na prática:** ferramentas simples para profissões que o software deixou de lado. "A IA faz o braçal. O especialista decide." Nenhum produto substitui o profissional.
- **A IA não inventa:** na dúvida, deixa o campo vazio ou marca "incerto". O que o agente produz nasce como rascunho, e uma pessoa aprova.
- **Rodapé:** todo produto leva "Powered by PONTE".
- **Site:** https://ponte.dev, institucional. Projeto de cliente fica em endereço próprio na Netlify, com noindex.
- **Peças que se repetem:** WhatsApp oficial da Meta, Supabase, IA da Anthropic, Whisper para áudio, Netlify/Vercel e o Jev (TypeSafe).

## Frentes (só nome e estágio)

Números, preços, nomes de cliente e prazos ficam no documento interno, não aqui.

| Frente | O que é | Estágio | No ar para cliente? |
|---|---|---|---|
| GIZ | assistente acadêmico pelo WhatsApp para docentes | no ar, **sem cliente pagante** | sim (app, banco e `main`) |
| ili | app para corretor de imóveis (repositório `ponte-imo`) | pagando | sim |
| NoCampo | assistente de lavoura pelo WhatsApp | protótipo | não |
| Lê e Conta | leitura e escrita para a educação inclusiva, 3º ao 5º ano | protótipo | sim (páginas) |
| PONTE.TUR | operação de agência de turismo (serviço dedicado) | no ar | sim |
| São Mateus II | gestão de fazenda por satélite, drone e WhatsApp | proposta | sim (sites) |
| Painel do leite | demonstração com dados simulados | demonstração | sim |
| Pousada Anamã | sistema e site de pousada | código pronto, fora do ar | não |
| Kit de Natal do Empório | kit de café em consignação | proposta | sim (proposta) |
| Site da GPM | site de escritório de advocacia e proposta de mídia | no ar | sim |
| Overhead / NEAR | hackathons | competição | público: passa pelo Leo |

**Largados (não reabra sem o Leo):** CLARA café (não sugira "Clara"), marca Santa Rosa, DIV Fund, Talhão e apps-rural.
**Parados:** Vet., ATER e PONTE_GRÃO.

## Regras da casa

**Sigilo (regra de ouro).**
- Repositório guarda **só código**.
- Nunca vão para o GitHub: conteúdo de cliente, planilha com números, auditoria, `.env`, chave, token, senha, dado pessoal ou dado de pagamento.
- Material de cliente no Drive também é sigiloso: não compartilhe nem mude quem vê.
- Se um segredo vazar: primeiro troque a credencial no sistema real, depois tire do git, depois avise o Leo.
- "Na dúvida, não commita e fala com o Leo."

**Chaves e senhas.**
- Ficam no Keychain do Mac, nunca em documento nem na conversa.
- Quando o agente precisar de uma chave, quem põe no lugar sou eu.

**Números internos** (custo, margem, valor da empresa, termos do aporte) nunca saem para cliente, investidor ou parceiro, nem em pedaços. Cliente nunca vê custo nem margem.

**Não diga** que o GIZ tem cliente pagando.

## Quem aprova o quê

- **No dia a dia, aprovo eu:** rascunho, pesquisa, teste, arquivo novo, commit, material interno e proposta nova.
- **Passa pelo Leo:**
  - o que mexe no que já está no ar para cliente: o GIZ em produção (a `main` do GIZ publica sozinha), os sites publicados e qualquer banco de produção;
  - o que vai para investidor: os decks, o one-pager e o material do Founders Club.
- Um OK vale para uma ação, não para as seguintes.
- Quando uma trava perguntar e a decisão for do Leo, **espere**. Não procure outro caminho para o mesmo efeito.
- Artifact privado não conta como publicar. Compartilhar o link já conta.

## Como trabalhar (playbook: ambiente → evidência → fluxo)

1. **Contrato antes de começar:** toda tarefa com entrega tem tarefa · insumos · entrega · restrições · `pronto_quando`. O `pronto_quando` são 2 a 5 critérios conferíveis, que falham hoje. Se não der para escrever o critério, pergunte.
2. **Pronto só com prova mostrada:** saída de comando, teste passando, arquivo que abre, link que responde. "Deve funcionar" não é prova.
3. **Até 3 tentativas.** Se o resultado se repetir, pare e me traga: falhou · esperado · observado · escopo · becos tentados.
4. **Quem produz não aprova:** o que sai para alguém passa por revisão de um subagente em contexto separado.
5. **Memória em arquivo:** o que atravessa sessões vai para um registro com objetivo · tentado · descoberto · próximo · nunca. Segredo nunca entra nele.
6. **Nunca:** `--no-verify`, teste desligado, verificador editado para passar ou regra em CAIXA ALTA como correção.
7. **Scripts de publicação:** rode primeiro sem `--ok` (só mostra o que mudaria). O `--ok` publica e passa pela regra de aprovação.

## Marca e tom

- **Nome:** PONTE, em maiúsculas. Na tríade e no bot, "GIZ". Os materiais publicados ainda usam "Giz".
- **Logo:** o selo preto horizontal, com barras brancas e "PONTE". O "P" no quadrado vermelho é só ícone de app. Os arquivos estão em Meu Drive/PONTE/01_Marca.
- **Visual:** só versão clara, desde 01/11/2026. Fontes do site: Raleway (títulos) e IBM Plex Mono (texto). Fundo creme `#fff8e7`, tinta `#0f1923`, destaque âmbar `#c68a14`.
- **Tom:** português direto, sem enchimento. "Mostre o dado, não o adjetivo."
- **Proibido:** "revolucionar", "transformar", "potencializado por IA", "o futuro de" e emoji decorativo.
- **Sem gênero** no GIZ e no deck: "docente", "quem orienta", "coordenação".
- **Demonstração** usa dados fictícios, sem nome real de pessoa ou instituição.

## Onde fica cada coisa

- **Código:** GitHub, organização **PONTETECH**, privada (acesso por convite do Leo). Repositórios: `ponte-dev`, `handbook`, `ponte-giz`, `ponte-imo`, `nocampo`, `ponte-tur`, `PONTE_SMATEUS` e outros.
- **Playbook completo:** doc 11 do `PONTETECH/handbook`, no ramo `docs/playbook-agentes-ia`.
- **Drive:** Meu Drive/PONTE (01_Marca, 02_Apresentações, 05_Documentos). O acesso é com o Leo.
- **Este repositório** (`Junimorlando/ponte`) é pessoal. Ele guarda só este mapa e notas sem sigilo.
- **Cada projeto tem o próprio CLAUDE.md:** leia antes de mexer nele. O do projeto vale por cima deste.
