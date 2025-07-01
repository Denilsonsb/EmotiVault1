# EmotiVault1
Projeto de banco de dados
# EmotiVault: Banco de Dados para Memórias Emocionais

> Um projeto original que propõe uma estrutura relacional para armazenar experiências emocionais humanas, integrando tecnologia e bem-estar.

---

## Sobre o projeto

O **EmotiVault** é um banco de dados relacional projetado para registrar **memórias emocionais** de forma estruturada, contextual e ética. A proposta é permitir a análise de padrões emocionais, apoiar o autoconhecimento e abrir portas para futuras integrações com inteligência artificial empática e ferramentas de apoio à saúde mental.

---

##  Tecnologias e ferramentas utilizadas

- **PostgreSQL** – SGBD robusto e gratuito
- **DBeaver** – Cliente para consultas SQL
- **dbdiagram.io** – Modelagem de dados visual (ER)
- **Python + SQLAlchemy** – Simulação de acesso ao banco
- **Visual Studio Code** – Edição de código e documentação
- **Whisper (OpenAI)** – Potencial de integração com transcrição de voz para análise emocional

---

##  Estrutura do Banco de Dados

O banco é composto por tabelas como:

- `Usuario`
- `MemoriaEmocional`
- `Emoção`
- `Memoria_Emocao` (N:N)
- `PessoaEnvolvida`
- `Memoria_Pessoa` (N:N)

Você pode visualizar o [diagrama ER](docs/diagram_er.png) e acessar os scripts SQL em [`sql/create_tables.sql`](sql/create_tables.sql).

---

## Exemplo de uso

```sql
-- Inserindo uma memória emocional
INSERT INTO MemoriaEmocional (id, usuario_id, titulo, descricao, data_ocorrencia)
VALUES ('uuid...', 'uuid...', 'Conversa importante', 'Fiquei ansioso após uma reunião familiar', '2025-06-15');
