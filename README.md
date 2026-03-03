# Urna-Eletronica-em-Java
📌 *Descrição*

Este projeto consiste na implementação de um Sistema de Urna Eletrônica Simplificada, desenvolvido em Java, com o objetivo de simular o funcionamento básico de um sistema de votação digital.
O sistema permite:
Cadastro de cargos
Cadastro de candidatos
Registro de votos
Controle de estados da votação
Emissão de relatório final
Encerramento controlado da votação
O projeto foi estruturado seguindo princípios de orientação a objetos, com separação clara entre regras de negócio, controle de fluxo e interface textual.

🧠 *Conceitos Aplicados*

Programação Orientada a Objetos (POO)
Encapsulamento
Enum para controle de estados
Organização em múltiplas classes
Separação de responsabilidades
Estrutura de dados (ArrayList)
Controle de fluxo e validação de entrada

🏗️ *Estrutura do Projeto*
Projeto_UrnaEletronica/
│
├── Main.java
├── UrnaEletronica.java
├── Eleicao.java
├── Cargo.java
├── Candidato.java
├── Relatorio.java
├── Tela.java
└── EstadoVotacao.java

📄 *Principais Classes*
Classe	Responsabilidade
Main	Ponto de entrada do programa
UrnaEletronica	Controla o fluxo principal da aplicação
Eleicao	Gerencia os cargos cadastrados
Cargo	Representa um cargo em disputa
Candidato	Representa um candidato
Relatorio	Gera relatório final da votação
Tela	Interface textual com o usuário
EstadoVotacao	Enum que controla os estados da votação

🔄 *Estados do Sistema*

O sistema utiliza um enum (EstadoVotacao) para controlar o ciclo da votação:
INICIANDO
ADMIN
VOTANDO
ENCERRADA
Isso garante maior organização e evita inconsistências no fluxo do programa.

⚙️ *Como Executar o Projeto*
🔹 Pré-requisitos
Java JDK 8 ou superior
Terminal ou IDE (IntelliJ, Eclipse, VS Code, etc.)

🔹 Compilação via Terminal
Navegue até a pasta do projeto:
cd Projeto_UrnaEletronica
Compile os arquivos:
javac *.java
Execute o programa:
java Main

🗳️ *Funcionalidades*

Cadastro manual de cargos
Cadastro de candidatos por cargo
Registro de votos por número
Validação de voto
Voto nulo
Encerramento controlado (sequência específica de votos)
Emissão de relatório final com totalização

🔐 *Regra Especial de Encerramento*

O sistema possui um mecanismo de encerramento que é ativado após uma sequência específica de votos confirmados (exemplo: três votos "999").

Essa funcionalidade foi implementada para simular um controle administrativo seguro.

🧪 *Configuração Padrão*

O método:
urna.setupEleicaoPadraoSeVazia();
Permite iniciar o sistema com cargos e candidatos pré-configurados.
Caso seja necessário realizar todo o cadastro manualmente (por exigência acadêmica), basta comentar essa linha no Main.java.

🎯 *Objetivo Acadêmico*

Este projeto foi desenvolvido como prática acadêmica para consolidar conceitos fundamentais de:
Modelagem orientada a objetos
Estruturação de sistemas
Controle de estados
Manipulação de coleções

👨‍💻 *Autor*
Eduardo Brandão Dias
Graduando em Engenharia de Computação

📜 *Licença*
Este projeto foi desenvolvido para fins acadêmicos e de aprendizado.
