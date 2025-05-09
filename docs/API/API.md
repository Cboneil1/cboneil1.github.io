# Message Communication

This is the style of communication decided by the group to best send messages between each other's boards. This controller will begin making a message which starts at the values [A][Z][ID][ID][SA] in Hex. The message will end when it receives the values [S][T][0x0A] in Hex. The message type will be at most 64 bytes long. These are the established norms for our protocol from the requirements.

---

## Message Structure

**Example Message Structure:** [A][Z][SENDER][RECEIVER][MESSAGE TYPE][VALUE][S][T]

---

## Sender IDs

| Name     | ID  | Value |
|----------|-----|-------|
| Brendon  | B   | 0x42  |
| Zack     | Z   | 0x5A  |
| Carter   | C   | 0x43  |

---

## Receiver IDs

| Name      | ID  | Value |
|-----------|-----|-------|
| Brendon   | B   | 0x42  |
| Zack      | Z   | 0x5A  |
| Carter    | C   | 0x43  |
| Broadcast | X   | 0x58  |

---

## Message Type

| Message Type    | Value | Type  |
|-----------------|--------|--------|
| Motor (Freq)    | 1      | 0x31   |
| Pitch (up/d)    | 6      | 0x36   |

---

## Values

| Message Type     | Value   | Type       |
|------------------|---------|------------|
| Motor (Freq)     | 0–255   | 0x00–0xFF  |
| Pitch Up/Down    | 0–1     | 0x00–0x01  |

---

## Error Types

| Error Type           | Value  |
|----------------------|--------|
| Wrong start sequence | 0x30   |
| Wrong header         | 0x31   |
| Wrong Receiver       | 0x32   |
| Wrong Sender         | 0x33   |
| Wrong Message Type   | 0x34   |
| Wrong Message ending | 0x35   |
