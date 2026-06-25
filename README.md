````markdown
# Container Runtime Process Isolation

A lightweight container runtime built in **C++17** for Linux using **Linux Namespaces** and **cgroups v2**. This project demonstrates how operating-system level virtualization works by creating isolated execution environments with configurable resource limits.

---

## 🚀 Features

- Process isolation using Linux Namespaces
- Resource management using cgroups v2
- Filesystem isolation using `chroot`
- Command-line interface (CLI)
- Modular C++17 codebase
- CMake build system

---

## 🛠️ Tech Stack

- **Language:** C++17
- **Operating System:** Linux
- **Kernel Features:**
  - PID Namespace
  - Mount Namespace
  - UTS Namespace
  - cgroups v2
- **Build System:** CMake

---

## 📌 Project Overview

This project implements the core building blocks of a lightweight container runtime.

Each container runs inside its own isolated environment where:

- Processes cannot view host processes.
- Hostname is isolated.
- Filesystem is separated from the host.
- CPU and memory limits can be applied.
- Applications execute securely with restricted access.

The project is designed for learning Linux kernel internals and operating-system virtualization concepts.

---

## 📂 Project Structure

```text
container-runtime-process-isolation/
├── src/                # Source files
├── include/            # Header files
├── cmake/              # CMake modules
├── config/             # Sample configuration files
├── CMakeLists.txt
├── README.md
└── plan.md
````

---

## ⚙️ Prerequisites

* Linux (Ubuntu 22.04+ recommended)
* g++
* CMake
* make
* Root privileges
* Linux kernel with cgroups v2 enabled

---

## 🔨 Build

```bash
git clone https://github.com/Nancy-311/container-runtime-process-isolation.git

cd container-runtime-process-isolation

mkdir build

cd build

cmake ..

make
```

---

## ▶️ Usage

Run the runtime using:

```bash
sudo ./mnu-os run --config ../config/sample.json
```

The runtime will:

* Create isolated PID namespace
* Create isolated Mount namespace
* Create isolated UTS namespace
* Apply filesystem isolation
* Configure cgroups
* Launch the target application

---

## 🗺️ Roadmap

### ✅ Phase 1 — Core Runtime

* [ ] PID Namespace
* [ ] Mount Namespace
* [ ] UTS Namespace
* [ ] cgroups v2
* [ ] Memory Limits
* [ ] CPU Limits
* [ ] Process Limits
* [ ] Filesystem Isolation

### 🚧 Phase 2 — Configuration

* [ ] JSON Configuration
* [ ] YAML Support
* [ ] CLI Improvements
* [ ] Configuration Validation

### 🔒 Phase 3 — Security

* [ ] User Namespace
* [ ] pivot_root
* [ ] Capability Dropping
* [ ] Seccomp Support

### 🌐 Phase 4 — Networking

* [ ] Network Namespace
* [ ] Bridge Networking
* [ ] Port Forwarding
* [ ] DNS Support

### 🚀 Phase 5 — Advanced Features

* [ ] Container Logging
* [ ] Monitoring
* [ ] Image Management
* [ ] Image Builder

### ⚡ Phase 6 — Performance

* [ ] Startup Optimization
* [ ] Multi-threading
* [ ] Health Checks
* [ ] Basic Orchestration

---

## 🔧 Future Improvements

* Unit Tests
* Integration Tests
* CI/CD Pipeline
* Docker Development Environment
* API Documentation
* Performance Benchmarking

---

## 📄 License

This project is intended for educational and learning purposes.

---

## 👩‍💻 Author

**Nancy Sagar**

GitHub: https://github.com/Nancy-311

```
```
