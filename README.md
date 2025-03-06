# Задание 1

![image](https://github.com/user-attachments/assets/ca84f57e-dec7-4a46-9821-6d78c43b36be)


# Задание 2

![image](https://github.com/user-attachments/assets/730849c0-f324-430d-8ba3-b5127f71abdf)


### утилизация CPU для nodeexporter (в процентах, 100-idle);
```
100 - (avg by (instance) (rate(node_cpu_seconds_total{mode="idle"}[5m])) * 100)
```
### CPULA 1/5/15;
```
A
node_load1
B
node_load2
C
node_load3

```
### количество свободной оперативной памяти;
```
node_memory_MemAvailable_bytes
```
### количество места на файловой системе.
```
node_filesystem_free_bytes{fstype!~"tmpfs"}
```
