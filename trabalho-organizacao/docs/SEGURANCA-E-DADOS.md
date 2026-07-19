# Segurança e dados

- Não versionar nomes, endereços, telefones, documentos, e-mails ou identificadores
  de compradores.
- Não versionar etiquetas, notas fiscais, comprovantes, conversas ou exportações dos
  marketplaces.
- Remover ou anonimizar dados antes de criar exemplos para documentação.
- Manter tokens, cookies, chaves de API e senhas fora do projeto.
- Revogar e substituir imediatamente qualquer segredo exposto por engano; apagar o
  arquivo em um commit posterior não remove o segredo do histórico.
- Revisar acessos e permissões de integrações periodicamente.

O `.gitignore` reduz acidentes, mas não substitui a revisão antes do commit.
