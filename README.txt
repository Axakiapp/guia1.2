
Guia1 - pacote completo para deploy (Guia1.zip)

Arquivos incluídos:
- index.html        -> Site público
- admin.html        -> Painel admin (acesso por Firebase Auth)
- style.css
- app.js            -> lógica do site (Firestore + Storage)
- firebase-config.js -> coloque seu firebaseConfig se quiser alterar
- assets/           -> logo and icons

CONFIGURE FIREBASE (essencial):
1) No Console Firebase (https://console.firebase.google.com):
   - Abra o projeto (guia1-23459).
   - Authentication -> Sign-in method -> habilite Email/Password.
   - Authentication -> Users -> Add user: guia1.br@hotmail.com / Lu32Iv75@
   - Firestore -> criar banco (modo test ou production conforme sua escolha).
   - Storage -> criar bucket, ajustar regras (para testes, regras liberais; para produção, proteger).

2) Deploy no Vercel:
   - https://vercel.com/new -> Upload -> selecione os arquivos do pacote (index.html na raiz).
   - Após deploy, abra /admin e faça login com o usuário criado.

OBS:
- Para segurança real, ajuste regras do Firestore/Storage e use custom claims para admin.
- Caso queira, eu posso ajudar a ajustar as regras e criar o usuário admin no Firebase passo a passo.
