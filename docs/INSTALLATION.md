# 安装与授权 / Installation and licensing

## 中文

### 1. 下载并校验

从对应版本的 Release Assets 下载安装包及 `SHA256SUMS.txt`。文件名与哈希必须与 [下载清单](DOWNLOADS.md) 一致。校验失败时不要运行，重新下载并报告包名。

Windows PowerShell（以下示例为 1.0.1 Windows 包）：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\Ketupa-AI-Fabric-1.0.1-Windows-x64-Setup.exe
```

Linux（在该版本安装包与校验文件所在目录执行）：

```sh
sha256sum --check --ignore-missing SHA256SUMS.txt
```

只校验本地已有的文件；未下载的其他平台文件不会被核验。应至少看到自己下载文件的 `OK`。

### 2. 安装

- Windows x64：阅读适用条款后运行对应 Setup.exe，按安装程序提示操作。
- Debian/Ubuntu amd64：选择适用的 `.deb`，使用系统包管理器安装。例如 `sudo apt install ./ketupa-ai-fabric-linux_1.0.1_amd64.deb`。依赖、权限和系统兼容性由实际目标环境决定。
- Linux x64 TAR.GZ：解压到独立目录，例如 `tar -xzf ketupa-ai-fabric-linux-1.0.1-x64.tar.gz`，按包内说明使用入口。不要把多个版本混装到同一个目录。

本仓库发布流程不会运行安装程序，也不代表目标系统安装成功。历史包按各自原始安装方式操作，文件名不改写。

### 3. 授权与环境

使用产品提供的授权入口导入有效 `.lic`，授权路径与参数以当前版本提示或授权方说明为准，不猜测未公开命令。不在本仓库存放、签发或共享真实授权。需要外部商业软件时，应在有合法许可的机器配置对应工具；购买 Ketupa 授权不等于取得第三方工具许可。

### 4. 验收与反馈

依次核验文件哈希、安装/解压、启动与授权识别，再用不敏感的小案例验证实际流程。保留产品版本、包名、脱敏日志和可重现步骤。仿真输出及工程签核需独立验证；1.0.1 仍为预览状态。

## English

### 1. Download and verify

Download a package and `SHA256SUMS.txt` from the matching Release Assets. Compare the filename and hash with the [download index](DOWNLOADS.md). Do not execute a file whose hash differs; download again and report its filename.

On Windows, use the PowerShell command above to calculate SHA-256. On Linux, run the `sha256sum` command above in the directory containing that version's files. `--ignore-missing` checks only files present locally; it does not verify packages you have not downloaded. Your downloaded file must show `OK`.

### 2. Install

- Windows x64: read the applicable terms and run the matching Setup.exe, following its prompts.
- Debian/Ubuntu amd64: install the suitable `.deb` with the system package manager. The command above illustrates 1.0.1. Dependencies, permissions, and compatibility depend on the actual target system.
- Linux x64 TAR.GZ: extract into a dedicated directory using the command above and follow the instructions inside the package. Do not combine different versions in one installation directory.

The publication process does not execute installers or certify installation on a target system. Historical packages keep their original filenames and installation methods.

### 3. Licensing and environment

Import a valid `.lic` through the product's licensing interface. Follow the current version's prompts or the licensor's instructions for paths and arguments; do not assume undocumented commands. This repository neither stores nor issues real licenses. Configure separately licensed external commercial tools where required. A Ketupa entitlement does not license those tools.

### 4. Acceptance and feedback

Verify the file hash, installation or extraction, startup, and license recognition, then exercise a small non-sensitive real workflow. Record the version, filename, redacted logs, and reproducible steps. Validate simulation results and engineering signoff independently. Version 1.0.1 remains a preview.
