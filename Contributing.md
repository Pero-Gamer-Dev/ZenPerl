# Contributing to ZenPerl

We welcome contributions focused on improving server performance, reducing memory footprints, and expanding our unique API layout. Please review the following guidelines before submitting your changes.

## 🧱 Patch Management Workflow

ZenPerl relies heavily on automated Git patches built on top of Paper code internals. Do not modify the decompiled server source files directly without utilizing the Gradle workflow.

1. **Setup Workspace:** Run `./gradlew applyPatches` to set up your local development environment.
2. **Make Changes:** Edit the code inside the specific submodule projects.
3. **Rebuild Patches:** Once you verify your changes work, run:
   ```bash
   ./gradlew rebuildPatches
   ```
4. **Commit:** Commit the newly generated or modified `.patch` files located in the `patches/` directories.

## 📝 Code Guidelines

* **Performance First:** ZenPerl aims for peak efficiency. Avoid heavy use of reflection, unnecessary objects in high-frequency tick loops, and unoptimized stream mappings.
* **Keep APIs Simple:** Custom API interfaces should be fluent, documented, and intuitive for plugin developers.
* **Maintain Mappings:** Ensure all custom internal logic hooks cleanly into Mojang's native mappings (NMS).

## 🐛 Reporting Issues

Please open an issue describing the exact reproduction steps, the server version hash, and any relevant thread dump or profile logs (such as Spark or timings profiles) if reporting performance bottlenecks.
