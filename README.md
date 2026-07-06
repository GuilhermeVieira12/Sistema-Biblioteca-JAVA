# Sistema-Biblioteca-JAVA
Um sistema interativo desenvolvido em Java para gerenciar o acervo de uma biblioteca, permitindo o cadastro de materiais, registro de usuários e controle completo do ciclo de empréstimos e devoluções.

Funcionalidades

Gestão de Acervo: Cadastro de Livros e Revistas com identificadores únicos (IDs).
Gestão de Usuários: Registro de clientes para vinculação aos empréstimos.
Sistema de Empréstimos: Validação de disponibilidade de itens em tempo real.
Devolução e Renovação: Controle de prazos (ex: +7 dias para renovação), com restrições específicas (Revistas não podem ser renovadas).
Listagem Dinâmica: Exibição do acervo completo utilizando Polimorfismo para diferenciar os atributos específicos de cada tipo de material.

Conceitos Aplicados

Linguagem:** Java (Console)
Estrutura:** MVC simplificado (Model, Service, Exception, Main)
Herança & Classes Abstratas: Classe base `Material` estendida por `Livro` e `Revista`.
Polimorfismo:** Sobrescrita de métodos (`@Override`) para comportamentos específicos na listagem de dados.
Interfaces / Contratos:Implementação de `Emprestavel` e `Renovavel` para garantir regras de negócio rigorosas.
Tratamento de Exceções: Criação de exceções customizadas (ex: `MaterialIndisponivelException`) capturadas via blocos `try-catch` para impedir a quebra do sistema.
Encapsulamento: Proteção de dados sensíveis utilizando modificadores `private` e `protected`.
