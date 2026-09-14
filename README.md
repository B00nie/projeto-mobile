# Sistema de Consultas Mobile

App em React Native (Expo) para agendamento de consultas medicas, com telas separadas para pacientes e medicos. Consome uma API backend em Spring Boot.

## Stack

- Expo 54 / React Native 0.81
- React Navigation (native-stack)
- Axios

## Rodando o projeto

```bash
npm install
npm start
```

Depois escolha a plataforma (`npm run android`, `npm run ios` ou `npm run web`).

O backend Spring Boot precisa estar rodando em `http://localhost:8080` (ver `src/services/api.ts`). Dependendo de onde o app roda, ajuste a `BASE_URL`:

- Expo Web / iOS Simulator: `localhost` funciona
- Android Emulator: use `10.0.2.2`
- Dispositivo fisico: use o IP da maquina na rede local

## Login

- **Paciente**: login por CPF (11 digitos)
- **Medico**: login por CRM

## Cadastros de teste

| Nome | Perfil | Documento |
|---|---|---|
| Enzo | Paciente | CPF: 10298971747 |
| Pedro | Paciente | CPF: 26849314106 |
| Dra. Alessandra | Medica | CRM: 223344 |
| Dr. Roberto Silva | Medica | CRM: 347170 |
