# [BluePayRingAndroidDoc](https://sdkpay.github.io/BluePayRingAndroidDoc/)

#### [Сущности и классы](https://sdkpay.github.io/BluePayRingAndroidDoc/classes) | [Работа с SDK](https://sdkpay.github.io/BluePayRingAndroidDoc/usage) | [Актуальная версия SDK](https://sdkpay.github.io/BluePayRingAndroidDoc/version) | [Используемые зависимости](https://sdkpay.github.io/BluePayRingAndroidDoc/dependencies)

<br>

# Работа с SDK

## Запрос платежных токенов

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


### Отмена/остановка запроса платежных токенов по sub карты, ранее запусщенный через getTokensForCard()

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