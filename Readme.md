# ZenPerl 🚀

ZenPerl is a high-performance **Minecraft server jar** built as a fork of [Paper](https://github.com/PaperMC/Paper).

Unlike traditional server software that preserves legacy Bukkit limitations, ZenPerl bypasses structural bottlenecks to introduce **native performance patches** and a **modernized, lightweight API layer** designed to make server-side development faster, cleaner, and zero-overhead.

## ✨ Core Features & Unique APIs

* **Ultra-Fast Packet API:** Native, high-velocity packet interception and injection baked straight into the core—eliminating the heavy reflection overhead of external packet libraries.
* **Simplified Asynchronous Utilities:** High-level API frameworks to offload intensive tasks (NBT parsing, database queries, mathematical calculations) cleanly away from the main tick thread.
* **Optimized Raycasting & Math Vectors:** Custom, native raycasting pipelines for lightning-fast entity tracking, custom mechanics, and weapon tracking with minimal CPU footprints.
* **Streamlined Component Pipeline:** Fluent wrapper interfaces for Mojang's modern Data Components, allowing developers to manipulate item and entity metadata instantly.
* **Aggressive Thread & Engine Optimizations:** Hardcoded structural enhancements targeting event listener pipelines, entity brain tracking, and chunk processing.

## 🛠️ Building From Source

ZenPerl utilizes the modern `paperweight` toolchain to manage decompilation, mapping, and patching.

### Prerequisites
* **Java 25** (required by the current Gradle toolchain)
* A git-configured terminal

### Compilation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pero-Gamer-Dev/ZenPerl.git
   cd ZenPerl
   ```

2. **Initialize and apply development patches:**
   ```bash
   ./gradlew applyPatches
   ```

3. **Rebuild the production-ready server jar:**
   ```bash
   ./gradlew :paper-server:createPaperclipJar
   ```
   Your compiled server binary will be located in `paper-server/build/libs/`.

## 📄 License
ZenPerl includes upstream projects under their respective licenses. See [License](License) for details.
