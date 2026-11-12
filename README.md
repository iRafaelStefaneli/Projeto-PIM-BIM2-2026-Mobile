<p align="center">
  <img src="assets/logo.png" alt="Bons Momentos" width="180">
</p>

<h1 align="center">Bons Momentos Entregador</h1>

<p align="center">
  Aplicativo Android para os entregadores da confeitaria Bons Momentos.
</p>

---

## Sobre

Bons Momentos Entregador é o aplicativo mobile do projeto PIM, voltado ao entregador. Quando a cozinha envia um pedido, o entregador o vê no app, consulta os dados da entrega e marca como concluído ao entregar.

## Como baixar

Requisitos: Android 8.0 ou superior e conexão com a internet.

1. Abra a página de [Releases](https://github.com/iRafaelStefaneli/Projeto-PIM-BIM2-2026-Mobile/releases/latest) pelo celular.
2. Baixe o arquivo `.apk`.
3. Abra o arquivo e, se o Android pedir, permita instalar apps desconhecidos.
4. Entre com o e-mail e a senha fornecidos pela equipe da Bons Momentos.

## Como funciona

1. A cozinha envia o pedido para um entregador pelo sistema web.
2. O pedido aparece no app desse entregador, e só nele.
3. O entregador toca no pedido para ver produto, pagamento, CEP e endereço.
4. Ao entregar, toca em **Concluir** e o pedido passa para *Entregue* no sistema.

O app precisa de internet para funcionar: login, pedidos e conclusões usam o banco de dados online.

## Funcionalidades

- Login com e-mail e senha
- Lista com os pedidos do entregador
- Detalhes do pedido: produto, pagamento, CEP e endereço
- Botão para concluir a entrega
- Atualização dos pedidos pela internet
- Sair da conta

## Para desenvolvedores

Tecnologias: Kotlin, Retrofit e Supabase.

1. Abra o projeto no Android Studio (Hedgehog ou mais recente, JDK 17).
2. No Supabase, execute o arquivo `supabase_setup.sql`.
3. Em `app/build.gradle.kts`, configure `BASE_URL` e `SUPABASE_KEY` com a chave pública do projeto.
4. Execute o app em um aparelho ou emulador.

Para testar sem servidor, altere `MODO_DEMO` para `true` no mesmo arquivo.

Para gerar o APK:

```bash
./gradlew assembleDebug
```
