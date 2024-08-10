## Objective
learn the differences of a nodejs proccess when started manually v.
managed with systemd

## Things learned
- to view stdout or console.log() output from a process started with systemd
  use the command: 

  ```
  sudo journalctl -u service_name
  ```
