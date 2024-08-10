## Objective
learn the differences of a nodejs proccess when started manually v.
managed with systemd

## Things learned
- to view stdout or console.log() output from a process started with systemd
  use the command: 
  ```
  sudo journalctl -u service_name
  ```
- the working directory of a node process started with systemd must be set with
  the [Service] directive `WorkingDirectory = /path/to/working/directory`,
  otherwise will default to the root directory when systemd is running as a system
  instance and the user's home directory if run as a user.
