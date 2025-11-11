================================================================================
                    CALCULADORA CIENTÍFICA - GUIA DE INSTALAÇÃO
                           Windows e Linux
================================================================================

ÍNDICE:
1. Pré-requisitos
2. Instalação no Windows
3. Instalação no Linux
4. Como Abrir no VSCode
5. Solução de Problemas

================================================================================
1. PRÉ-REQUISITOS
================================================================================

PARA WINDOWS E LINUX:
- Node.js (versão 16 ou superior)
- npm (vem com Node.js)
- Um editor de texto (VSCode recomendado)

DOWNLOAD:
- Node.js: https://nodejs.org/ (escolha a versão LTS)
- VSCode: https://code.visualstudio.com/

VERIFICAR INSTALAÇÃO:
Abra o terminal/prompt e execute:
  node --version
  npm --version

Se aparecer um número de versão, está instalado corretamente.

================================================================================
2. INSTALAÇÃO NO WINDOWS
================================================================================

OPÇÃO A: INSTALAÇÃO AUTOMÁTICA (RECOMENDADO)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PASSO 1: Extrair o arquivo ZIP
  1. Clique com botão direito em "calculadora-cientifica.zip"
  2. Selecione "Extrair tudo..."
  3. Escolha a pasta de destino (ex: C:\Users\SeuUsuario\Desktop)
  4. Clique em "Extrair"

PASSO 2: Instalar dependências
  1. Abra a pasta extraída "calculadora-cientifica"
  2. Clique duas vezes em "install-windows.bat"
  3. Uma janela preta (terminal) abrirá
  4. Aguarde até aparecer "Instalação concluída com sucesso!"
  5. Pressione qualquer tecla para fechar

PASSO 3: Iniciar a calculadora
  1. Na pasta "calculadora-cientifica", clique duas vezes em "iniciar-desenvolvimento.bat"
  2. Uma janela preta abrirá
  3. Aguarde até aparecer "Local: http://localhost:5173"
  4. Abra seu navegador (Chrome, Firefox, Edge, etc)
  5. Acesse: http://localhost:5173
  6. Pronto! A calculadora está funcionando!

PARA PARAR O SERVIDOR:
  - Pressione Ctrl + C na janela preta do terminal
  - Ou feche a janela

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

OPÇÃO B: INSTALAÇÃO MANUAL (VIA TERMINAL)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PASSO 1: Extrair o arquivo ZIP
  (Mesmo que a Opção A - Passo 1)

PASSO 2: Abrir o Prompt de Comando
  1. Pressione Windows + R
  2. Digite: cmd
  3. Pressione Enter

PASSO 3: Navegar até a pasta do projeto
  1. No Prompt de Comando, digite:
     cd C:\caminho\para\calculadora-cientifica
     
     Exemplo:
     cd C:\Users\SeuUsuario\Desktop\calculadora-cientifica

PASSO 4: Instalar dependências
  1. Digite: pnpm install
  2. Se aparecer erro "pnpm: comando não encontrado", execute primeiro:
     npm install -g pnpm
  3. Aguarde a instalação completar

PASSO 5: Iniciar o servidor
  1. Digite: pnpm dev
  2. Aguarde até aparecer "Local: http://localhost:5173"

PASSO 6: Abrir no navegador
  1. Abra seu navegador
  2. Acesse: http://localhost:5173
  3. Pronto! A calculadora está funcionando!

PARA PARAR O SERVIDOR:
  - Pressione Ctrl + C no Prompt de Comando

================================================================================
3. INSTALAÇÃO NO LINUX
================================================================================

PASSO 1: Verificar se Node.js está instalado
  1. Abra o Terminal (Ctrl + Alt + T)
  2. Digite: node --version
  3. Se aparecer um número, pule para o Passo 3
  4. Se não aparecer nada, continue no Passo 2

PASSO 2: Instalar Node.js (se necessário)
  Para Ubuntu/Debian:
    sudo apt update
    sudo apt install nodejs npm

  Para Fedora/RHEL:
    sudo dnf install nodejs npm

  Para Arch:
    sudo pacman -S nodejs npm

  Após instalar, verifique:
    node --version
    npm --version

PASSO 3: Extrair o arquivo ZIP
  1. Abra o gerenciador de arquivos
  2. Navegue até o arquivo "calculadora-cientifica.zip"
  3. Clique com botão direito e selecione "Extrair aqui"
  4. Ou use o terminal:
     unzip calculadora-cientifica.zip

PASSO 4: Abrir o Terminal na pasta do projeto
  1. Abra o Terminal
  2. Digite:
     cd ~/calculadora-cientifica
     
     (ou o caminho correto se extraiu em outro local)

PASSO 5: Instalar dependências
  1. Digite: pnpm install
  2. Se aparecer erro "pnpm: comando não encontrado", execute primeiro:
     npm install -g pnpm
  3. Aguarde a instalação completar

PASSO 6: Iniciar o servidor
  1. Digite: pnpm dev
  2. Aguarde até aparecer "Local: http://localhost:5173"

PASSO 7: Abrir no navegador
  1. Abra seu navegador (Firefox, Chrome, etc)
  2. Acesse: http://localhost:5173
  3. Pronto! A calculadora está funcionando!

PARA PARAR O SERVIDOR:
  - Pressione Ctrl + C no Terminal

================================================================================
4. COMO ABRIR NO VSCODE
================================================================================

WINDOWS:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PASSO 1: Abrir VSCode
  1. Clique no ícone do VSCode na área de trabalho ou menu Iniciar

PASSO 2: Abrir a pasta do projeto
  1. Clique em "File" (Arquivo) no menu superior
  2. Selecione "Open Folder" (Abrir Pasta)
  3. Navegue até a pasta "calculadora-cientifica"
  4. Clique em "Select Folder" (Selecionar Pasta)

PASSO 3: Abrir o Terminal Integrado
  1. Pressione Ctrl + ` (backtick/acento grave)
  2. Ou vá em Terminal → New Terminal (Terminal → Novo Terminal)

PASSO 4: Instalar dependências
  1. No terminal do VSCode, digite: pnpm install
  2. Aguarde a conclusão

PASSO 5: Iniciar o servidor
  1. Digite: pnpm dev
  2. Clique no link "http://localhost:5173" que aparecer
  3. Ou copie e cole no navegador

PASSO 6: Editar o código
  1. Na esquerda, você verá a estrutura de pastas
  2. Clique em "client/src/components/Calculator.tsx" para ver o código
  3. Faça suas alterações
  4. O servidor atualizará automaticamente

LINUX:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

(Os passos são idênticos ao Windows acima)

PASSO 1: Abrir VSCode
  1. Abra o Terminal
  2. Digite: code calculadora-cientifica
  3. VSCode abrirá com a pasta do projeto

OU:
  1. Abra VSCode normalmente
  2. Clique em "File" → "Open Folder"
  3. Navegue até a pasta "calculadora-cientifica"
  4. Clique em "Open" (Abrir)

PASSOS 3-6: Mesmos que Windows acima

================================================================================
5. SOLUÇÃO DE PROBLEMAS
================================================================================

PROBLEMA: "pnpm: comando não encontrado"
SOLUÇÃO:
  npm install -g pnpm

PROBLEMA: "node: comando não encontrado"
SOLUÇÃO:
  - Instale Node.js em https://nodejs.org/
  - Reinicie o terminal/prompt após instalar

PROBLEMA: "Porta 5173 já está em uso"
SOLUÇÃO:
  Opção 1: Feche outros programas que usam essa porta
  Opção 2: Use uma porta diferente
    pnpm dev -- --port 5174

PROBLEMA: Erro ao executar install-windows.bat
SOLUÇÃO:
  1. Abra o PowerShell como Administrador
  2. Clique com botão direito no PowerShell
  3. Selecione "Executar como administrador"
  4. Navegue até a pasta e execute novamente

PROBLEMA: Dependências não instaladas corretamente
SOLUÇÃO:
  1. Delete a pasta "node_modules"
  2. Delete o arquivo "pnpm-lock.yaml"
  3. Execute: pnpm install

PROBLEMA: A aplicação não abre no navegador
SOLUÇÃO:
  1. Verifique se o terminal mostra "Local: http://localhost:5173"
  2. Copie e cole manualmente no navegador
  3. Tente em outro navegador (Chrome, Firefox, Edge)

PROBLEMA: Mudanças no código não aparecem
SOLUÇÃO:
  1. Verifique se o servidor está rodando (terminal mostra "Local: ...")
  2. Pressione F5 no navegador para recarregar
  3. Limpe o cache: Ctrl + Shift + Delete (em alguns navegadores)

================================================================================
COMANDOS ÚTEIS
================================================================================

WINDOWS (Prompt de Comando):
  cd C:\caminho\para\pasta          - Mudar de pasta
  dir                               - Listar arquivos
  pnpm install                      - Instalar dependências
  pnpm dev                          - Iniciar servidor
  pnpm build                        - Compilar para produção
  Ctrl + C                          - Parar o servidor

LINUX (Terminal):
  cd ~/caminho/para/pasta           - Mudar de pasta
  ls                                - Listar arquivos
  pnpm install                      - Instalar dependências
  pnpm dev                          - Iniciar servidor
  pnpm build                        - Compilar para produção
  Ctrl + C                          - Parar o servidor

================================================================================
ESTRUTURA DO PROJETO
================================================================================

calculadora-cientifica/
├── client/                        - Frontend (React)
│   ├── src/
│   │   ├── components/
│   │   │   └── Calculator.tsx     - Componente principal da calculadora
│   │   ├── pages/
│   │   │   └── Home.tsx           - Página inicial
│   │   ├── App.tsx                - Componente raiz
│   │   └── main.tsx               - Ponto de entrada
│   └── public/                    - Arquivos estáticos
├── package.json                   - Dependências do projeto
├── vite.config.ts                 - Configuração do Vite
├── install-windows.bat            - Script de instalação (Windows)
├── iniciar-desenvolvimento.bat    - Script de inicialização (Windows)
├── README.md                      - Leia-me
├── INSTALACAO-WINDOWS.md          - Guia detalhado para Windows
├── userGuide.md                   - Guia do usuário
├── GUIA-INSTALACAO.txt            - Este arquivo
└── todo.md                        - Lista de funcionalidades

================================================================================
PRÓXIMOS PASSOS
================================================================================

1. EXPLORAR A CALCULADORA
   - Teste as operações básicas: 5 + 3 = 8
   - Teste funções científicas: sin(90) = 1
   - Use o teclado para digitar números

2. PERSONALIZAR O PROJETO
   - Edite cores em: client/src/index.css
   - Edite o layout em: client/src/components/Calculator.tsx
   - Altere o título em: client/src/const.ts

3. APRENDER MAIS
   - Leia: README.md
   - Leia: userGuide.md
   - Explore o código em: client/src/

4. COMPILAR PARA PRODUÇÃO
   - Execute: pnpm build
   - Arquivos compilados estarão em: dist/

================================================================================
DÚVIDAS FREQUENTES
================================================================================

P: Posso usar a calculadora offline?
R: Sim! Após compilar com "pnpm build", você pode abrir os arquivos em dist/

P: Como mudo a cor da calculadora?
R: Edite o arquivo "client/src/index.css" e altere as cores CSS

P: Posso adicionar novas funções matemáticas?
R: Sim! Edite "client/src/components/Calculator.tsx" e use a biblioteca mathjs

P: Qual é a diferença entre pnpm dev e pnpm build?
R: dev = servidor de desenvolvimento com auto-reload
   build = compilação para produção (arquivos otimizados)

P: Preciso de internet para usar a calculadora?
R: Não! Após "pnpm build", é totalmente offline

================================================================================
SUPORTE E DOCUMENTAÇÃO
================================================================================

Para mais informações:
- README.md - Visão geral do projeto
- userGuide.md - Como usar a calculadora
- INSTALACAO-WINDOWS.md - Guia detalhado para Windows
- GUIA-INSTALACAO.txt - Este arquivo

================================================================================
