# RedisInsight Docker Extension


RedisInsight is an intuitive and efficient GUI for Redis. It allows developers to interact with your databases and manage your data—with built-in support for most popular Redis modules. 

It is an open source Redis GUI tool that allows you to visualise, monitor, and optimize while developing your applications with Redis.

This repository show how to run Redis GUI as a single-click installation using RedisInsight Docker Extension.





> This is Work-in-progress
- [x] Building Compose File
- [x] Constructing UI
- [ ] Final Testing


RedisInsight is an intuitive and efficient GUI for Redis, allowing you to interact with your databases and manage your data—with built-in support for most popular Redis modules. It is an open source Redis GUI tool that allows you to visualise, monitor, and optimize while developing your applications with Redis.


<img width="1359" alt="image" src="https://user-images.githubusercontent.com/34368930/196146699-950f387a-3133-48ab-bb4e-5cf266745123.png">



## Getting Started

### Pre-requisite

- Docker Desktop 4.12


## 1. Clone the repository


```shell
 git clone https://github.com/collabnix/redisinsight-docker-extension
```

## 2. Build the Extension

```shell
 make build-extension
```
#### If you run into error: Failed to solve with frontend dockerfile.v0: failed to create LLB definition
```
export DOCKER_BUILDKIT=0
export COMPOSE_DOCKER_CLI_BUILD=0
```


## 3. Install the Extension

```shell
 docker extension install <name-of-extension>
 ```
 
 
 Open Docker Dashboard to see RedisInsight Extension already up and running.
 
 ## Connecting to the Local Redis Database
 
 ### Step 1. Toggle to agree to the license terms and click "Confirm"
 
 <img width="1157" alt="image" src="https://user-images.githubusercontent.com/313480/188198634-c51317d3-2379-4b64-953f-2e315861503d.png">

### Step 2. Click "Apply Changes" to connect to the default Redis database
 
 <img width="1226" alt="image" src="https://user-images.githubusercontent.com/34368930/196146825-3cd9eab6-1917-40d6-a8d8-13edf6a41fd2.png">



This extensions runs local Redis database too. It is included for testing purpose.

### Step 3. Add a Redis key and assign a value

<img width="1039" alt="image" src="https://user-images.githubusercontent.com/34368930/196147521-2e5bdff7-4427-4b7a-a85f-8fecd222e626.png">
<img width="1047" alt="image" src="https://user-images.githubusercontent.com/34368930/196147709-ae0b3d49-1037-40b0-af75-21f35d35a888.png">

### Step 4. Verify the key/value

<img width="1106" alt="image" src="https://user-images.githubusercontent.com/34368930/196147804-0bf494b1-e36b-407d-bc7a-c185b4455ca7.png">





### Important Notes:
- This Extension only works for the default localhost
- This extension doesn't work with the remote Redis Cloud instance
- This extension doesn't work with the localhost with port other than 6379
