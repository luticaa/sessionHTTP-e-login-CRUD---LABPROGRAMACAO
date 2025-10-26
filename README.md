# sessionHTTP-e-login-CRUD---LABPROGRAMACAO
Persistencia de filtros e validação de usuário no LUTICA's SEBO (crud de discos musicais)

Sistema web desenvolvido em **Spring Boot** para gerenciamento de álbuns musicais, implementando **CRUD completo** com **autenticação de usuários** e **persistência de filtros** via sessão HTTP.

Sistema proposto como entrega para a disciplina de **Laboratório de Programação**.

---

#Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.x**
- **Spring MVC**
- **Spring Data JPA**
- **MySQL 8.0**
- **Thymeleaf**
- **Bootstrap 5.3**

---

#Funcionalidades Implementadas

### Autenticação e Sessão
- Login/Logout de usuários
- Cadastro de novos usuários
- Proteção de rotas por sessão
- Validação de credenciais
- Usuário administrador automático

### CRUD de Álbuns
- Criar novos álbuns
- Listar todos os álbuns
- Editar álbuns existentes
- Excluir álbuns
- Validações de campos obrigatórios

### Sistema de Filtros
- Busca por banda com persistência na sessão
- Filtro ativo visual na interface
- Limpeza de filtros com um clique
- Manutenção do estado entre navegações

---

## 🔑 Credenciais de Acesso

### Usuário Administrador
- **Email:** `admin@sebo.com`
- **Senha:** `123456`

---

## 🛣️ Rotas da Aplicação

### Públicas
- `/` → Redireciona para login
- `/login` → Página de autenticação
- `/registro` → Cadastro de usuários

### Protegidas (Requer Login)
- `/albuns/galeria` → Lista de álbuns
- `/albuns/novo` → Criar novo álbum
- `/albuns/editar/{id}` → Editar álbum
- `/albuns/excluir/{id}` → Excluir álbum
- `/albuns/galeria/filtro` → Aplicar filtro
- `/albuns/limpar-filtro` → Limpar filtro
- `/logout` → Fazer logout
