# [BluePayRingAndroidDoc](https://sdkpay.github.io/BluePayRingAndroidDoc/)

#### [Сущности и классы](https://sdkpay.github.io/BluePayRingAndroidDoc/classes) | [Работа с SDK](https://sdkpay.github.io/BluePayRingAndroidDoc/usage) | [Актуальная версия SDK](https://sdkpay.github.io/BluePayRingAndroidDoc/version) | [Используемые зависимости](https://sdkpay.github.io/BluePayRingAndroidDoc/dependencies)

<br>

# Работа с SDK v2.0

### Установка необходимых настроек для осуществления запроса платежных токенов

```kotlin
RingClientSdk
    .getInstance()
    .setup(RingSdkConfig(...))
```


### Авторизация пользователя (без выбора карты)

```kotlin
RingClientSdk
    .getInstance()
    .auth(activityContext)
```



### Запрос платежных токенов

```kotlin
RingClientSdk
    .getInstance()
    .getTokens(activityContext)
```


### Запрос платежных токенов для ранее выбранной карты

```kotlin
RingClientSdk
    .getInstance()
    .getTokensForCard()
```


### Отмена запроса платежных токенов для ранее выбранной карты (через getTokensForCard())

```kotlin
RingClientSdk
    .getInstance()
    .cancelGettingTokensForCard()
```


### Деактивацию ранее выпущенных токенов пользователя

```kotlin
RingClientSdk
    .getInstance()
    .deactivateTokens()
```


### Отмена запроса деактивации ранее выпущенных токенов пользователя

```kotlin
RingClientSdk
    .getInstance()
    .cancelGettingTokensForCard()
```



### Разлогирование пользователя

```kotlin
RingClientSdk
    .getInstance()
    .logout(context)
```


<br>

# Работа с SDK v1.0

### Запрос платежных токенов

```kotlin
RingClientSdk
    .getInstance()
    .getTokens(RingSdkConfig.Default(...))
```


### Запрос платежных токенов по sub карты

```kotlin
RingClientSdk
    .getInstance()
    .getTokensForCard(RingSdkConfig.ForCard(...))
```


### Отмена запроса платежных токенов по sub карты, ранее выпущенных через getTokensForCard()

```kotlin
RingClientSdk
    .getInstance()
    .cancelGettingTokensForCard()
```


### Разлогирование пользователя

```kotlin
RingClientSdk
    .getInstance()
    .logout(context)
```