# Trabalho Organização

Base local para organizar uma operação de vendas na Shopee e no Mercado Livre.
Este projeto separa procedimentos, modelos reutilizáveis e dados operacionais para
reduzir erros, facilitar auditorias e permitir automações futuras.

> Estado inicial: estrutura e documentação publicadas sem credenciais ou dados de
> clientes. As integrações operacionais ainda serão implementadas gradualmente.

## Estrutura

| Pasta | Finalidade | Pode ir para o Git? |
| --- | --- | --- |
| `rotina-diaria/` | Checklists de abertura, acompanhamento e encerramento | Sim, sem dados pessoais |
| `anuncios/` | Padrões de títulos, descrições, categorias e revisão | Sim, nos modelos e guias |
| `imagens/` | Orientações de produção e organização das mídias | Somente guias e arquivos leves aprovados |
| `produtos/` | Regras de cadastro, SKU, preço, estoque e catálogo | Somente modelos sem dados sensíveis |
| `pedidos/` | Fluxo operacional de pedidos, envio, troca e devolução | Somente procedimentos e modelos vazios |
| `relatorios/` | Definições de indicadores e periodicidade | Somente documentação e modelos vazios |
| `automacoes/` | Código e documentação de integrações futuras | Sim; segredos e estado local nunca |
| `modelos/` | Textos e arquivos reutilizáveis | Sim, após revisão de dados pessoais |
| `arquivo/` | Índice para material encerrado ou histórico | Somente índice; conteúdo operacional não |
| `docs/` | Políticas gerais do projeto | Sim |

As pastas locais `work/` e `outputs/` são áreas transitórias do Codex e estão
ignoradas pelo Git.

## Convenções

- Arquivos: `aaaa-mm-dd_assunto_descricao.ext` quando houver data.
- SKUs: adote um padrão estável antes de cadastrar produtos; não reutilize códigos.
- Dados reais exportados dos marketplaces ficam fora do Git.
- Credenciais devem existir apenas em variáveis de ambiente ou em um gerenciador de
  segredos. Use `.env.example` para documentar nomes, nunca valores reais.
- Antes de cada commit, execute `git status` e confirme que não há dados pessoais,
  chaves, planilhas operacionais, etiquetas ou mídias pesadas.

## Fluxo sugerido

1. Consulte `rotina-diaria/README.md` e registre exceções fora do repositório.
2. Prepare catálogo em `produtos/` usando somente cópias locais dos modelos.
3. Produza anúncios conforme `anuncios/README.md` e imagens conforme
   `imagens/README.md`.
4. Trate pedidos seguindo `pedidos/README.md`.
5. Gere indicadores conforme `relatorios/README.md`, mantendo exportações reais fora
   do Git.
6. Mova itens concluídos para armazenamento operacional e mantenha apenas um índice
   anonimizado em `arquivo/`.

## Configuração local futura

Quando houver uma automação definida:

1. copie `automacoes/.env.example` para `automacoes/.env`;
2. preencha os valores apenas na máquina local;
3. confirme que `.env` continua ignorado;
4. use contas de teste e permissões mínimas antes de acessar a operação real.

## GitHub

Esta base pertence ao repositório
[`Lucasbn1909/Trabalhos`](https://github.com/Lucasbn1909/Trabalhos), dentro da pasta
`trabalho-organizacao/`. Consulte `docs/GITHUB.md` para as regras de publicação e
sincronização local.
