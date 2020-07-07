# Meals App
Este App foi criado no XCode com o objetivo de integrar um módulo flutter coo uma view iOS e implementar
canais de comunicação entre App nativo e o [módulo Flutter](https://github.com/akmerejf/flutter-meals-module)

## Getting Started
Primeiro siga o passo a passo descrito no repositório do módulo flutter acima
para gerar o arquivo `.framework` e integrar no App iOS

## Integrar o módulo flutter no XCode
Após gerar o arquivo `.framework` no diretório especificado no readme do módulo flutter siga os seguintes passos:

- Copie o diretório `MealCategories` inteiro do módulo flutter para a raiz do projeto XCode
- No XCode, navegue em > `MealsApp > Build Settings > Search Paths > Framework Search Paths`, adicione:
> `$(PROJECT_DIR/MealsApp/MealCategories/Flutter/Debug`

- Build no projeto **⌘+b**

[Adicionando uma flutter view](https://flutter.dev/docs/development/add-to-app/ios/add-flutter-screen)
[Adicionando canais e métodos de comunicação entre o módulo flutter e o app nativo](https://flutter.dev/docs/development/platform-integration/platform-channels)

## Visão arquitetural

![arquitetura](https://github.com/akmerejf/flutter-meals-module/blob/master/form.png?raw=true)
