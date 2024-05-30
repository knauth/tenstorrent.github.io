# noc_semaphore_set

```cpp
void noc_semaphore_set(volatile uint32_t *sem_addr, uint32_t val)
```

Sets the value of a local L1 memory address on the Tensix core executing this function to a specific value. This L1 memory address is used as a semaphore of size 4 Bytes, as a synchronization mechanism. Also, see *noc_semaphore_wait*.

Return value: None

| Argument      | Description                          | Type      | Valid Range        | Required       |
|---------------|--------------------------------------|-----------|--------------------|----------------|
| sem_addr      | Semaphore address in local L1 memory | uint32_t  | 0..1MB             | True           |
| val           | Value to set the semaphore to        | uint32_t  | Any uint32_t value | True           |
