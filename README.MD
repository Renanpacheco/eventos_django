# Eventos Django

## 📌 Descrição

O **Eventos Django** é uma aplicação backend desenvolvida com Django para gerenciamento de eventos e disponibilidade de horários.

A plataforma permite que usuários:

* Criem eventos
* Definam horários disponíveis
* Participem de eventos criados por outros usuários

O projeto segue uma arquitetura organizada por camadas (Layer-Based), promovendo separação de responsabilidades, escalabilidade e facilidade de manutenção.

---

## 🧱 Arquitetura

O projeto está estruturado com base em boas práticas modernas:

* **apps/** → Domínios da aplicação (ex: eventos)
* **services/** → Regras de negócio
* **selectors/** → Consultas ao banco
* **api/** → Camada de entrada (REST)
* **shared/** → Código reutilizável

---

## ⚙️ Pré-requisitos

Antes de começar, você precisa ter instalado:

* Python 3.10+
* pip
* Virtualenv (opcional, mas recomendado)

---

## 🚀 Como rodar o projeto

### 1. Clonar o repositório

```bash
git clone <url-do-repositorio>
cd eventos-django
```

---

### 2. Criar e ativar ambiente virtual

```bash
python -m venv venv
```

#### Linux / Mac

```bash
source venv/bin/activate
```

#### Windows

```bash
venv\Scripts\activate
```

---

### 3. Instalar dependências

```bash
pip install -r requirements.txt
```

---

### 4. Configurar variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto (se necessário).

---

### 5. Rodar migrations

```bash
python manage.py migrate
```

---

### 6. Criar superusuário (opcional)

```bash
python manage.py createsuperuser
```

---

### 7. Iniciar o servidor

```bash
python manage.py runserver
```

---

## 🌐 Acessos

* API: http://127.0.0.1:8000/api/
* Admin: http://127.0.0.1:8000/admin/

---

## 🧪 Testes

Para rodar os testes:

```bash
python manage.py test
```

---

## 🎯 Objetivo do Projeto

* Praticar arquitetura backend moderna com Django
* Implementar separação de responsabilidades (services, selectors, API)
* Servir como base para aplicações escaláveis

