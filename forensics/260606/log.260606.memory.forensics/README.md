# Memory Forensics
[Link to the resource](https://ctf101.org/forensics/what-is-memory-forensics/)

### Overview
- It involves analyzing a image of the system's volatile memory (RAM)
- Highly valuable data since RAM is cleared after a power off and it contains information which will never touch the hard drive
- Clipboard history, running executables, active network connections are some examples of data/clues

### Volatility
- [Volatility 3](https://volatilityfoundation.org/) is a memory extraction framework which can analyze the raw memory dumps ('.raw'/'.vmem')
- We can run specific plugins to rebuild process lists, command histories, etc
    - **Process Trees**(`pstree`): Used for mapping the hierarchy of running programs and spot parent-child connetions, for example a notepad trying to open a command shell
    - **Command Lines**(`cmdline`): Used to extract terminal commands and executables that were executed
    - **Network Connections*(`netscan`): Used to identify communication with external servers

