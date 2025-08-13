# Desafio de Código: Aprenda na Prática Programação Orientada a Objetos com Java

## 📚 Descrição do Desafio

Este projeto é um desafio de código desenvolvido para desmistificar e praticar os conceitos fundamentais da Programação Orientada a Objetos (POO) utilizando a linguagem Java. O objetivo principal é aplicar os quatro pilares da OO em um cenário real: **Abstração**, **Encapsulamento**, **Herança** e **Polimorfismo**.

O domínio modelado neste desafio é um sistema de gerenciamento de **Bootcamps**, onde desenvolvedores (Devs) se inscrevem em conteúdos (Cursos e Mentorias), progridem e calculam seu progresso (XP).

---

## 🚀 Objetivo do Projeto

O objetivo principal é exercitar a modelagem de um domínio de negócio real através dos conceitos de POO:

- **Abstração**: Modelar as entidades `Bootcamp`, `Conteudo`, `Curso`, `Mentoria` e `Dev`, definindo seus atributos e comportamentos essenciais.
- **Encapsulamento**: Proteger os dados das classes (`private`) e controlar o acesso a eles através de métodos (`getters` e `setters`).
- **Herança**: Criar uma hierarquia de classes, onde `Curso` e `Mentoria` herdam da classe base `Conteudo`, aproveitando a reutilização de código e definindo comportamentos comuns.
- **Polimorfismo**: Implementar o método `calcularXp()` na classe `Conteudo` de forma abstrata, permitindo que cada subclasse (`Curso` e `Mentoria`) forneça sua própria implementação específica.

---

## 📁 Estrutura do Projeto

A lógica do projeto está organizada nas seguintes classes, localizadas no pacote `br.com.dio.desafio.dominio`:

- `Main.java`: O ponto de entrada da aplicação. Orquestra a criação dos objetos (`Bootcamp`, `Cursos`, `Mentorias`, `Devs`) e simula a interação entre eles, demonstrando os conceitos de inscrição, progresso e cálculo de XP.
- `Conteudo.java`: Uma **classe abstrata** que representa o conceito genérico de conteúdo de um bootcamp. Possui atributos comuns a todos os conteúdos (título, descrição) e um método abstrato `calcularXp()` que deve ser implementado pelas subclasses.
- `Curso.java`: Uma classe concreta que **herda** de `Conteudo`. Adiciona o atributo `cargaHoraria` e implementa a lógica específica para calcular o XP de um curso.
- `Mentoria.java`: Uma classe concreta que **herda** de `Conteudo`. Adiciona o atributo `data` e implementa a lógica específica para calcular o XP de uma mentoria.
- `Dev.java`: Representa um desenvolvedor. Ele pode se inscrever em um `Bootcamp`, progredir nos conteúdos e calcular o seu total de XP, demonstrando a interação entre as diferentes classes.
- `Bootcamp.java`: Representa o Bootcamp. Ele agrupa os conteúdos e os desenvolvedores inscritos, servindo como uma entidade central.

---

## 🤝 Contribuição

Este repositório foi criado para fins de estudo e prática na DIO. Sinta-se à vontade para explorá-lo, modificá-lo e adaptá-lo.

Se tiver alguma sugestão ou encontrar um problema, por favor, abra uma "Issue".
Se te ajudei de alguma forma, ficarei feliz em saber. E caso você conheça alguém que se identifique com o conteúdo, não deixe de compartilhar.

⭐️ Dê uma estrela no projeto!
