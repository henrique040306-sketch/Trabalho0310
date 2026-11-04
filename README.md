# Trabalho0310

**Integrantes:**
- Henrique Nunes Peixoto (RA: 60300275)
- Rodrigo Valim Junior (RA: 60000597)

---

## Etapa 1 - Base do Projeto Flutter e Telas de Autenticação

### O que foi feito
- Configuração da estrutura base do projeto em Flutter com gerenciamento de rotas.
- Criação das telas de Login e Cadastro baseadas nos requisitos de autenticação por e-mail/senha do Firebase Auth.
- Implementação de validações de campos (formato de e-mail, senha com mínimo de 6 caracteres e confirmação de senha).
- Levantamento de requisitos e Histórias de Usuário documentados na Wiki do repositório.

### Prints das Telas
| Tela de Login | Tela de Cadastro | Validação de Erros |
| :---: | :---: | :---: |
| ![Login](prints/login.png) | ![Cadastro](prints/cadastro.png) | ![Validação](prints/validacao.png) |

### Vídeo de Apresentação
🔗 [Assistir ao vídeo da Etapa 1 no YouTube](https://youtu.be/SEU_LINK_AQUI)

### Declaração de Uso de IA
- **Usamos IA nesta etapa?** Sim (Gemini).
- **Para quê:** Levantamento da estrutura de campos compatíveis com o Firebase Auth (`email`, `password`, `displayName`) e auxílio na sintaxe dos widgets de validação (`TextFormField` com `FormState`).
- **O que a IA sugeriu:** Sugeriu a divisão modular em arquivos (`main.dart`, `login_page.dart` e `cadastro_page.dart`) com navegação nomeada por rotas.
- **O que alteramos ou aprendemos:** Adaptamos as regras de validação para os requisitos da disciplina, aprendemos a manipular formulários com chaves globais (`GlobalKey<FormState>`) e a estruturar as histórias de usuário na Wiki.
