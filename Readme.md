# ZenPerl 🚀

ZenPerl is a next-generation, high-performance **Minecraft server jar** built as a fork of [Paper](https://github.com). It is engineered specifically for hyper-demanding production networks that require absolute raw performance, stripped-back latency, and streamlined developer interfaces.

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
* **Java 21** or higher (Depending on target Minecraft version)
* A git-configured terminal

### Compilation Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd ZenPerl
   ```

2. **Initialize and apply development patches:**
   ```bash
   ./gradlew applyPatches
   ```

3. **Rebuild the production-ready server jar:**
   ```bash
   ./gradlew createReobfPaperclipJar
   ```
   Your compiled server binary will be located in the `build/libs/` directory.

## 📄 License
ZenPerl is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.
