# 发布运维 / Release operations

## 中文

1. **准备**：在私有构建环境生成安装包、依赖许可与对应源码资料。不要把核心源码、真实授权、签名私钥或客户数据放入公开资料目录。
2. **检查**：核验版本、文件名、字节数、SHA-256、归档可读性、包内许可及敏感资料；对实际目标系统安装和真实功能分别验收，不能用哈希通过代替。
3. **更新资料**：更新 README、下载表、catalog.json、版本说明及对应版本的 SHA256SUMS.txt。只使用相对仓库链接或官方公开地址，不写维护者本机路径。
4. **草稿上传**：每个版本创建一个 Release 草稿，上传该版本安装包、校验文件和公开清单。使用固定版本标签；不把大二进制提交到 Git。
5. **核对**：逐个比对 GitHub 附件的文件名、大小与服务端 SHA-256，完整后再公开。预览版与 Beta 标为 prerelease，历史版本不冒充新发布。
6. **发布后**：确认下载链接、文件清单和预发布状态，记录远端资产 ID、哈希与发布时间。不要原地替换同版本安装包；字节变化时发布新版本并更新记录。
7. **撤回与恢复**：发现问题先停止推荐受影响版本并将其转为草稿或明确标记撤回，发布修正版及原因。公开后已经下载的文件无法保证收回。
8. **后续同步**：本次为人工授权触发的一次性同步。今后本地增加版本不会自动上传；应重新执行完整发布检查与上传流程，不包含无人值守监听服务。

原始安装包保持不变，因此本仓库 EULA 不会自动加入旧安装界面。后续构建应将适用许可、隐私声明及明确接受步骤纳入安装或激活流程，并完成法律与依赖合规审核。

## English

1. **Prepare:** build installers, dependency notices, and corresponding-source materials privately. Keep core source, real licenses, signing private keys, and customer data out of public documentation.
2. **Check:** verify versions, filenames, byte sizes, SHA-256, archive readability, embedded notices, and sensitive content. Test target-system installation and real features separately; matching hashes are not functional acceptance.
3. **Update documentation:** refresh README, the download table, catalog.json, release notes, and version-specific SHA256SUMS.txt. Use relative repository links or official public URLs, never a maintainer's local paths.
4. **Upload drafts:** create one draft Release per version and attach its installers, checksums, and public catalog. Use fixed version tags and keep large binaries out of Git history.
5. **Verify:** compare every GitHub asset's name, size, and server-side SHA-256 before publishing. Mark previews and Beta as prereleases; do not present historical versions as new builds.
6. **After publication:** check download links, inventories, and prerelease flags; record asset IDs, hashes, and publication time. Do not replace a released binary in place; changed bytes require a new version and updated records.
7. **Withdraw and recover:** stop recommending an affected version, withdraw it or clearly mark it as withdrawn, and publish a correction with an explanation. Copies already downloaded cannot reliably be recalled.
8. **Future synchronization:** this is a user-authorized, one-time synchronization. New local versions are not automatically uploaded; repeat the checked publication workflow. No unattended folder watcher is included.

Original installers remain unchanged, so this repository's EULA is not automatically inserted into old installation dialogs. Future builds should integrate the applicable license, privacy notice, and explicit acceptance into installation or activation and complete legal and dependency-compliance review.
