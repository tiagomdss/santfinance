# Sant Finanças

Controle financeiro pessoal em Nuxt 4, TypeScript, Tailwind CSS e Nuxt UI. Login Google com Firebase Authentication e dados por usuário no Cloud Firestore.

## Executar

```sh
npm install
npm run dev
```

Abra http://localhost:3000. Para validar e compilar:

```sh
npm run typecheck
npm run build
```

## Firebase

A configuração Web está em `app/app.vue`. Para usar outro projeto, substitua esse objeto e habilite o provedor Google no Firebase Authentication. Autorize o domínio usado pelo aplicativo.

Publique as regras de `firestore.rules` no Firestore. Cada conta acessa somente `users/{uid}/finance/main`. Não use chaves privadas ou credenciais de conta de serviço no navegador.

## Dados e funcionalidades

Contas mensais, entradas extras, valores a receber, parcelas, salário com escopo por mês, relatórios e backups JSON. Importar JSON substitui os dados atuais após confirmação. Exportação Excel/CSV e impressão para PDF estão disponíveis no histórico.

Os backups pessoais e as dependências não são versionados. Biometria e notificações push ainda não estão implementadas.
