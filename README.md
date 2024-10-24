# *Relatório do Projeto: Gerenciador de Produtos (CRUD)*
1. Introdução
Este projeto consiste em um aplicativo Android que permite a gestão de produtos utilizando o Firebase Firestore como banco de dados. As operações básicas de CRUD (Create, Read, Update, Delete) são implementadas para facilitar a adição, busca, atualização e remoção de produtos.

2. Tecnologias Utilizadas
Android Studio: IDE para desenvolvimento Android.
Firebase Firestore: Serviço de banco de dados NoSQL em tempo real.
Java: Linguagem de programação utilizada para o desenvolvimento do aplicativo.
3. Funcionalidades
O aplicativo possui as seguintes funcionalidades:

Adicionar Produto: O usuário pode inserir um código e um valor para cadastrar um novo produto.
Buscar Produto: Permite ao usuário procurar um produto pelo código e visualizar seu valor.
Atualizar Produto: O usuário pode atualizar o valor de um produto existente através de seu código.
Deletar Produto: O usuário pode remover um produto utilizando seu código.
4. Estrutura do Código
O código está dividido em duas partes principais: a lógica do aplicativo (MainActivity.java) e a interface do usuário (activity_main.xml).

4.1 MainActivity.java
Atributos:

EditText editTextCode: Campo para entrada do código do produto.
EditText editTextValue: Campo para entrada do valor do produto.
TextView textViewResult: Exibe mensagens ao usuário.
FirebaseFirestore db: Instância do Firestore para interações com o banco de dados.
Métodos Principais:

addProduct(): Adiciona um novo produto ao Firestore.
searchProduct(): Busca um produto pelo código e exibe seu valor.
updateProduct(): Atualiza o valor de um produto existente.
deleteProduct(): Remove um produto do banco de dados.
showMessage(String message): Exibe mensagens em forma de Toast.
4.2 activity_main.xml
Layout:
Utiliza um LinearLayout vertical com campos de entrada e botões.
Cada botão realiza uma operação específica (Adicionar, Atualizar, Deletar, Buscar).
TextViews são utilizados para exibir informações e mensagens.
5. Experiência do Usuário
A interface é simples e intuitiva, permitindo que o usuário realize operações sem complexidade. Mensagens de feedback são exibidas para confirmar operações bem-sucedidas ou informar sobre erros.

6. Considerações Finais
O projeto demonstra a implementação eficaz de operações CRUD em um aplicativo Android com integração ao Firebase Firestore. Pode ser expandido para incluir funcionalidades adicionais, como autenticação de usuários, categorização de produtos, ou uma interface mais elaborada com listas e detalhes de produtos.

7. Possíveis Melhorias
Validação de Dados: Implementar validações mais robustas para entradas do usuário.
Interface do Usuário: Melhorar a estética e a usabilidade da interface.
Persistência Local: Adicionar suporte a armazenamento local para operações offline.
Documentação: Criar uma documentação mais detalhada sobre a arquitetura e uso do aplicativo.
Esse relatório fornece uma visão geral do projeto e suas funcionalidades, destacando tanto a implementação quanto a experiência do usuário.
