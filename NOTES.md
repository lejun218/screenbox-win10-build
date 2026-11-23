## Screenbox for Windows 10 (x64)

由 [huynhsontung/Screenbox](https://github.com/huynhsontung/Screenbox) 源码在现场编译生成的 x64 MSIX 安装包。

- 编译配置：Release / x64 / UWP，.NET AOT，`UapAppxPackageBuildMode=SideloadOnly`
- 签名：构建时生成的临时自签名证书（`Screenbox_TemporaryKey.cer`）
- 适用系统：Windows 10 1903 (10.0.18362) 及以上 64 位

### 安装

1. 开启"设置 → 更新和安全 → 开发者选项 → 开发人员模式"。
2. 右键 `Screenbox_TemporaryKey.cer` → 安装证书 → 本地计算机 → 放入"受信任的根证书颁发机构"。
3. 双击 `.msix` 安装，或执行 `Add-AppxPackage -Path .\Screenbox_x.x.x.x_x64.msix`。

详细步骤见压缩包内 `INSTALL.txt`。
