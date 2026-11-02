# Safe Room — downloads

Pré-lançamento para um grupo inicial de amigos. Este repositório contém somente instaladores, assinaturas, manifesto de atualização e orientações. O código-fonte permanece privado.

**Versão atual: 0.5.2 — pré-lançamento público.** [Baixar instalador Windows x64](https://github.com/FernandoPestillo/safe-room-releases/releases/download/preview/Safe-Room-Windows-x64-setup.exe) · [Notas e assinatura da versão](https://github.com/FernandoPestillo/safe-room-releases/releases/tag/v0.5.2). O download é público e não exige conta GitHub. Não é uma versão stable nem uma afirmação de homologação completa em dois computadores.

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

O pacote e o manifesto assinados estão disponíveis no canal preview. Para atualizar pelo aplicativo, abra **Configurações → Atualizações → Verificar**, confira as notas, baixe e escolha **Instalar e reiniciar**. Encerre chamadas e compartilhamentos antes da instalação. A atualização instalada 0.5.1 → 0.5.2 foi exercitada pelo aplicativo, com sessão e histórico preservados. Isso não substitui os testes físicos e cenários prolongados ainda pendentes.

Não envie senhas, tokens, arquivos de perfil ou capturas privadas em relatos de falha.
