# API

## Message Structure

| Start Value 1            | Start Value 2         | From   | To     | Data Byte 1       | Data N        | End Value 1 | End Value 2 |
| ------------------------ | --------------------- | ------ | ------ | ----------------- | ------------- | ----------- | ----------- |
| 0x41                     | 0x5a                  | 0xXX   | 0xXX   | Message Select    | 56 Byte Limit | 0x59        | 0x42        |

## Members

| Brendan            | Carter         | Sivanee   | Zach     |
| ------------------ | -------------- | --------- | -------- |
| 0x42               | 0x43           | 0x53      | 0x5a     |

### Byte 1 Structure

|               | Byte 1         |
|---------------|----------------|
| **Variable Name** | `message_type` |
| **Variable Type** | `uint8_t`      |
| **Min Value**     | 0              |
| **Max Value**     | 20             |
| **Example**       | 1              |

## Pitch Info Structure

|                   | Byte 1         | Byte 2          | Byte 3        |
|-------------------|----------------|-----------------|---------------|
| **Variable Name** | `Pitch Info`   | `Source Select` | `Pitch Value` |
| **Variable Type** | `uint8_t`      | `uint8_t`       | `int8_t`      |
| **Value**         | 1              | ex: 1           | ex: 176       |

### Pitch Info Byte 2 Structure

|               | Byte 2                      |
|---------------|-----------------------------|
| **Variable Name** | `Source Select`         |
| **Variable Type** | `uint8_t`               |
| **Min Value**     | 0                       |
| **Max Value**     | 1                       |
| **Example**       | 0 for Mic, 1 for Button |

### Pitch Info Byte 3 Structure

|               | Byte 3            |
|---------------|-------------------|
| **Variable Name** | `Pitch Value` |
| **Variable Type** | `uint8_t`     |
| **Min Value**     | 0 Hz          |
| **Max Value**     | 255 Hz        |
| **Example**       | 75Hz          |


## Up/Down Pitch Structure

|                   | Byte 1         | Byte 2          |
|-------------------|----------------|-----------------|
| **Variable Name** | `Pitch Adjust` | `High or Low`   |
| **Variable Type** | `uint8_t`      | `bool`          |
| **Value**         | 2              | ex: False       |

### Up/Down Byte 2 Structure

|               | Byte 3            |
|---------------|-------------------|
| **Variable Name** | `High or Low` |
| **Variable Type** | `bool`        |
| **Min Value**     | False Down    |
| **Max Value**     | True Up       |

