# 非官方测试包 / Unofficial community test build

Windows 11 x64; tested only on build 26340.9750 with two displays. Based on official TranslucentTB 2026.2 portable files; only ExplorerTAP.dll replaced, plus a fresh generic Clear configuration. This is not an official signed release. The repair DLL is locally built and unsigned.

## 下载 / Downloads

- [运行包 / Portable test build](TranslucentTB-2026.2-26340-x64-community-test.zip)
- [完整对应源码与构建说明 / Complete corresponding source and build instructions](TranslucentTB-2026.2-26340-fix-source.zip)
- [SHA-256](SHA256SUMS.txt)

## 中文用法

1. 完整解压运行包；不要在 ZIP 内运行。
2. 从托盘退出所有 TranslucentTB，包括商店版。
3. 在任务管理器中重新启动 Windows 资源管理器，卸载旧模块。桌面和任务栏会短暂闪烁；不要在资源管理器复制文件时执行。
4. 运行解压后的 TranslucentTB.exe，选择 Clear（透明）外观。
5. 一次只运行一个版本。恢复原版时，退出测试版，重启资源管理器，再启动原版。

本包不修改注册表、不设置开机启动，不包含个人配置备份。完整中英文说明和许可证在压缩包内。

## English usage

1. Extract the entire portable ZIP. Do not run it inside the ZIP.
2. Exit all TranslucentTB instances, including the Store version.
3. Restart Windows Explorer in Task Manager to unload the previous module. The desktop/taskbar will blink briefly; avoid this during Explorer file copies.
4. Run the extracted TranslucentTB.exe and select Clear.
5. Run one version at a time. To revert, exit this build, restart Explorer, then run the original version.

No registry or startup changes are made. No personal configuration backups are included. Full bilingual instructions and license notices are inside the ZIP.

## Validation and limits / 验证与限制

Both taskbars visually became transparent. Clear, Acrylic and border visibility service calls passed on both; restarting the app passed. The bundled DLL matches the tested DLL exactly. The fresh public configuration was checked structurally; the repackaged ZIP has not been separately run on another PC. Full develop build/CI, full Windows reboot, other OS builds and all appearance modes remain untested. This does not establish a fix for the separately reported RPC_E_WRONG_THREAD error.

[Source patch / 源码补丁 PR #1376](https://github.com/TranslucentTB/TranslucentTB/pull/1376). Complete release-base source with the patch, dependency sources/licenses and a build recipe is provided alongside the binary for GPL-3.0 compliance. Upstream release base: d4636e439865df0a1a1419db408e055740ce5c74.
