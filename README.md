# 🚀 WorkHubLaravel - Marketplace de Serviços Freelance

Uma plataforma moderna e intuitiva para conectar profissionais com quem busca serviços. Publique vagas, encontre talentos e gerencie seus projetos tudo em um único lugar!

## 📋 Sobre o Projeto

WorkHub é um marketplace completo para serviços freelance que permite:

- 👤 **Criar Perfis Profissionais** - Destaque suas habilidades, portfólio e redes sociais
- 💼 **Publicar Vagas** - Anuncie serviços com descrição, valor/hora e tipo de trabalho
- 🔍 **Buscar Profissionais** - Encontre talentos por localização, profissão e tipos de serviço
- 📍 **Geolocalização** - Filtros por região (estado, cidade) para encontrar profissionais próximos
- 🔗 **Integração Social** - Links para GitHub, LinkedIn, Instagram e portfólio pessoal
- 🛡️ **Autenticação Segura** - Sistema robusto de autenticação com Laravel Sanctum

## 🛠️ Tecnologias

| Tecnologia | Versão |
|-----------|--------|
| **PHP** | 8.1.7 |
| **Laravel** | 9.21.5 |
| **Node.js** | 16.15.1 |
| **Database** | MySQL/SQLite |
| **Frontend** | Blade + Bootstrap/Tailwind |

## 📦 Requisitos

- PHP 8.0.2+
- Composer
- Node.js 14+
- npm ou yarn
- MySQL ou SQLite

## 🚀 Como Instalar

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/workhub.git
cd workhub
```

### 2. Instale as dependências PHP
```bash
composer install
```

### 3. Configure o arquivo de ambiente
```bash
cp .env.example .env
php artisan key:generate
```

### 4. Configure o banco de dados no `.env`
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=workhub
DB_USERNAME=root
DB_PASSWORD=
```

### 5. Execute as migrations
```bash
php artisan migrate
php artisan db:seed
```

### 6. Instale dependências Node.js
```bash
npm install
```

### 7. Compile os assets
```bash
npm run dev
```

### 8. Inicie o servidor
```bash
php artisan serve
```

Acesse: `http://localhost:8000`

## 📖 Funcionalidades Principais

### Para Profissionais
- ✅ Criar e gerenciar perfil profissional
- ✅ Adicionar foto de perfil
- ✅ Listar redes sociais e portfólio
- ✅ Visualizar e aplicar a vagas
- ✅ Gerenciar localização e disponibilidade

### Para Contratantes
- ✅ Publicar vagas de trabalho
- ✅ Definir valor/hora e tipo de serviço
- ✅ Buscar profissionais por região
- ✅ Gerenciar vagas publicadas
- ✅ Filtrar por especialização

## 📁 Estrutura do Projeto

```
workhub/
├── app/
│   ├── Base/              # Modelos e controllers base
│   ├── Job/               # Módulo de vagas
│   ├── Profile/           # Módulo de perfis
│   └── Repositories/      # Padrão Repository
├── routes/
│   ├── web.php            # Rotas web
│   └── api.php            # Rotas API
├── resources/
│   ├── views/             # Templates Blade
│   └── js/                # Assets JavaScript
├── database/
│   ├── migrations/        # Esquemas do banco
│   └── seeders/           # Seeds de dados
└── public/                # Assets públicos
```

## 🔌 API Endpoints

### Autenticação
- `POST /api/login` - Fazer login
- `POST /api/register` - Registrar novo usuário
- `POST /api/logout` - Fazer logout

### Vagas
- `GET /api/jobs` - Listar todas as vagas
- `POST /api/jobs` - Criar nova vaga
- `GET /api/jobs/{id}` - Detalhes da vaga
- `PUT /api/jobs/{id}` - Atualizar vaga
- `DELETE /api/jobs/{id}` - Deletar vaga

### Perfis
- `GET /api/profiles` - Listar perfis
- `GET /api/profiles/{id}` - Detalhes do perfil
- `PUT /api/profiles/{id}` - Atualizar perfil

## 🧪 Testes

Execute os testes com PHPUnit:
```bash
php artisan test
```

## 📝 Contribuindo

Contribuições são bem-vindas! Por favor:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👥 Autor

Criado com ❤️ por [Seu Nome](https://github.com/seu-usuario)

## 💬 Suporte

Encontrou um bug? Abra uma [Issue](https://github.com/seu-usuario/workhub/issues)!

---

**⭐ Se este projeto ajudou você, considere dar uma estrela!**
