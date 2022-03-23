## Interrupt I/O

- Interrupts allows a device to change the flow of control in the CPU
- Modern OS are **interrupt driven** (event driven)
- Hareware may trigger an interrupt at any time by sendinng a **sigal** to CPU
- Software may trigger an interrupt either by an error or by a user request for an OS service (**system call**)
- Software interrupt also called trap

## Common Function of Interrupts

- Through interrupt vector (知道 system function 位址)
- Do service routines (interrupt handlers)
- Interrupt architecture 必須紀錄被中斷程式的 address
- Incoming interrupts may be **disable** while another interrupt is being processed => in other to prevent a lost interrupt
