# Alura Space | Curso "Django: templates e boas práticas"

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=yellow)
![Django](https://img.shields.io/badge/Django-4.x-green?logo=django)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

Projeto de uma galeria de fotos, desenvolvido como parte do curso **"Django: templates e boas práticas"** da [Alura](https://www.alura.com.br). O foco principal do projeto é a aplicação dos conceitos fundamentais do sistema de templates do Django e a implementação de boas práticas de organização e desenvolvimento.

## 🚀 Sobre o Projeto

O Alura Space é uma aplicação web que simula uma galeria de fotos espaciais. Ele possui uma página inicial que exibe uma coleção de imagens e uma página de detalhe para cada imagem. O projeto foi estruturado para maximizar a reutilização de código e a manutenibilidade, seguindo os padrões recomendados pelo Django.

### ✨ Funcionalidades

* Página inicial com uma galeria de imagens.
* Página de visualização individual para cada imagem.
* Layout responsivo e estilizado com CSS.
* Estrutura de templates reutilizável (cabeçalho e rodapé).

## 🛠️ Tecnologias Utilizadas

* **Python:** Linguagem de programação principal.
* **Django:** Framework web utilizado para o back-end.
* **HTML5 e CSS3:** Para a estruturação e estilização do front-end.

## 🧠 Principais Aprendizados e Conceitos Aplicados

Este projeto foi fundamental para solidificar meu conhecimento sobre a camada de apresentação (front-end) em Django e as melhores formas de estruturar um projeto. Os principais tópicos abordados foram:

#### 1. **Sistema de Roteamento Avançado**
   - Descentralização das URLs, criando um arquivo `urls.py` para cada aplicação e utilizando a função `include()` no arquivo de URLs do projeto principal.
   - **Boas Práticas:** Adoção do padrão de nomear todas as rotas com o parâmetro `name='...'` para criar referências dinâmicas e seguras com a tag `{% url 'nome_da_rota' %}`.

#### 2. **Templates e Renderização**
   - Transição do `HttpResponse` para a função `render()`, que permite combinar um template com um contexto (dicionário de dados) para gerar uma resposta HTTP.
   - Envio de dados (contexto) da `view` para o template, permitindo a exibição de informações dinâmicas.

#### 3. **Gerenciamento de Arquivos Estáticos**
   - Configuração das variáveis `STATIC_URL`, `STATICFILES_DIRS` e `STATIC_ROOT` para o correto gerenciamento de arquivos como CSS, JavaScript e imagens.
   - Utilização das template tags `{% load static %}` e `{% static 'caminho/do/arquivo' %}` para gerar URLs para os arquivos estáticos de forma dinâmica e manutenível.
   - Compreensão do comando `collectstatic` e seu papel em ambientes de produção.

#### 4. **Herança de Templates (DRY - Don't Repeat Yourself)**
   - Criação de um template base (`base.html`) com toda a estrutura repetitiva do site (HTML boilerplate, header, footer, links de CSS/JS).
   - Utilização da tag `{% extends 'base.html' %}` nos templates "filhos" para herdar a estrutura base.
   - Definição de áreas editáveis no template base com as tags `{% block nome_do_bloco %}` e `{% endblock %}`, que são preenchidas pelos templates filhos.

#### 5. **Partials e Componentes Reutilizáveis**
   - Uso da tag `{% include 'caminho/do/partial.html' %}` para criar e reutilizar componentes menores e independentes, como o cabeçalho e o rodapé.
   - Entendimento da diferença conceitual entre `extends` (herança de layout) e `include` (composição de componentes).

## 📂 Como Executar o Projeto Localmente

Siga os passos abaixo para rodar o Alura Space em sua máquina.

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/Lucas-Fiche/alura-django-aluraspace.git (https://github.com/Lucas-Fiche/alura-django-aluraspace.git)
    cd alura-django-aluraspace
    ```

2.  **Crie e ative um ambiente virtual:**
    ```bash
    # Criar o ambiente
    python -m venv .venv

    # Ativar no Windows
    .\.venv\Scripts\activate

    # Ativar no Linux/macOS
    source .venv/bin/activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Execute o servidor de desenvolvimento:**
    ```bash
    python manage.py runserver
    ```

5.  **Acesse a aplicação:**
    Abra seu navegador e acesse `http://127.0.0.1:8000/`

## 👨‍💻 Autor

Projeto desenvolvido por **Lucas Fiche** como parte dos estudos na plataforma Alura.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/lucas-fiche-76aa24201)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-fiche-76aa24201)