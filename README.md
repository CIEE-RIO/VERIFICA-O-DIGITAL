# Comparador de Planilhas CPF/CNPJ

Aplicação web para comparar duas planilhas usando CPF ou CNPJ como chave. Todo o processamento ocorre no navegador: os arquivos não são enviados para um servidor.

## Funcionalidades

- Importação de `.xlsx`, `.xls` e `.csv`.
- Seleção da aba e da coluna-chave em cada arquivo.
- Comparação de CPF/CNPJ com ou sem pontuação.
- Identificação de registros exclusivos de cada base e registros presentes nas duas.
- Aviso de chaves duplicadas e linhas sem chave.
- Busca, filtros e exportação do resultado completo para Excel.
- Layout responsivo para computador e celular.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e envie todos os arquivos deste projeto para a branch `main`.
2. Abra **Settings > Pages** no repositório.
3. Em **Build and deployment > Source**, selecione **GitHub Actions**.
4. A publicação será executada automaticamente. O endereço aparecerá na aba **Actions** e em **Settings > Pages**.

O fluxo de publicação está pronto em `.github/workflows/deploy-pages.yml`.

## Executar no computador

```bash
npm install
npm run dev
```

Para validar especificamente a versão estática do GitHub Pages:

```bash
npm run build:pages
```

Os arquivos finais serão criados em `github-pages-dist`.
