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
<img width="345" height="750" alt="image" src="https://github.com/user-attachments/assets/0f218347-ea94-48b6-a428-460a8084cb69" />
<img width="356" height="759" alt="image" src="https://github.com/user-attachments/assets/2b6336da-6b8d-4e7c-a8fe-809c6cdcbb0c" />
<img width="350" height="753" alt="image" src="https://github.com/user-attachments/assets/9c6ee77a-0be1-4ba3-a32e-58b672156cd8" />
<img width="347" height="756" alt="image" src="https://github.com/user-attachments/assets/47e79a79-90cb-43a4-b3b1-1c3d455d7efd" />
<img width="353" height="757" alt="image" src="https://github.com/user-attachments/assets/89165ada-b65d-4320-8da6-54e2876edaf4" />

### Vídeo de Apresentação
🔗 [Assistir ao vídeo da Etapa 1 no YouTube](https://youtu.be/FNEiWZ_jmEw)

### Declaração de Uso de IA
- **Usamos IA nesta etapa?** Sim (Gemini).
- **Para quê:** Levantamento da estrutura de campos compatíveis com o Firebase Auth (`email`, `password`, `displayName`) e auxílio na sintaxe dos widgets de validação (`TextFormField` com `FormState`).
- **O que a IA sugeriu:** Sugeriu a divisão modular em arquivos (`main.dart`, `login_page.dart` e `cadastro_page.dart`) com navegação nomeada por rotas.
- **O que alteramos ou aprendemos:** Adaptamos as regras de validação para os requisitos da disciplina, aprendemos a manipular formulários com chaves globais (`GlobalKey<FormState>`) e a estruturar as histórias de usuário na Wiki.




---

## Etapa 2 - Tela Principal, SharedPreferences e Drawer Navigation

### O que foi feito
- Adição da dependência `shared_preferences` no `pubspec.yaml` para persistência local chave-valor.
- Atualização da tela de Cadastro para salvar e sobrescrever os dados do usuário (`user_displayName`, `user_email`, `user_password`).
- Atualização da tela de Login para validar as credenciais diretamente contra os dados salvos no `SharedPreferences`.
- Criação da `HomePage` mantida em branco e equipada com `Drawer` de navegação exibindo o perfil ativo (`UserAccountsDrawerHeader`) e opção de logout.

### Prints das Telas (Etapa 2)
**Tela Principal em Branco:**
<img width="352" height="756" alt="image" src="https://github.com/user-attachments/assets/626af772-0e53-459f-9264-70bc188a20a3" />


**Drawer Navigation Aberto:**
<img width="353" height="757" alt="image" src="https://github.com/user-attachments/assets/d2859203-b783-452f-af32-dc68efd38672" />


### Vídeo de Apresentação (Etapa 2)
🔗 [Assistir ao vídeo da Etapa 2 no YouTube](vamos publicar ainda rs)

### Declaração de Uso de IA (Etapa 2)
- **Usamos IA nesta etapa?** Sim (Gemini).
- **Para quê:** Implementação assíncrona com `SharedPreferences.getInstance()` e estruturação do widget `Drawer` com `UserAccountsDrawerHeader`.
- **O que a IA sugeriu:** Sugeriu o uso de `pushReplacementNamed` nas transições de login/logout e o carregamento dos dados no `initState` da `HomePage`.
- **O que alteramos ou aprendemos:** Implementamos a lógica de sobrescrita a cada novo cadastro e compreendemos o ciclo de vida assíncrono (`Future`/`async`/`await`) para leitura de dados locais no Flutter.
