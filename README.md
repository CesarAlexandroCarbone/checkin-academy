# checkin-academy
Api for manager checkins in academy using node.js

GymPass style app.

## RFs(Requisitos funcionais)

[] Deve ser possívl se cadastrar;
[] Deve ser possível se autenticar;
[] Deve ser possível obter o perfil de um usuário logado;
[] Deve ser possível obter o número de checkins realizados pelo usuário logado;
[] Deve ser possível o usuário obter seu histórico de checkins;
[] Deve ser possível o usuário buscar academias próximas;
[] Deve ser possível o usuário buscar academias pelo nome;
[] Deve ser possíel o usuário realizar checkin em uma academia;
[] Deve ser possível validar o checkin de um usuário;
[] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócios)

[] O usuário não deve poder se cadastrar com um email duplicado;
[] O usuário não pode fazer 2 checkins no mesmo dia;
[] O usuário não pode fazer checkin se não estiver perto (100m) da academia;
[] O checkin só pode ser validado até 20min após ser criado;
[] O checkin só pode ser validado por administradores;
[] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não-funcionais)

[] A senha do usuário precisa estar criptografada;
[] Os dados da aplicação precisam estar persistidos em um banco PostgresSql;
[] Todfas listas de dados precisam estar paginadas com 20 itens por página;
[] O usuário deve ser identificado por um JWT (JSON Web Token) 