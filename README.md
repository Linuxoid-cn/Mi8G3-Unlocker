# Mi8G3-Unlocker 全自动版
目前已支持高版本！！！
​本项目是专为搭载骁龙 8g3（Snapdragon 8 Gen3）平台的小米设备打造的 Windows 一键 BL 解锁辅助工具。通过 toUnlock.bat 脚本，实现 HyperOS 全补丁系统下的自动化解锁流程
---
感谢来自 [@Littlenine](https://github.com/LittlenineEnnea) 的核心技术支持

### 📱 已适配支持机型

本脚本目前已精准适配以下 **7 款** 骁龙 8 Gen3 平台设备：

* **Xiaomi 系列：**
    * **Xiaomi 14**
    * **Xiaomi 14 Pro**
    * **Xiaomi 14 Ultra**
* **Redmi 系列：**
    * **Redmi K70 Pro**
    * **Redmi K80**
* **MIX 系列：**
    * **Xiaomi MIX Fold 4**
    * **Xiaomi MIX Flip**

---
## ⚠️ 系统要求与兼容性逻辑 (System Requirements)

本工具利用的底层服务漏洞具有严格的系统环境限制，请在执行前确认目标设备符合以下条件：

### 1. 系统版本 (OS Version)
*   **最低要求**：HyperOS 2.0 (澎湃二) 及以上版本。
*   **排除范围**：HyperOS 1.0 (澎湃一) 及更早版本。
*   **原理说明**：由于澎湃一系统底层缺少该特定的服务组件，相关漏洞利用代码在旧版系统上无法生效。

### 2. 安全补丁级别 (Security Patch Level)
*   **截止日期**：必须等于或低于 **2026年2月1日** 补丁。
*   **修复情况**：自 2026-02-01 补丁后，针对 SELinux 的提权路径已被官方修复。
*   **建议**：若您的系统已更新至 2026 年 2 月更晚的补丁，该工具将无法提权SELinux宽容。
---
### 🚀 核心功能亮点

* **机型目录对齐：** 脚本运行后会根据你选择的机型自动调用对应文件夹（如 `Redmik80`、`Xiaomi14ultra` 等）内的特定配置文件。
* **Windows 一键直达：** 专为 Windows 平台设计，直接运行 `toUnlock.bat` 即可，无需配置冗余的 ADB/Fastboot 环境。
* **自动化引导：** 内置完整的中文交互提示，包含驱动自检、机型匹配确认以及解锁前的安全风险告知。
* **环境兼容性：** 针对 Windows 10/11 优化，确保在解锁高频通讯时数据传输的稳定性。

---

### 🛠️ 使用步骤

1.  **准备阶段：** 手机端开启“开发者选项” -> **USB 调试** 与 **OEM 解锁**，退出小米账号与谷歌账号，并确认已关闭设备查找
2.  **解锁阶段：** 在 Windows 电脑解压本工具包，双击运行目录下的 `toUnlock.bat'脚本
3.  **状态检测：** 双击运行目录下的 'check-unlock.bat'脚本，将开始自动进行检测bl锁与工程abl状态并给出相应的解决方案
4.  **Debug：**双击运行目录下的 'adb-tool.bat'脚本，内置adb fastboot环境以调试
---

### ⚠️ 注意事项与免责声明

* **数据清除：** 解锁 BL **必定会清除所有用户数据**，请务必提前备份。
* **硬件建议：** 建议使用原装数据线，并优先连接电脑后置的 **USB 2.0 接口**。
* **免责条款：** 本脚本仅供技术交流使用。因操作不当或环境问题导致的任何设备故障、保修失效或数据丢失，开发者不承担任何责任。

---

### 💬 反馈与贡献

如果你在上述 7 款机型上遇到“未识别设备”或脚本报错，请提交 **Issue** 并附上报错截图，我会针对该机型文件夹内的逻辑进行修复。
## 👥 贡献者名单 (Contributors)

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/LittlenineEnnea">
        <img src="https://github.com/LittlenineEnnea.png" width="100px;" alt="LittlenineEnnea"/><br />
        <sub><b>Littlenine</b></sub>
      </a><br />
      💡 核心技术 / 💻 解锁boot.img
    </td>
  </tr>
</table>

