# CHATÃO

## Versão 

### **v0.1.1**

## Sobre o projeto


O **Chatão** é um sistema de **chat desenvolvido com Python e Django**, criado para permitir a comunicação entre usuários através de um chat.

## 🎯 Funcionalidades

O Chatão serve para:

* 👤 Cadastrar usuários;
* 💬 Permitir a comunicação através de um sistema de chat;
* 🗄️ Armazenar informações dos usuários e mensagens;
* 🔄 Gerenciar dados através de operações CRUD;
* 🌐 Praticar o desenvolvimento de aplicações web com Django.

## 🛠️ Tecnologias utilizadas

* 🐍 **Python**
* 🌐 **Django**
* 🗄️ **SQLite**
* 🔄 **CRUD**
* 🧩 **HTML / Templates Django**



## Diagrama de classes
~~~mermaid
classDiagram
    class Usuário {
        - string nome 
        - string nickname
        - string email
        - string telefone
        - date data_nascimento
        + nome() string
        + nome(string nome) void
        + nickname() string
        + nickname(string nickname) void
        + email() string
        + email(string email) void
        + telefone() string
        + telefone(string telefone) void
        + data_nascimento() date
        + data_nascimento(date data_nascimento) void
    }
~~~

Código-fonte:
~~~python
class Usuario:

    def __init__(self, nome, nickname, email, telefone, data_nascimento):
        self.__nome = nome
        self.__nickname = nickname
        self.__email = email
        self.__telefone = telefone
        self.__data_nascimento = data_nascimento

    @property
    def nome(self):
        return self.__nome

    @nome.setter
    def nome(self, nome):
        self.__nome = nome

    @property
    def nickname(self):
        return self.__nickname

    @nickname.setter
    def nickname(self, nickname):
        self.__nickname = nickname

    @property
    def email(self):
        return self.__email

    @email.setter
    def email(self, email):
        self.__email = email

    @property
    def telefone(self):
        return self.__telefone

    @telefone.setter
    def telefone(self, telefone):
        self.__telefone = telefone

    @property
    def data_nascimento(self):
        return self.__data_nascimento

    @data_nascimento.setter
    def data_nascimento(self, data_nascimento):
        self.__data_nascimento = data_nascimento
~~~