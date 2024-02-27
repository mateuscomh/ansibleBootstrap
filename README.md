# ansibleBootstrap
#####
- Precisa que usuário já esteja criado
- Precisa que usuário tenha permissoes de sudo



#install
sudo apt update
sudo apt install ansible




meu_projeto_ansible/
│
├── inventário/
│   └── hosts                  # Arquivo de inventário com os hosts a serem gerenciados
│
├── playbooks/
│   ├── provisionar.yml        # Playbook para provisionar a máquina
│   └── configurar.yml         # Playbook para configurar a máquina
│
├── roles/
│   ├── comum/                 # Role com tarefas comuns a todos os hosts
│   │   ├── tasks/
│   │   │   └── main.yml       # Tarefas comuns
│   │   └── defaults/
│   │       └── main.yml       # Variáveis padrão para esta role
│   │
│   └── meu_aplicativo/        # Role para configurar seu aplicativo específico
│       ├── tasks/
│       │   └── main.yml       # Tarefas específicas do seu aplicativo
│       └── defaults/
│           └── main.yml       # Variáveis padrão para esta role
│
└── arquivos/
    └── arquivo_de_configuracao.txt  # Arquivos necessários para configuração
