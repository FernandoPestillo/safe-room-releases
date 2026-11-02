# Safe Room — downloads

Pré-lançamento para um grupo inicial de amigos. Este repositório contém somente instaladores, assinaturas, manifesto de atualização e orientações. O código-fonte permanece privado.

Os primeiros artefatos estão em homologação e serão disponibilizados em **Releases**, identificados como pré-lançamento. Não é uma versão stable nem uma afirmação de homologação completa em dois computadores.

## Windows

O instalador é para Windows x64 com WebView2. O usuário não precisa instalar Node.js, Rust, Docker ou PostgreSQL. A API pública já vem configurada no aplicativo: `https://api.safe-room.tech`.

Após instalar, use **Criar conta**, informe nome, email, senha e confirmação. A senha precisa ter pelo menos 8 caracteres, uma maiúscula, uma minúscula e um número de 0 a 9; símbolos são opcionais. O email ainda não é verificado e não há recuperação por email implementada.

Na tela principal, crie um servidor ou selecione **Entrar em servidor** e informe o convite. Escolha um canal de texto ou voz. Câmera e compartilhamento exigem seleção e confirmação locais.

## Limitações conhecidas

- Recuperação automática do microfone USB pode falhar; use **reiniciar microfone** nas configurações. Correção adiada.
- O runtime testado não forneceu áudio do sistema ao compartilhar a tela. Não há capturador nativo de áudio por aplicativo nesta entrega.
- Testes completos em dois Windows físicos, redes distintas e Windows limpo continuam pendentes.
- Não há backup externo nem proteção adequada contra perda definitiva dos dados. Não se declara recuperação de desastres. O responsável decidiu prosseguir com este pré-lançamento aceitando esse risco.
- A assinatura do updater verifica autenticidade do pacote; não equivale a Authenticode ou à identificação do editor pelo Windows.

O updater assinado está sendo homologado antes da disponibilização final. Não instalar atualizações durante chamadas ou compartilhamentos sem antes encerrá-los.

Não envie senhas, tokens, arquivos de perfil ou capturas privadas em relatos de falha.
