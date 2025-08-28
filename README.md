## [详细教程](http://docs.yw-games.top/posts/tutorial/modpack/packwiz.html)

以下是一些在管理 Packwiz 项目时常用的命令，方便快速操作和维护整合包。这些命令可以帮助你更高效地创建、更新整合包。

- **`packwiz init`**  
  初始化一个新的整合包，生成 `pack.toml` 和 `index.toml` 文件，用于定义整合包的基本信息和资源索引。

- **`packwiz refresh`**  
  更新整合包的 `index.toml` 文件，重新扫描项目目录中的文件并更新其哈希值，以确保索引与实际文件一致。每次手动添加、删除或编辑文件后都需要运行此命令。

- **`packwiz server -p <port>`**
  启动一个本地服务器，提供整合包更新服务。

- **`packwiz curseforge install [mod]`**  
  从 CurseForge 安装指定的 Mod 到整合包中，自动生成对应的 `.pw.toml` 文件。

- **`packwiz modrinth install [mod]`**  
  从 Modrinth 安装指定的 Mod 到整合包中，自动生成对应的 `.pw.toml` 文件。

- **`packwiz update [mod]`**  
  更新指定 Mod 到最新版本，自动从 CurseForge 或 Modrinth 下载最新文件。

- **`packwiz update --a`**  
  更新整合包中的所有 Mod 到最新版本，简化批量更新流程。

- **`packwiz curseforge detect`**  
  扫描整合包中的文件，检测哪些文件可在 CurseForge 上找到，并将其配置为从 CurseForge 下载。

使用 `--help` 标志可以获取每个命令的详细说明，例如 `packwiz init --help`。