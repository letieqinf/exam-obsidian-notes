*Трехкратное использование алгоритма DES*

Предполагается использование двух или трех ключей:
- $3$ – $2^{168}$ вариантов ключа;
- $2$ – $2^{112}$ вариантов ключа.

**Варианты 3DES**:

| № | Шифрование | Расшифрование |
| :-: | :-: | :-: |
| 1 | $E_{k_1}E_{k_2}E_{k_3}$ | $D_{k_3}D_{k_2}D_{k_1}$ |
| 2 | $E_{k_1}D_{k_2}E_{k_3}$ | $D_{k_3}E_{k_2}D_{k_1}$ |
| 3 | $E_{k_1}E_{k_2}E_{k_1}$ | $D_{k_1}D_{k_2}D_{k_1}$ |
| 4 | $E_{k_1}D_{k_2}E_{k_1}$ | $D_{k_1}E_{k_2}D_{k_1}$ |
Примечание: последний позволяет передавать сообщения устройствам, не поддерживающим трехкратное применение DES: при $k2=k1$.

**Преимущества**:
- Высокая криптостойкость;

**Недостатки:
- Снижение производительности.