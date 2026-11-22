CARECAS 3D — SITE INICIAL
Domínio: carecas3d.com.br

O QUE ESTÁ INCLUÍDO
- Landing page responsiva em português.
- Identidade visual preto, grafite, branco e laranja.
- Logomarca enviada pelo cliente.
- Seções: início, serviços, portfólio, materiais, sobre e contato.
- Estrutura inicial do painel administrativo Decap CMS em /admin/.

IMPORTANTE SOBRE O PAINEL
O painel administrativo está preparado, mas ainda NÃO está pronto para autenticar. Para que o login e as alterações funcionem, é necessário publicar o projeto em um repositório GitHub e configurar a autenticação OAuth do GitHub. O arquivo admin/config.yml contém um endereço de repositório de exemplo que deverá ser substituído. Não publique credenciais ou senhas dentro dos arquivos do site.

PUBLICAÇÃO NA CLOUDFLARE PAGES (VISÃO GERAL)
1. Crie/acesse uma conta GitHub e crie um repositório vazio chamado carecas3d-site.
2. Envie todos os arquivos desta pasta para a branch main do repositório.
3. No Cloudflare, vá a Workers & Pages > Create > Pages > Connect to Git.
4. Conecte o GitHub e selecione carecas3d-site.
5. Framework preset: None. Build command: deixe vazio. Build output directory: / (ou .).
6. Publique. Depois, em Custom domains, adicione carecas3d.com.br e www.carecas3d.com.br conforme desejar.
7. Para ativar /admin/, será necessário concluir a configuração OAuth descrita abaixo e substituir SEU-USUARIO/SEU-REPOSITORIO no admin/config.yml pelo usuário e nome reais do repositório GitHub.

PAINEL CMS
O Decap CMS permite cadastrar trabalhos com título, descrição, fotografia, categoria e opção de publicação. O conteúdo salvo é versionado no GitHub. A autenticação GitHub OAuth exige um provedor OAuth seguro (por exemplo, um Cloudflare Worker configurado com as credenciais de um GitHub OAuth App). Essa etapa depende de criar o OAuth App e cadastrar os segredos no ambiente Cloudflare; não é possível concluir sem acesso e autorização do titular das contas.

CONTATO
WhatsApp informado: 55 11 98321-8537. O número já está configurado em content/site.json; os botões de orçamento abrirão uma conversa com a mensagem inicial.

ANTES DE DIVULGAR
- Trocar os cartões demonstrativos do portfólio por fotografias reais.
- Informar telefone/WhatsApp, Instagram e e-mail.
- Revisar a descrição institucional e materiais realmente disponíveis.
- Testar formulário/links, visualização em celular e domínio HTTPS.

COMO O CONTEÚDO DO PAINEL APARECE NO SITE
Depois que o CMS estiver autenticado, a galeria editada em content/portfolio.json é carregada automaticamente na seção Trabalhos. As configurações em content/site.json atualizam o texto de apresentação, WhatsApp, Instagram e e-mail. Se a galeria estiver vazia, o site mantém os cartões demonstrativos.
