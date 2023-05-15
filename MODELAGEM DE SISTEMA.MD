MODELAGEM DE SISTEMA

Diagrama de Casos de Uso:

Jogador: Registro de usuário, login, pesquisa de partidas, criação de partida, confirmação de participação, envio de mensagens, avaliação de outros jogadores.
Criador de Partida: Criação de partida, gerenciamento de detalhes da partida, visualização de confirmações dos jogadores.
Sistema: Autenticação de usuário, notificações de novas mensagens e atualizações de partida.
Diagrama de Classes:

Jogador: Atributos como nome, e-mail, senha, foto, posição em campo, avaliações. Métodos como criar partida, confirmar participação, enviar mensagens.
Partida: Atributos como localização, data, horário, número de jogadores necessários, confirmações dos jogadores. Métodos como gerenciar detalhes da partida.
Mensagem: Atributos como remetente, destinatário, conteúdo, data/hora. Métodos para envio e leitura de mensagens.
Avaliação: Atributos como jogador avaliado, jogador avaliador, pontuação, comentário.
Diagrama de Sequência:

Registro de Usuário: Jogador envia informações de registro -> Sistema verifica e armazena informações no banco de dados.
Login: Jogador envia credenciais -> Sistema verifica credenciais e autentica o jogador.
Criação de Partida: Jogador cria uma partida -> Sistema armazena os detalhes da partida no banco de dados.
Confirmação de Participação: Jogador confirma participação em uma partida -> Sistema atualiza a lista de confirmações da partida.
Envio de Mensagens: Jogador envia mensagem -> Sistema registra a mensagem e notifica o destinatário.
Avaliação de Jogadores: Jogador avalia outro jogador após a partida -> Sistema armazena a avaliação e atualiza a pontuação do jogador avaliado.
Diagrama de Componentes:

Interface do Usuário: Responsável pela interação do usuário com o aplicativo.
Controladores: Gerenciam a lógica de negócio, processando as requisições dos usuários e realizando operações no banco de dados.
Banco de Dados: Armazena as informações dos jogadores, partidas, mensagens e avaliações.
Serviços Externos: Integrações com serviços de autenticação, notificações e pagamentos, caso sejam implementados.
