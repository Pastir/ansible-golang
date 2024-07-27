Role Name
=========
pastir.go

Installing golang release

Role Variables
--------------
```
# Go language SDK version number
# default: 1.20
# support: all version
``` 
  - ```- go_version: "go1.20"```
```
# OS
# default: "linux"
# support: 
   - linux
``` 
 - ```- go_os: "linux"```

 ```
# architecture
# default: "amd64" 
# support: 
     - amd64
     - 386
 ```
 - ```- go_arch: "amd64"``` 

  ```
# path install bin golang release
# default: /usr/local/go1.20
  ```
 -  ```- go_dir: "/usr/local/go1.20" ```
 
```
# export PATH 
# default: false
```
 -  ```-go_env_path: false ```


Example Playbook
----------------

```
  - role: pastir.go
      vars:
        go_version: 'go1.22.5'
        go_os: 'linux'
        go_arch: 'amd64'
        go_dir: '/usr/local/go1.22.5'
        go_env_path: no 
```

License
-------

BSD

Author Information
------------------
Pastir Ivan
