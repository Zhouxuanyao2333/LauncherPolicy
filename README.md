# Kilim Minecraft Launcher — 项目政策与法律声明

> 中文版 | [English Version](#english-version)
>
> 本文档包含：隐私政策、第三方信息收集政策、用户协议、开源许可与版权声明。
> This document includes: Privacy Policy, Third-Party Data Collection Policy, Terms of Service, Open Source License and Copyright Notice.

---

## 目录 / Table of Contents

### 中文版

- [文档说明](#doc-zh)
- [隐私政策](#privacy-zh)
- [第三方信息收集政策](#third-party-zh)
- [用户协议](#terms-zh)
- [开源许可与版权声明](#license-zh)
- [English Version](#english-version)

### English Version

- [Document Notice](#doc-en)
- [Privacy Policy](#privacy-en)
- [Third-Party Data Collection Policy](#third-party-en)
- [Terms of Service](#terms-en)
- [Open Source License and Copyright Notice](#license-en)

---

<a id="doc-zh"></a>
## 文档说明

**生效日期：2026 年 10 月 31 日**

**最后更新：2026 年 10 月 31 日**

Kilim Minecraft Launcher（以下简称“本启动器”或“本软件”）是一个**开源的、非商业的 Minecraft 启动工具**。本启动器不是 Minecraft 官方启动器，与 Mojang Studios、Microsoft 或其关联公司没有隶属、赞助、认可或其他官方关系。

本文档用于说明本启动器的隐私政策、第三方信息收集政策、用户协议、开源许可与版权声明。本文档应与本启动器的实际代码行为和发布版本保持一致；如果本文档与当地强制性法律规定冲突，以当地强制性法律规定为准。

本启动器通过以下方式明确项目边界并降低用户误解：

1. **本启动器不包含后门、隐藏遥测、静默数据上传、远程控制或账号窃取逻辑。**
2. **本启动器没有开发者服务器、没有官方网站、没有账户系统，开发者不会接收、存储或上传用户的账户令牌、密码或个人数据。**
3. **正版登录过程中获取的令牌仅保存在用户本地设备，绝不上传至开发者或任何第三方服务器。**
4. **下载功能仅用于获取 Minecraft 游戏运行所需文件，不提供破解、绕过正版验证、盗版分发、外挂、作弊或账号窃取功能。**
5. **本启动器是开源工具，源代码采用 MIT 许可证发布，供用户和公众审计。**
6. **用户应自行确保其使用行为符合当地法律、Minecraft 最终用户许可协议（EULA）以及微软服务协议。**

本文档不构成法律意见。项目发布者应根据实际代码、发布地区和适用法律，在必要时咨询专业法律人士。

---

<a id="privacy-zh"></a>
## 隐私政策

**生效日期：2026 年 10 月 31 日**

### 1. 我们收集的信息

**本启动器不收集任何个人信息。**

本启动器没有后端服务器、没有遥测（Telemetry）、没有崩溃上报、没有使用统计、没有广告或分析 SDK，也没有任何形式的网络回传。开发者没有能力通过本启动器接收、存储、出售或分享用户的个人信息。

用户的账户令牌、游戏路径、Java 路径、实例信息、设置和日志等数据，均只保存在用户自己的电脑上。默认情况下，本启动器的运行时数据位于可执行文件同级的 `KilimLauncher` 文件夹中。

### 2. 微软正版登录与账户信息

本启动器支持微软正版登录，使用微软官方 OAuth 2.0 设备代码流（Device Code Flow）。

- 登录过程主要在微软官方服务器之间完成，包括 `login.microsoftonline.com`、`user.auth.xboxlive.com`、`xsts.auth.xboxlive.com`、`api.minecraftservices.com` 等。
- 本启动器仅作为 OAuth 客户端，在用户电脑与微软官方服务器之间转发认证请求和令牌。
- 本启动器不会要求用户在本启动器内输入微软账户密码。设备代码流通常由用户在浏览器中完成授权。
- 获取到的访问令牌（Access Token）和刷新令牌（Refresh Token）仅保存在用户本地设备的 `accounts.json` 文件中。
- **正版登录收集信息不会上传。** 本启动器不会将微软账户令牌、Minecraft 访问令牌、刷新令牌、密码或账户资料上传至开发者服务器、开发者控制的第三方服务器或任何非必要的第三方服务。
- 开发者看不到、拿不到，也不会主动收集用户的微软账户密码或令牌内容。

用户应妥善保护本地 `accounts.json` 文件，因为该文件可能包含可用于访问账户的敏感令牌。用户可以通过删除 `KilimLauncher` 文件夹清除本地账户数据。

### 3. 下载功能与版权

本启动器的下载功能仅用于从 Minecraft 官方资源服务器以及社区镜像源获取游戏运行所需文件，例如版本清单、版本 JSON、客户端 JAR、依赖库和资源文件。

- **下载功能不提供破解。**
- 本启动器不提供任何破解、绕过正版验证、盗版分发、外挂、作弊或账号窃取功能。
- 本启动器不分发 Minecraft 游戏本体文件。
- 下载和运行 Minecraft 需要用户已经拥有合法的 Minecraft 账户，或仅在法律和 EULA 允许的范围内用于测试、单人游戏等用途。
- 离线模式仅用于测试或单人游戏等场景，不代表开发者鼓励、支持或认可盗版。
- Minecraft 游戏本体、游戏文件、Mojang 商标及相关知识产权归 Mojang Studios / Microsoft 所有。

### 4. 日志文件

本启动器会在本地生成运行日志，例如 `app.log`、`game.log`、`startup.log`、`crash.log`、`MainWindowLog.txt` 等，用于用户自行排查问题。

- 日志仅保存在用户本地设备。
- 日志不会自动上传至开发者或任何第三方服务器。
- 日志设计上不记录用户的微软账户密码或正版登录令牌。
- 用户应注意，日志可能包含本地路径、系统信息、错误堆栈、游戏输出等信息。分享日志前应自行检查并删除敏感内容。

### 5. 你的权利

由于开发者不收集用户数据，用户无需向开发者请求删除、导出或更正数据。所有数据均在用户自己的电脑上。用户可以随时：

- 删除 `KilimLauncher` 文件夹以清除本地账户、实例、日志和配置数据。
- 使用防火墙、网络监控工具或抓包工具验证本启动器的网络行为。
- 在不使用正版登录或在线功能的情况下，仅使用本地已有实例进行离线测试。
- 停止使用本启动器。

### 6. 政策更新

开发者可能更新本隐私政策。更新后的政策将在项目文档页面公布。继续使用本启动器即视为接受更新后的政策。如果用户不同意更新后的政策，应停止使用本启动器。

---

<a id="third-party-zh"></a>
## 第三方信息收集政策

**生效日期：2026 年 10 月 31 日**

本启动器本身不收集任何个人信息，也没有开发者服务器。但在使用过程中，用户的设备会与以下第三方服务通信。这些第三方服务可能按照其各自隐私政策记录标准 HTTP 请求信息，例如 IP 地址、请求时间、请求路径、User-Agent、错误码等。开发者无法控制这些第三方服务的数据处理行为，也不对其隐私实践承担责任。

### 1. 微软、Xbox Live 与 Minecraft 服务

**涉及功能：** 微软正版登录、Xbox Live 认证、XSTS 认证、Minecraft 档案获取。

**可能通信的地址：**

- `login.microsoftonline.com`
- `user.auth.xboxlive.com`
- `xsts.auth.xboxlive.com`
- `api.minecraftservices.com`

**数据接收方：** Microsoft Corporation / Mojang Studios。

**说明：** 当用户选择正版登录时，用户会在浏览器中与微软服务器交互完成 OAuth 授权。微软会按照其隐私声明处理用户数据。本启动器不会将用户的微软账户信息传输给微软官方服务器以外的任何一方。**正版登录收集信息不会上传至开发者服务器。**

### 2. Minecraft 官方资源服务器

**涉及功能：** 获取版本列表、版本 JSON、客户端 JAR、依赖库、资源文件。

**可能通信的地址：**

- `piston-meta.mojang.com`
- `piston-data.mojang.com`
- `resources.download.minecraft.net`
- `libraries.minecraft.net`
- 其他 Mojang / Microsoft 官方 Minecraft 资源域名

**数据接收方：** Microsoft Corporation / Mojang Studios。

**说明：** 下载游戏文件时，用户的 IP 地址和标准 HTTP 请求信息可能被 Mojang 服务器记录。这是正常网络请求行为。本启动器不会在这些请求中附加额外追踪信息。

### 3. 社区镜像源 BMCLAPI

**涉及功能：** 在官方源不可用或较慢时，可选地加速下载 Minecraft 文件。

**可能通信的地址：**

- `bmclapi2.bangbang93.com`
- 该镜像服务可能重定向到的其他节点域名

**数据接收方：** BMCLAPI 项目维护者及相关镜像节点运营者。

**说明：** BMCLAPI 是社区维护的 Minecraft 下载镜像。用户的 IP 地址和标准 HTTP 请求信息可能被该服务记录。本启动器默认优先使用官方源，仅在官方源不可用、失败或根据下载策略需要回退时使用镜像。用户应自行阅读 BMCLAPI 及其节点服务的相关政策和说明。

### 4. GitHub

**涉及功能：** 源代码托管、文档托管、问题反馈、发布页面访问。

**可能通信的地址：**

- `github.com`
- GitHub 相关子域名

**数据接收方：** GitHub, Inc. (Microsoft)。

**说明：** 如果用户访问本项目的 GitHub 仓库、文档或发布页面，GitHub 会按照其隐私政策记录访问行为。本启动器本身不会自动检查更新，除非用户手动触发相关操作或未来版本明确说明。

### 5. 用户网络环境与代理

如果用户使用代理软件、VPN、防火墙、网络加速器或其他网络工具，用户的网络流量可能先经过这些工具。这些工具的隐私实践由用户自行选择和负责。开发者不控制、不运营也不承担用户代理环境的责任。

### 6. 第三方政策变更

第三方服务可能更新其隐私政策、服务条款或数据处理方式。开发者建议用户定期阅读相关第三方政策。本启动器不控制第三方服务，也不对其数据处理行为作出保证。

---

<a id="terms-zh"></a>
## 用户协议

**生效日期：2026 年 10 月 31 日**

**重要提示：** 在使用 Kilim Minecraft Launcher（以下简称“本启动器”）之前，请仔细阅读本协议。使用本启动器即表示用户同意接受本协议的全部条款。如果用户不同意本协议的任何内容，请立即停止使用本启动器。

### 1. 软件性质

1.1 本启动器是一个开源的、非商业的 Minecraft 启动工具，采用 MIT 许可证发布。

1.2 本启动器不是 Minecraft 官方启动器，与 Mojang Studios、Microsoft 或其关联公司没有隶属、赞助、认可或其他官方关系。

1.3 本启动器不分发、不破解、不绕过 Minecraft 的正版验证系统。下载和运行 Minecraft 需要用户已经拥有合法的 Minecraft 账户，或仅在法律和 EULA 允许的范围内使用。

1.4 本启动器不包含后门、隐藏遥测、静默数据上传、远程控制或账号窃取逻辑。源代码采用 MIT 许可证发布，供用户和公众审计。

### 2. 许可与限制

2.1 用户可以：

- 自由使用、复制、修改、合并、发布、分发本启动器的源代码；
- 将本启动器用于个人或商业目的，但游戏本身仍需合法授权；
- 在遵守 MIT 许可证和适用法律的前提下制作衍生作品。

2.2 用户不得：

- 将本启动器用于任何违反当地法律的行为；
- 使用本启动器下载、分发或传播盗版 Minecraft 游戏文件；
- 修改本启动器以绕过微软或 Mojang 的正版验证机制；
- 将本启动器伪装成官方启动器进行钓鱼、欺诈或误导；
- 在本启动器基础上添加后门、恶意代码、账号窃取、外挂、作弊或未经授权的数据收集功能；
- 删除或伪造本启动器中的版权声明、许可证声明或商标声明。

### 3. 知识产权

3.1 本启动器的源代码版权归开发者所有，采用 MIT 许可证发布。

3.2 Minecraft 游戏本体、游戏文件、Mojang 商标及相关知识产权归 Mojang Studios / Microsoft 所有。本启动器不包含任何 Minecraft 游戏本体文件。

3.3 本启动器中使用的第三方库，例如 Avalonia、Avalonia.Skia、SkiaSharp、NAudio、LiquidGlassAvaloniaUI 等，其版权归各自作者所有，详见其开源许可证。

### 4. 免责声明

4.1 本启动器按“现状”提供，不附带任何明示或默示的担保，包括但不限于适销性、特定用途适用性、非侵权性或无错误运行的担保。

4.2 在适用法律允许的最大范围内，开发者不对因使用或无法使用本启动器而导致的任何直接、间接、偶然、特殊或后果性损害承担责任，包括但不限于：

- 账户被封禁、限制或处罚；
- 数据丢失、损坏或泄露；
- 系统损坏、软件冲突或病毒感染；
- 因违反 Minecraft EULA 或微软服务协议导致的后果；
- 因第三方服务、镜像源、网络环境或用户操作导致的后果。

4.3 使用本启动器完全由用户自行承担风险。如果用户担心账户安全或合规风险，应使用 Minecraft 官方启动器。

### 5. 用户责任

5.1 用户确认其已经拥有合法的 Minecraft 账户，或仅将本启动器用于法律和 EULA 允许的离线测试、单人游戏等用途。

5.2 用户同意遵守 Minecraft 最终用户许可协议（EULA）、微软服务协议以及适用的当地法律。

5.3 用户理解并同意：使用第三方启动器可能涉及与 Minecraft EULA 相关的风险，可能导致账户受到限制。开发者不鼓励、不支持、也不对任何因使用本启动器导致的账户问题承担责任。

5.4 用户应自行保护本地账户令牌、日志、配置文件和其他敏感数据。

### 6. 协议变更与可分割性

6.1 开发者可能随时更新本协议。更新后的协议将在项目文档页面公布。继续使用本启动器即视为接受更新后的协议。

6.2 如果本协议的任何条款被有管辖权的机构认定为无效或不可执行，该条款应在最小必要范围内调整或删除，其余条款继续有效。

6.3 中英文版本如有不一致，以中文版本为准，但当地强制性法律规定另有要求的除外。

---

<a id="license-zh"></a>
## 开源许可与版权声明

### 1. 主项目许可证

Kilim Minecraft Launcher 采用 MIT 许可证发布。

```text
MIT License

Copyright (c) 2026 Erics (Zhouxuanyao2333)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 2. 第三方库许可

本启动器使用了以下开源项目，感谢其作者：

| 库名 | 许可证 | 用途 |
| --- | --- | --- |
| Avalonia | MIT | UI 框架 |
| Avalonia.Skia | MIT | 跨平台渲染 |
| SkiaSharp | MIT | 2D 图形渲染、3D 皮肤、液态玻璃着色器 |
| NAudio | MIT | 音效播放 |
| LiquidGlassAvaloniaUI | MIT | 液态玻璃 UI 效果，作者 KaranocaVe |

具体许可证文本以各第三方项目发布内容为准。

### 3. 商标声明

Minecraft 是 Mojang Studios / Microsoft 的注册商标。本启动器与 Mojang Studios、Microsoft 没有任何隶属、赞助或认可关系。

GitHub 是 GitHub, Inc. 的注册商标。

本启动器不声称拥有任何第三方的商标、游戏素材、游戏文件或知识产权。

### 4. 版权归属

- 启动器源代码：版权归 Erics (Zhouxuanyao2333) 所有，采用 MIT 许可证。
- Minecraft 游戏文件及相关知识产权：版权归 Mojang Studios / Microsoft 所有，本启动器不分发任何游戏本体文件。
- 液态玻璃效果库：版权归 KaranocaVe 所有，采用 MIT 许可证。
- 其他第三方库：版权归各自作者所有，详见其许可证。

---

<a id="english-version"></a>
# English Version

<a id="doc-en"></a>
## Document Notice

**Effective Date: October 31, 2026**

**Last Updated: October 31, 2026**

Kilim Minecraft Launcher (the "Launcher" or the "Software") is an **open-source, non-commercial Minecraft launcher tool**. The Launcher is not the official Minecraft launcher and has no affiliation, sponsorship, endorsement, or other official relationship with Mojang Studios, Microsoft, or their affiliates.

This document describes the Launcher's Privacy Policy, Third-Party Data Collection Policy, Terms of Service, Open Source License, and Copyright Notice. This document should be read together with the actual behavior of the Launcher's source code and released builds. If this document conflicts with mandatory local law, the mandatory local law prevails.

The Launcher defines its project boundaries through the following statements:

1. **The Launcher does not contain backdoors, hidden telemetry, silent data uploads, remote control, or account-stealing logic.**
2. **The Launcher has no developer-operated server, no official website, and no account system. The developer does not receive, store, or upload users' account tokens, passwords, or personal data.**
3. **Authentication data collected during Microsoft login is never uploaded by the Launcher to the developer or any third-party server.**
4. **The download feature is only for obtaining files required to run Minecraft. It does not provide cracking, authentication bypass, piracy distribution, cheating, or account theft.**
5. **The Launcher is an open-source tool released under the MIT License and is available for public audit.**
6. **Users are responsible for ensuring that their use complies with local law, the Minecraft End User License Agreement (EULA), and the Microsoft Services Agreement.**

This document is not legal advice. The project publisher should review it against the actual code, release regions, and applicable law, and consult a qualified legal professional where necessary.

---

<a id="privacy-en"></a>
## Privacy Policy

**Effective Date: October 31, 2026**

### 1. Information We Collect

**The Launcher does not collect any personal information.**

The Launcher has no backend server, no telemetry, no crash reporting, no usage analytics, no advertising or analytics SDKs, and no network callbacks of any kind. The developer has no ability to receive, store, sell, or share users' personal information through the Launcher.

Account tokens, game paths, Java paths, instance information, settings, and logs are stored only on the user's own computer. By default, runtime data is stored in a `KilimLauncher` folder next to the executable.

### 2. Microsoft Authentication and Account Information

The Launcher supports Microsoft authentication using the official Microsoft OAuth 2.0 Device Code Flow.

- Authentication primarily occurs between Microsoft official servers, including `login.microsoftonline.com`, `user.auth.xboxlive.com`, `xsts.auth.xboxlive.com`, and `api.minecraftservices.com`.
- The Launcher acts only as an OAuth client, relaying authentication requests and tokens between the user's computer and Microsoft official servers.
- The Launcher does not ask users to enter their Microsoft account password inside the Launcher. The device code flow is normally completed by the user in a browser.
- Access tokens and refresh tokens are stored only in the local `accounts.json` file on the user's device.
- **Authentication data collected during Microsoft login is never uploaded by the Launcher.** The Launcher does not upload Microsoft account tokens, Minecraft access tokens, refresh tokens, passwords, or account profiles to the developer's server, developer-controlled third-party servers, or any unnecessary third-party service.
- The developer cannot see, access, or intentionally collect the user's Microsoft account password or token contents.

Users should protect their local `accounts.json` file because it may contain sensitive tokens that can be used to access the account. Users may delete the `KilimLauncher` folder to remove local account data.

### 3. Download Functionality and Copyright

The Launcher's download feature is only for obtaining files required to run Minecraft from official Minecraft resource servers and community mirror sources, such as version manifests, version JSON files, client JARs, libraries, and assets.

- **The download feature does not provide cracking or piracy support.**
- The Launcher does not provide cracking, authentication bypass, piracy distribution, cheating, or account theft.
- The Launcher does not distribute Minecraft game binaries.
- Downloading and running Minecraft requires the user to own a legitimate Minecraft account, or to use the Software only within the limits permitted by law and the EULA, such as testing or single-player use.
- Offline mode is intended for testing or single-player scenarios and does not mean that the developer encourages, supports, or endorses piracy.
- Minecraft, game files, Mojang trademarks, and related intellectual property are owned by Mojang Studios / Microsoft.

### 4. Log Files

The Launcher generates local logs such as `app.log`, `game.log`, `startup.log`, `crash.log`, and `MainWindowLog.txt` for troubleshooting.

- Logs are stored only on the user's local device.
- Logs are not automatically uploaded to the developer or any third-party server.
- By design, logs do not record Microsoft account passwords or Microsoft authentication tokens.
- Users should note that logs may contain local paths, system information, error stacks, and game output. Users should review and remove sensitive content before sharing logs.

### 5. Your Rights

Because the developer does not collect user data, users do not need to request deletion, export, or correction of data from the developer. All data is on the user's own computer. Users may at any time:

- Delete the `KilimLauncher` folder to remove local accounts, instances, logs, and configuration data.
- Use firewalls, network monitoring tools, or packet capture tools to verify the Launcher's network behavior.
- Use existing local instances for offline testing without Microsoft login or online features.
- Stop using the Launcher.

### 6. Policy Updates

The developer may update this Privacy Policy. Updated policies will be published in the project documentation. Continued use of the Launcher constitutes acceptance of the updated policy. If the user does not agree, the user should stop using the Launcher.

---

<a id="third-party-en"></a>
## Third-Party Data Collection Policy

**Effective Date: October 31, 2026**

The Launcher itself does not collect personal information and has no developer-operated server. However, during use, the user's device may communicate with the following third-party services. These services may log standard HTTP request information under their own privacy policies, such as IP address, request time, request path, User-Agent, and error codes. The developer does not control these third-party services and is not responsible for their privacy practices.

### 1. Microsoft, Xbox Live, and Minecraft Services

**Features:** Microsoft authentication, Xbox Live authentication, XSTS authentication, and Minecraft profile retrieval.

**Possible communication endpoints:**

- `login.microsoftonline.com`
- `user.auth.xboxlive.com`
- `xsts.auth.xboxlive.com`
- `api.minecraftservices.com`

**Data recipient:** Microsoft Corporation / Mojang Studios.

**Description:** When the user chooses Microsoft authentication, the user interacts with Microsoft servers in a browser to complete OAuth authorization. Microsoft processes user data under its privacy statement. The Launcher does not transmit the user's Microsoft account information to any party other than Microsoft official servers. **Authentication data collected during Microsoft login is never uploaded to the developer's server.**

### 2. Minecraft Official Resource Servers

**Features:** Version manifest, version JSON, client JAR, libraries, and assets.

**Possible communication endpoints:**

- `piston-meta.mojang.com`
- `piston-data.mojang.com`
- `resources.download.minecraft.net`
- `libraries.minecraft.net`
- Other official Mojang / Microsoft Minecraft resource domains

**Data recipient:** Microsoft Corporation / Mojang Studios.

**Description:** When downloading game files, the user's IP address and standard HTTP request information may be logged by Mojang servers. This is normal network request behavior. The Launcher does not attach additional tracking information to these requests.

### 3. Community Mirror BMCLAPI

**Features:** Optional acceleration for Minecraft file downloads when official sources are unavailable or slow.

**Possible communication endpoints:**

- `bmclapi2.bangbang93.com`
- Other node domains to which the mirror service may redirect

**Data recipient:** BMCLAPI maintainers and related mirror node operators.

**Description:** BMCLAPI is a community-maintained Minecraft download mirror. The user's IP address and standard HTTP request information may be logged by this service. The Launcher prioritizes official sources by default and falls back to mirrors only when official sources are unavailable, fail, or the download policy requires fallback. Users should read the relevant policies and notices of BMCLAPI and its node services.

### 4. GitHub

**Features:** Source code hosting, documentation hosting, issue reporting, and release page access.

**Possible communication endpoints:**

- `github.com`
- GitHub-related subdomains

**Data recipient:** GitHub, Inc. (Microsoft).

**Description:** If the user visits the project's GitHub repository, documentation, or release pages, GitHub will record the visit under its privacy policy. The Launcher itself does not automatically check for updates unless the user manually triggers such an action or a future version explicitly states otherwise.

### 5. User Network Environment and Proxies

If the user uses proxy software, VPNs, firewalls, network accelerators, or other network tools, network traffic may pass through those tools first. The privacy practices of those tools are chosen by and are the responsibility of the user. The developer does not control, operate, or assume responsibility for the user's proxy environment.

### 6. Third-Party Policy Changes

Third-party services may update their privacy policies, terms of service, or data processing practices. The developer encourages users to review relevant third-party policies periodically. The Launcher does not control third-party services and does not guarantee their data processing behavior.

---

<a id="terms-en"></a>
## Terms of Service

**Effective Date: October 31, 2026**

**Important Notice:** Please read this agreement carefully before using Kilim Minecraft Launcher (the "Launcher"). By using the Launcher, the user agrees to be bound by all terms of this agreement. If the user does not agree with any part of this agreement, the user should stop using the Launcher immediately.

### 1. Software Nature

1.1 The Launcher is an open-source, non-commercial Minecraft launcher tool released under the MIT License.

1.2 The Launcher is not the official Minecraft launcher and has no affiliation, sponsorship, endorsement, or other official relationship with Mojang Studios, Microsoft, or their affiliates.

1.3 The Launcher does not distribute, crack, or bypass Minecraft's authentication system. Downloading and running Minecraft requires the user to own a legitimate Minecraft account, or to use the Software only within the limits permitted by law and the EULA.

1.4 The Launcher does not contain backdoors, hidden telemetry, silent data uploads, remote control, or account-stealing logic. The source code is released under the MIT License for public audit.

### 2. License and Restrictions

2.1 The user may:

- Freely use, copy, modify, merge, publish, and distribute the Launcher's source code;
- Use the Launcher for personal or commercial purposes, provided that the game itself is properly licensed;
- Create derivative works in compliance with the MIT License and applicable law.

2.2 The user may not:

- Use the Launcher for any activity that violates local law;
- Use the Launcher to download, distribute, or disseminate pirated Minecraft game files;
- Modify the Launcher to bypass Microsoft or Mojang authentication mechanisms;
- Disguise the Launcher as the official launcher for phishing, fraud, or misleading purposes;
- Add backdoors, malicious code, account theft, cheating, or unauthorized data collection to the Launcher;
- Remove or falsify copyright notices, license notices, or trademark notices in the Launcher.

### 3. Intellectual Property

3.1 The Launcher's source code is copyrighted by the developer and released under the MIT License.

3.2 Minecraft, game files, Mojang trademarks, and related intellectual property are owned by Mojang Studios / Microsoft. The Launcher does not contain any Minecraft game binaries.

3.3 Third-party libraries used in the Launcher, such as Avalonia, Avalonia.Skia, SkiaSharp, NAudio, and LiquidGlassAvaloniaUI, are copyrighted by their respective authors under their respective open-source licenses.

### 4. Disclaimer of Warranties

4.1 The Launcher is provided "as is" without warranty of any kind, express or implied, including but not limited to warranties of merchantability, fitness for a particular purpose, non-infringement, or error-free operation.

4.2 To the maximum extent permitted by applicable law, the developer shall not be liable for any direct, indirect, incidental, special, or consequential damages arising from the use of or inability to use the Launcher, including but not limited to:

- Account bans, restrictions, or penalties;
- Data loss, corruption, or disclosure;
- System damage, software conflicts, or virus infection;
- Consequences of violating the Minecraft EULA or Microsoft Services Agreement;
- Consequences caused by third-party services, mirror sources, network environments, or user actions.

4.3 Use of the Launcher is entirely at the user's own risk. If the user is concerned about account security or compliance risks, the user should use the official Minecraft launcher.

### 5. User Responsibilities

5.1 The user confirms that the user owns a legitimate Minecraft account, or uses the Launcher only for offline testing, single-player use, or other purposes permitted by law and the EULA.

5.2 The user agrees to comply with the Minecraft End User License Agreement (EULA), the Microsoft Services Agreement, and applicable local law.

5.3 The user understands and agrees that using third-party launchers may involve risks related to the Minecraft EULA and may result in account restrictions. The developer does not encourage, support, or assume responsibility for any account issues arising from the use of the Launcher.

5.4 The user is responsible for protecting local account tokens, logs, configuration files, and other sensitive data.

### 6. Changes and Severability

6.1 The developer may update this agreement at any time. Updated agreements will be published in the project documentation. Continued use of the Launcher constitutes acceptance of the updated agreement.

6.2 If any provision of this agreement is held invalid or unenforceable by a competent authority, that provision shall be adjusted or removed to the minimum extent necessary, and the remaining provisions shall remain in effect.

6.3 If there is any inconsistency between the Chinese and English versions, the Chinese version shall prevail, except where mandatory local law requires otherwise.

---

<a id="license-en"></a>
## Open Source License and Copyright Notice

### 1. Main Project License

Kilim Minecraft Launcher is released under the MIT License.

```text
MIT License

Copyright (c) 2026 Erics (Zhouxuanyao2333)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 2. Third-Party Library Licenses

The Launcher uses the following open-source projects. We thank their authors:

| Library | License | Purpose |
| --- | --- | --- |
| Avalonia | MIT | UI framework |
| Avalonia.Skia | MIT | Cross-platform rendering |
| SkiaSharp | MIT | 2D graphics rendering, 3D skins, liquid glass shaders |
| NAudio | MIT | Audio playback |
| LiquidGlassAvaloniaUI | MIT | Liquid glass UI effects, author KaranocaVe |

The full license texts of third-party projects are governed by their respective releases.

### 3. Trademark Notice

Minecraft is a registered trademark of Mojang Studios / Microsoft. The Launcher has no affiliation, sponsorship, or endorsement from Mojang Studios or Microsoft.

GitHub is a registered trademark of GitHub, Inc.

The Launcher does not claim ownership of any third-party trademarks, game assets, game files, or intellectual property.

### 4. Copyright Attribution

- Launcher source code: Copyright Erics (Zhouxuanyao2333), released under the MIT License.
- Minecraft game files and related intellectual property: Copyright Mojang Studios / Microsoft. The Launcher does not distribute any game binaries.
- Liquid glass effects library: Copyright KaranocaVe, released under the MIT License.
- Other third-party libraries: Copyright their respective authors; see their licenses for details.
