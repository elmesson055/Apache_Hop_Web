# Hop Web Docker Environment

Ambiente Docker para integração de bancos MySQL e PostgreSQL com Apache Hop Web

## Pré-requisitos
- Docker Desktop instalado ([Download](https://www.docker.com/products/docker-desktop/))
- 8GB+ de RAM disponível
- Diretório base: `C:\Users\elmessonjesus\Desktop\Hop`

## Estrutura de Diretórios

Hop/
├── docker-compose.yml
├── files/
│   ├── mysql-connector-j-8.4.0.jar
│   └── postgresql-42.7.3.jar
├── mysql-data/
└── postgres-data/


## Configuração Inicial
1. Criar estrutura de diretórios:
```bash
mkdir "%USERPROFILE%\Desktop\Hop\files"
mkdir "%USERPROFILE%\Desktop\Hop\mysql-data"
mkdir "%USERPROFILE%\Desktop\Hop\postgres-data"
```

docker-compose up -d


## Serviços Disponíveis
### 1. MySQL (Fonte)
- **Porta:** 3306
- **Credenciais:**
  - Usuário: `elmesson`
  - Senha: `elmesson1810`
  - Database: `hopfonte`

## Uso com DbSchema
2. Conexão MySQL:
   - Host: `localhost`
   - Port: `3306`
   - User: `elmesson`
   - Password: `elmesson1810`
   - Database: `hopfonte`
1. Instale o DbSchema
2. Conexão MySQL:
   
   - Host: localhost
   - Port: 3306
   - User: elmesson
   - Password: elmesson1810
   - Database: hopfonte
3. Conexão PostgreSQL:
   
   - Host: localhost
   - Port: 5432
   - User: elmesson
   - Password: dsa2212
   - Databases: dev , qa , prod


##Comandos Úteis    
   docker-compose up -d         

   docker-compose down

   docker-compose logs

   docker-compose ps