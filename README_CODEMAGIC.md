# Build no Codemagic

Este projeto já contém `codemagic.yaml` na raiz.

1. Suba esta pasta para um repositório GitHub.
2. No Codemagic, conecte o repositório.
3. Selecione o workflow `android-apk`.
4. Clique em **Start new build**.
5. Ao terminar, baixe `app-debug.apk` na seção **Artifacts**.

O workflow usa `assembleDebug`, portanto não exige keystore para gerar o APK instalável de teste. Para uma versão de produção/Google Play, será necessário configurar uma keystore no Codemagic e trocar o build para `assembleRelease`.
