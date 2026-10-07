# Voxali Android

Projeto Android preparado para GitHub Actions.

## Gerar APK

1. Suba todos os arquivos para um repositório GitHub.
2. Abra a aba **Actions**.
3. Selecione **Build Voxali APK**.
4. Clique em **Run workflow**.
5. Quando terminar, abra a execução.
6. Em **Artifacts**, baixe **Voxali-APK**.

## Sincronização

O aplicativo faz uma requisição para:

`https://voxali.com.br/api/sync`

a cada 5 segundos.

### Importante

O endereço `/api/sync` precisa existir no backend do Voxali e retornar HTTP 2xx.

Este projeto não usa o site como uma simples página dentro de um WebView: ele é um aplicativo Android nativo que conversa com o backend por HTTP.
