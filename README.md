# Navigation App (Jetpack Compose)

Projeto Android simples para praticar navegacao entre telas usando **Jetpack Compose** e **Navigation Compose**.

## Visao geral

O app simula um fluxo basico com quatro telas:

- `login` (tela inicial)
- `menu`
- `perfil`
- `pedidos`

A navegacao e feita com `NavHost` e rotas nomeadas, com `NavController` sendo repassado para cada tela composable.

## Fluxo de navegacao

- **Login** -> botao `ENTRAR` leva para `menu`
- **Menu** -> pode ir para `perfil`, `pedidos` ou voltar para `login` (`Sair`)
- **Perfil** -> botao `Voltar` navega para `pedidos`
- **Pedidos** -> botao `Voltar` retorna para `menu`

## Tecnologias usadas

- Kotlin
- Android Studio / Android Gradle Plugin
- Jetpack Compose (Material 3)
- `androidx.navigation:navigation-compose:2.6.0`
- Min SDK 24 / Target SDK 36 / Compile SDK 36

## Estrutura principal

- `app/src/main/java/.../MainActivity.kt`: configura `NavHost` e rotas
- `app/src/main/java/.../screens/LoginScreen.kt`
- `app/src/main/java/.../screens/MenuScreen.kt`
- `app/src/main/java/.../screens/PerfilScreen.kt`
- `app/src/main/java/.../screens/PedidosScreen.kt`

## Como executar

1. Abra o projeto no Android Studio.
2. Aguarde o sync do Gradle.
3. Selecione um emulador/dispositivo Android.
4. Execute o app pelo botao **Run**.

Opcionalmente, via terminal na raiz do projeto:

```powershell
.\gradlew.bat assembleDebug
```

## Capturas de tela

<img width="225" height="509" alt="image" src="https://github.com/user-attachments/assets/f5f5a33a-81c1-46b4-a0e6-50b29ca19b2f" />

<img width="219" height="511" alt="image" src="https://github.com/user-attachments/assets/6e705b94-bc97-4b47-87ae-adcfc5735fae" />

<img width="226" height="506" alt="image" src="https://github.com/user-attachments/assets/6ec3b1e1-f796-4eb9-bd00-f3f10e1d5b5d" />


<img width="227" height="509" alt="image" src="https://github.com/user-attachments/assets/3a750a50-c28a-43e3-9478-2dc10fb6f2cb" />
