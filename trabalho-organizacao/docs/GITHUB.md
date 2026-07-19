# Integração com o GitHub

Este projeto é mantido no repositório
[`Lucasbn1909/Trabalhos`](https://github.com/Lucasbn1909/Trabalhos), na branch `main`,
dentro da pasta `trabalho-organizacao/`.

Antes de cada publicação:

1. revisar todos os arquivos com `git status`;
2. executar uma ferramenta de detecção de segredos;
3. confirmar que não há dados de clientes, pedidos, etiquetas ou exportações;
4. criar um commit com mensagem objetiva;
5. enviar as alterações somente após revisar a lista final de arquivos.

Exemplo de configuração para uma cópia local nova:

```text
git clone https://github.com/Lucasbn1909/Trabalhos.git
cd Trabalhos
git status
```

Não grave tokens em arquivos nem na URL do remoto. Use a autenticação segura do
GitHub disponível na máquina.
