# 发布核验范围 / Publication verification scope

## 中文

本页说明本次安装包归档与发布检查的范围，不是产品认证报告。

- 清点三个版本的 12 个原始安装包，逐项计算 SHA-256，并与原发布清单的字节数和哈希比对。上传不重新打包或修改安装包。
- Linux TAR.GZ 与 DEB 的外层归档完成可读性检查及静态展开检查；Beta 的嵌套 Python 运行环境也进行检查，两个 Linux 分发格式中的嵌套环境哈希相同。
- 检查可读取的文件名、文本和二进制头部是否包含真实授权文件、常见凭据或私钥标记。发现的第三方密钥解析器常量及发布者公开验签密钥与真实私钥分别核对。这类扫描不能证明所有敏感信息均已排除。
- Windows 自定义封装及历史加密业务载荷没有完全解码。没有执行安装程序、产品核心、求解器或真实仿真；不能据此宣称其内部全部经过审计，也不能据此保证无漏洞、无恶意行为或工程结果正确。
- GitHub 发布附件逐项核对文件名、字节数与服务端 SHA-256。校验清单可检测下载损坏，但不构成独立的代码签名或安全认证。
- 已识别第三方组件的许可、对应源码及构建材料见 [第三方源码说明](THIRD_PARTY_SOURCES.md)。此项记录不替代完整的软件组成分析、法律审查或目标系统验收。

1.0.1 与 Beta 是预发布。历史 1.0.0 的“稳定通道”仅保留原渠道分类，不表示本次重新完成生产验收。

## English

This page defines the scope of installer archival and publication checks. It is not a product certification report.

- Twelve original installers across three versions are inventoried. Their SHA-256 hashes and byte sizes are compared against the original distribution catalog. Uploading does not repackage or modify installers.
- Outer Linux TAR.GZ and DEB archives are checked for readability and statically extracted. Beta's nested Python runtime is also inspected; the nested runtime hashes match between its two Linux distribution formats.
- Readable filenames, text, and binary headers are checked for real entitlements, common credentials, and private-key markers. Third-party parser constants and the publisher's public verification key are reviewed separately from real private keys. Such scans cannot prove the absence of every sensitive item.
- Custom Windows containers and historical encrypted business payloads are not fully decoded. Installers, product cores, solvers, and real simulations are not executed. This does not establish a complete internal audit, vulnerability or malware clearance, or correct engineering results.
- Every GitHub Release Asset is checked against the expected name, byte size, and server-side SHA-256. Checksums detect download corruption; they are not independent code signatures or security certification.
- See [third-party source information](THIRD_PARTY_SOURCES.md) for identified components, licenses, corresponding source, and build materials. These records do not replace complete software composition analysis, legal review, or target-system acceptance.

1.0.1 and Beta are prereleases. The historical 1.0.0 stable-channel label preserves its original channel classification and does not assert renewed production acceptance.
