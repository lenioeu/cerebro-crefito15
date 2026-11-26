# Segundo cérebro — Procuradoria Jurídica do CREFITO-15

Este arquivo é o mapa. Leia-o primeiro e depois vá direto à pasta da tarefa.

## Quem sou

Lenio Goularte, chefe da Procuradoria Jurídica do **CREFITO-15** (autarquia federal, conselho
profissional de Fisioterapia e Terapia Ocupacional). A Procuradoria emite pareceres e ofícios,
atua em ações civis públicas e acompanha processos administrativos.

O Conselho usa pelo menos dois sistemas administrativos: **Implanta** para as atividades-fim
(fiscalização, anuidade, parcelamento, inscrição, reembolso) e **SEI** para o resto (licitações,
contratos, diárias e passagens, ofícios). A Procuradoria é demandada e emite pareceres nos dois.
Ver `01 Procuradoria/Sistemas do Conselho.md`. O Claude não tem acesso a nenhum dos dois:
o que vier deles chega por documento exportado ou anexado.

O escritório Goularte Filho Advocacia tem vault separado (repositório `segundo-cerebro`).
**Nunca misture os dois**, nem use o Órion CRM para assuntos do Conselho.

## Mapa

| Pasta | O que tem | Quando ler |
|---|---|---|
| `00 Inbox/` | capturas rápidas | na revisão |
| `01 Procuradoria/` | atribuições, fluxos com outros setores, sistemas (SEI, Implanta) | contexto geral |
| `02 Padrões/` | parecer, ofício, peças judiciais; `Modelos/` tem os .docx-base | **antes de todo documento** |
| `10 Teses/` | posições da Procuradoria por tema | pareceres e ações |
| `20 Procedimentos/` | como fazer cada rotina (SEI, ações civis públicas, prazos) | ao executar a rotina |
| `30 Recursos/` | legislação e normas do sistema COFFITO/CREFITO, jurisprudência | pesquisa |
| `90 Modelos de nota/` | modelos para notas novas | ao criar nota |
| `99 Arquivo/` | o que saiu de uso | quase nunca |
| `.claude/skills/` | `/peca-judicial`, `/parecer`, `/aprendizado` | quando o comando é chamado |

## Regras que valem sempre

1. **O que não entra aqui:** conteúdo de processo ético-disciplinar (sigiloso), dados pessoais de
   profissionais, denunciantes ou servidores, e cópia de autos. Refira-se a um processo pelo
   **número SEI** (ou pelo identificador no Implanta) e pelo tema.
2. **Fonte oficial são os sistemas do Conselho (SEI e Implanta).** Este vault guarda o raciocínio
   e o modelo, não o documento oficial.
3. **Revisão humana.** Tudo o que o Claude produz é minuta até eu revisar e assinar no SEI.
4. **Aprendizados.** Antes de executar, leia `Aprendizados.md`. Quando eu corrigir algo, registre
   com `/aprendizado`.
5. **Padrões** de `02 Padrões/` prevalecem sobre qualquer hábito seu. Cargo do Lenio em toda
   assinatura: **Chefe da Procuradoria CREFITO-15**.
6. **Jurisprudência e normas:** nunca cite julgado, resolução ou artigo sem conferir na fonte oficial
   (JuriBase `verificar_citacao`, site do tribunal, site do COFFITO, Planalto). Se não achar, diga.
7. **Dúvida sobre fato:** pergunte.

## Convenções

- Nomes de nota em português, com acento.
- Ligações com `[[Nome da nota]]`.
- Propriedades mínimas:

```yaml
tipo: tese | procedimento | estrutura-de-documento | recurso
status: rascunho | em-uso | superado
atualizado: AAAA-MM-DD
sei: número do processo SEI de referência (opcional)
```

- Formato de cada entrada em `Aprendizados.md`:

```markdown
## AAAA-MM-DD — título curto
- **Errado:** o que foi feito
- **Certo:** como deve ser feito a partir de agora
- **Por quê:** motivo (quando eu disser)
```
