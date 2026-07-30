# PenForge - 网络安全风险评估系统

## 项目简介

PenForge（服安科技）是一个集成的网络安全风险评估平台，整合了102个主流渗透测试工具，覆盖了从信息收集到后渗透的完整攻击链。该平台旨在为安全研究人员、渗透测试工程师和合规审计人员提供一个统一、高效的工作环境。

**核心特性**：
- 🌐 **双界面模式**: 同时提供Web界面和CLI命令行工具箱
- 🔧 **102个工具集成**: 覆盖10大类渗透测试阶段
- 📊 **参数智能配置**: 详细的参数说明和一键命令生成
- ⚡ **实时输出显示**: 即时查看工具执行结果
- 🔒 **合法合规**: 仅用于授权安全测试
<img width="3456" height="2168" alt="17" src="https://github.com/user-attachments/assets/7c4a1a21-03bd-4347-bb30-5bec5a8705e9" />
<img width="3456" height="2168" alt="18" src="https://github.com/user-attachments/assets/f4231c0f-9794-480d-a3eb-a41f41da3ad3" />
<img width="3456" height="2168" alt="3" src="https://github.com/user-attachments/assets/409287ad-4a00-4191-b289-05760bf989fd" />
<img width="3456" height="2168" alt="2" src="https://github.com/user-attachments/assets/7f132bac-892c-4e3a-b46c-3423daef5427" />
<img width="3456" height="2168" alt="1" src="https://github.com/user-attachments/assets/9598d747-3b75-4bad-ac88-c89c939a8436" />
<img width="3456" height="2168" alt="11" src="https://github.com/user-attachments/assets/6c2e4257-b66b-408e-9a87-1926fc9bd692" />
<img width="3456" height="2168" alt="9" src="https://github.com/user-attachments/assets/22eb4a3b-04f4-4a92-8cd2-6717367b40a8" />
<img width="3456" height="2168" alt="8" src="https://github.com/user-attachments/assets/b3c1f546-2870-428b-846e-b7b84fab05cf" />
<img width="3456" height="2168" alt="7" src="https://github.com/user-attachments/assets/2da68c1f-f0bd-45fd-b114-a363c5e63b65" />
<img width="3456" height="2168" alt="6" src="https://github.com/user-attachments/assets/501587d2-5c27-43c7-b8b8-c4698ef84a99" />
<img width="3456" height="2168" alt="5" src="https://github.com/user-attachments/assets/5431c28b-08dd-449c-afa9-b872502fbcbf" />
<img width="3456" height="2168" alt="4" src="https://github.com/user-attachments/assets/aa09e7e5-f831-4d69-94e8-ea2804255b17" />

## 系统架构

### 技术栈
- **后端**: Python Flask
- **前端**: 原生HTML/CSS/JavaScript
- **CLI界面**: Python curses（交互式终端界面）
- **数据库**: 无需数据库（轻量级设计）
- **运行环境**: Kali Linux

### 核心功能
- **Web界面**: 提供统一的Web界面操作所有工具
- **CLI工具箱**: 交互式命令行界面，支持键盘导航
- **参数配置**: 每个工具都有详细的参数说明和配置选项
- **实时输出**: 执行结果实时显示在界面
- **结果复制**: 支持一键复制执行结果到剪贴板
- **命令生成**: 自动构建完整的工具命令行

## 双界面模式

PenForge提供两种使用方式，满足不同场景需求：

### Web界面（推荐新手使用）

**优势**：
- ✅ 图形化界面，直观易用
- ✅ 鼠标操作，无需记忆快捷键
- ✅ 适合团队协作和演示
- ✅ 可远程访问，支持多人使用

**访问方式**：
```bash
bash /sectools/start.sh
# 访问 http://localhost:34567
```

**功能特性**：
- 📱 响应式设计，支持各种屏幕尺寸
- 🎨 清晰的分类导航，10大类工具一目了然
- 📊 工具分布统计图表，可视化展示工具数量
- 🔍 实时搜索功能，快速定位工具
- 📋 一键复制功能，方便分享结果

### CLI命令行工具箱（推荐高级用户）

**优势**：
- ✅ 快速启动，无需浏览器
- ✅ 键盘操作，效率更高
- ✅ 适合自动化脚本集成
- ✅ 支持SSH远程操作

**启动方式**：
```bash
python3 /sectools/main.py
```

**界面预览**：

#### 1. 主界面 - 工具分类选择
<img width="3456" height="2168" alt="12" src="https://github.com/user-attachments/assets/d699ad45-86cc-404e-9599-b0d995b93d96" />

**功能说明**：
- 📊 显示10大类工具分类
- 🔢 实时显示每个类别的工具数量
- ⌨️ 使用↑↓键选择分类，Enter键进入
- 📝 顶部显示系统信息和使用提示

#### 2. 工具列表 - 工具选择界面
<img width="3456" height="2168" alt="13" src="https://github.com/user-attachments/assets/3df9df8b-e0d8-4a36-9b89-10b13c89b49f" />

**功能说明**：
- 📋 列出当前分类下的所有工具
- 📝 实时显示工具描述和示例命令
- 🔍 底部显示工具简介和使用示例
- ⌨️ 使用↑↓键选择工具，Enter键配置参数

#### 3. 参数配置 - 参数选择界面
<img width="3456" height="2168" alt="14" src="https://github.com/user-attachments/assets/36118777-8526-478c-bd9f-842cecb67db3" />

**功能说明**：
- 📂 参数按功能分组展示（如：主机发现、扫描技术、输出选项）
- ☑️ 支持复选框选择（开关参数）
- 📝 支持输入框输入（值参数）
- 🔧 实时构建完整的命令行
- ⌨️ 使用↑↓键选择参数，Space键切换，Enter键输入值

#### 4. 执行结果 - 输出显示界面
<img width="3456" height="2168" alt="15" src="https://github.com/user-attachments/assets/64fc2f05-3da9-4c2e-9d9d-189f10967463" />

**功能说明**：
- 📊 实时显示工具执行输出
- 🎨 彩色输出，区分不同类型信息
- 📋 支持一键复制输出结果
- ⚡ 支持中断和重试操作

**CLI键盘快捷键**：

| 按键 | 功能 | 说明 |
|------|------|------|
| `↑` | 向上移动 | 选择上一项 |
| `↓` | 向下移动 | 选择下一项 |
| `←` | 返回上级 | 返回分类选择 |
| `→` | 进入下级 | 进入工具详情 |
| `Enter` | 确认选择 | 选择当前项或执行命令 |
| `Space` | 切换参数 | 开关参数选择 |
| `Tab` | 切换焦点 | 在参数间切换 |
| `ESC` | 返回上级 | 返回上一级菜单 |
| `q` | 退出程序 | 退出CLI工具箱 |
| `r` | 重新执行 | 重新运行上一个命令 |
| `c` | 复制命令 | 复制当前命令到剪贴板 |
| `h` | 帮助信息 | 显示帮助文档 |

**CLI适用场景**：
- 🔧 **快速操作**: 无需打开浏览器，直接在终端执行
- 🤖 **自动化集成**: 可集成到CI/CD流水线
- 🌐 **远程操作**: 通过SSH远程使用，无需图形界面
- 📊 **资源占用低**: 轻量级设计，适合资源受限环境
- 🔒 **安全审计**: 审计人员可在无图形界面环境下工作

## 工具分类

系统将102个渗透测试工具按照攻击链分为10大类：

### 1. 信息收集（32个工具）
从目标网络、系统、应用中收集信息，为后续渗透测试奠定基础。

**核心工具**：
- **Nmap**: 端口扫描、服务识别、操作系统探测
- **BloodHound**: Active Directory环境分析
- **Amass**: OWASP子域名枚举工具
- **theHarvester**: 邮箱、子域名、员工信息收集
- **DNSenum/DNSrecon**: DNS枚举和区域传输
- **WhatWeb**: Web应用指纹识别

**其他工具**: SSLScan, GoBuster, DirB, FFUF, WFuzz, DMitry, Unicornscan, SpiderFoot, Masscan, Nmap等。

### 2. 漏洞扫描（7个工具）
自动化检测Web应用、主机系统、网络服务的安全漏洞。

**核心工具**：
- **Nuclei**: 基于模板的快速漏洞扫描器，支持CVE检测
- **Nikto**: Web服务器漏洞扫描
- **SSLyze**: SSL/TLS配置分析
- **WPScan**: WordPress漏洞扫描
- **Commix**: 命令注入自动检测

**其他工具**: Skipfish, Wapiti。

### 3. 漏洞利用（6个工具）
利用已知漏洞进行攻击验证和渗透测试。

**核心工具**：
- **SQLMap**: 自动化SQL注入检测和利用
- **Metasploit**: 世界领先的渗透测试框架
- **SET (Social Engineering Toolkit)**: 社会工程学攻击工具包
- **Gophish**: 钓鱼攻击模拟平台

**其他工具**: atk6-thcping6, DNS-rebind。

### 4. 密码破解（19个工具）
在线爆破、离线破解、哈希识别等身份认证安全测试。

**核心工具**：
- **Hydra**: 快速网络登录爆破工具，支持50+协议
- **Hashcat**: 世界最快的密码恢复工具，支持GPU加速
- **John the Ripper**: 经典密码破解工具
- **Crunch**: 自定义字典生成器

**其他工具**: Medusa, Ncrack, Patator, Cewl, HashID, Ophcrack, Bully, Pixiewps, Reaver, Wifite等。

### 5. 权限提升（5个工具）
在已获得低权限的情况下，提升至更高权限或系统管理员权限。

**核心工具**：
- **PEASS (Privilege Escalation Awesome Scripts)**: Linux/Windows提权辅助脚本
- **Unix-privesc-check**: Unix系统权限提升检查
- **MITMProxy**: 中间人攻击代理工具

**其他工具**: DNSChef, SSLSplit。

### 6. 横向渗透（7个工具）
在内网环境中进行横向移动，扩大攻击范围。

**核心工具**：
- **Evil-WinRM**: Windows远程管理渗透工具，支持Pass-the-Hash
- **Impacket**: Python网络协议工具集（psexec, wmiexec, smbexec等）
- **NetExec (原CrackMapExec)**: 后渗透瑞士军刀
- **Mimikatz**: Windows凭据提取工具

**其他工具**: SMBMap, XFreeRDP, Arping。

### 7. 后渗透（18个工具）
维持访问权限、数据渗出、隐蔽通道建立。

**核心工具**：
- **PowerSploit**: PowerShell后渗透框架
- **Weevely**: PHP Web Shell
- **Netcat**: 网络瑞士军刀，端口转发和反向Shell
- **Socat**: 高级网络中继工具

**其他工具**: Laudanum, Exe2hex, DNS2TCPC, ProxyTunnel, PTunnel, Pwnat, SSLH, Stunnel4, UDPTunnel等。

### 8. 应急响应（2个工具）
安全事件分析、流量捕获、入侵检测。

**核心工具**：
- **TCPDump**: 网络流量抓包和分析工具

**其他工具**: Dcpdump。

### 9. 网络攻击（0个工具）
预留类别，暂无工具。

### 10. 辅助工具（7个工具）
网络诊断、协议分析、编码解码等日常实用工具。

**核心工具**：
- **Hping3**: TCP/IP数据包生成和分析
- **Fping**: 批量主机存活检测
- **Rdesktop**: Windows远程桌面客户端

**其他工具**: Netmask, Ssldump, Socat, Wedecode。

## 使用指南

### 系统要求

**硬件要求**：
- CPU: 双核及以上
- 内存: 2GB RAM（推荐4GB+）
- 硬盘: 10GB可用空间
- 网络: 稳定的网络连接（用于安装依赖）

**软件要求**：
- 操作系统: Kali Linux 2023.x 或更高版本
- Python: 3.8+（推荐3.10+）
- Shell: Bash 4.0+
- 权限: root/管理员权限（某些工具需要）

**必需软件包**：
```bash
# Python环境
python3 python3-pip

# 网络工具
nmap masscan netcat

# 系统工具
git curl wget
```

### 安装步骤

#### 1. 环境准备

```bash
# 更新系统
sudo apt update && sudo apt upgrade -y

# 安装Python依赖
sudo apt install -y python3 python3-pip python3-dev

# 安装网络工具
sudo apt install -y nmap masscan netcat-openbsd

# 安装系统依赖
sudo apt install -y git curl wget build-essential
```

#### 2. 克隆项目

```bash
# 克隆项目
git clone https://github.com/yourusername/sectools.git
cd sectools

# 或者直接下载ZIP
wget https://github.com/yourusername/sectools/archive/refs/heads/main.zip
unzip main.zip
cd sectools-main
```

#### 3. 安装Python依赖

```bash
# 创建虚拟环境（可选但推荐）
python3 -m venv venv
source venv/bin/activate

# 安装Flask依赖
pip install -r requirements.txt

# 如果没有requirements.txt，手动安装
pip install flask flask-cors
```

#### 4. 验证安装

```bash
# 检查Python版本
python3 --version

# 检查Flask安装
python3 -c "import flask; print(flask.__version__)"

# 检查工具可用性
nmap --version
hydra -h
```

### 启动系统

#### Web界面启动

```bash
# 方式1：使用启动脚本（推荐）
bash start.sh

# 方式2：直接启动Flask
cd webapp
python3 app.py

# 方式3：指定端口启动
PORT=5000 bash start.sh
```

**启动参数说明**：
- 默认端口: 34567
- 支持自定义端口: 修改start.sh中的PORT变量
- 自动清理端口占用
- 自动安装缺失依赖

#### CLI工具箱启动

```bash
# 直接启动CLI
python3 /sectools/main.py

# 或进入项目目录后启动
cd /sectools
python3 main.py
```

**CLI启动注意事项**：
- 必须在真实的终端中运行（不能通过SSH隧道）
- 需要足够的终端窗口大小（最小80x24）
- 支持彩色终端（推荐256色）

### 配置说明

#### Web服务器配置

**修改端口**：
编辑 `/sectools/start.sh`：
```bash
PORT=34567  # 修改为你想要的端口
```

**修改监听地址**：
编辑 `/sectools/webapp/app.py`：
```python
app.run(host='0.0.0.0', port=34567, debug=True)
# 修改为：
app.run(host='127.0.0.1', port=34567, debug=False)  # 仅本地访问
```

**生产环境部署**：
```bash
# 使用gunicorn部署
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:34567 app:app

# 使用nginx反向代理
sudo apt install nginx
# 配置nginx...
```

#### CLI工具箱配置

**修改快捷键**：
编辑 `/sectools/main.py`，找到按键处理部分，修改key映射。

**调整界面颜色**：
编辑 `/sectools/main.py`，修改curses颜色定义。

### 故障排查

#### 常见问题

**问题1：端口被占用**
```bash
# 错误信息
# Address already in use
# Port 34567 is in use by another program

# 解决方案
# 手动查找并杀掉进程
lsof -ti:34567 | xargs kill -9

# 或使用脚本自动清理
bash start.sh  # 会自动处理端口占用
```

**问题2：Flask未安装**
```bash
# 错误信息
# ModuleNotFoundError: No module named 'flask'

# 解决方案
pip install flask flask-cors
```

**问题3：工具未找到**
```bash
# 错误信息
# command not found: nmap

# 解决方案
sudo apt install nmap
```

**问题4：权限不足**
```bash
# 错误信息
# Permission denied

# 解决方案
# 使用sudo运行
sudo python3 main.py

# 或添加用户到sudoers
sudo usermod -aG sudo $USER
```

**问题5：CLI界面乱码**
```bash
# 原因：终端不支持UTF-8

# 解决方案
export LANG=en_US.UTF-8
export LC_ALL=en_US.UTF-8
```

**问题6：Web页面无法访问**
```bash
# 检查防火墙
sudo ufw status
sudo ufw allow 34567

# 检查服务是否启动
curl http://localhost:34567

# 检查进程
ps aux | grep python
```

#### 日志查看

```bash
# 查看Flask日志
# 直接在终端输出

# 查看系统日志
tail -f /var/log/syslog | grep python

# 查看Nginx日志（如果使用）
tail -f /var/log/nginx/error.log
```

### 性能优化

#### Web界面优化

```bash
# 使用多进程模式
gunicorn -w 4 -b 0.0.0.0:34567 app:app

# 启用gzip压缩
# 在nginx配置中添加：
gzip on;
gzip_types text/html text/css application/json application/javascript;
```

#### CLI工具箱优化

```bash
# 减少工具加载时间
# 编辑main.py，使用延迟导入

# 调整刷新频率
# 修改curses刷新间隔
```

### 安全建议

**网络安全**：
- 🔒 仅在受信任的网络中使用
- 🛡️ 使用防火墙限制访问
- 🔐 定期更新系统和工具
- 📝 记录所有测试操作日志

**数据安全**：
- 💾 定期备份配置文件
- 🗑️ 及时清理测试数据
- 🔑 使用强密码保护系统
- 📁 敏感数据加密存储

**合规建议**：
- 📋 获取书面授权文件
- 📝 记录测试范围和时间
- ⚖️ 遵守当地法律法规
- 🏢 建立审计追踪机制

### 访问系统
启动成功后，在浏览器中访问：
- 本地访问: http://localhost:34567
- 网络访问: http://your-ip:34567

### 基本使用流程

1. **信息收集**
   - 使用Nmap进行端口扫描
   - 使用Amass进行子域名枚举
   - 使用WhatWeb识别Web技术栈

2. **漏洞扫描**
   - 使用Nuclei扫描已知漏洞
   - 使用Nikto检测Web服务器问题
   - 使用SSLyze检查SSL配置

3. **漏洞利用**
   - 使用SQLMap测试SQL注入
   - 使用Metasploit执行漏洞利用

4. **权限提升**
   - 使用PEASS检查提权路径
   - 提升至管理员/root权限

5. **横向渗透**
   - 使用Impacket进行内网渗透
   - 使用Evil-WinRM横向移动

6. **后渗透**
   - 使用PowerSploit维持权限
   - 使用Netcat建立反向Shell

## 法律声明

**重要提示**: 本系统仅供授权安全测试、渗透测试与合规审计使用。使用者须遵守所在国家及地区法律法规，未经授权不得对任何目标系统进行探测或攻击。使用本平台即表示您已充分理解并同意承担相应的法律责任。

### 合法使用场景
- ✅ 已获得书面授权的渗透测试项目
- ✅ 企业内部安全评估和合规审计
- ✅ 安全研究和教学实验环境
- ✅ 漏洞挖掘和漏洞赏金项目（需符合平台规则）

### 非法使用警示
- ❌ 未经授权的系统和网络攻击
- ❌ 非法获取他人数据和隐私
- ❌ 破坏信息系统正常运行
- ❌ 其他违反法律法规的行为

## 技术支持

### 官方公众号
关注"服安科技"公众号，获取最新工具使用教程、安全资讯和系统更新。

### 项目地址
- GitHub: https://github.com/yourusername/sectools
- 官网: https://www.fuan-tech.com

### 社区支持
- 📧 Email: support@fuan-tech.com
- 💬 微信公众号: 服安科技
- 📝 问题反馈: GitHub Issues

## 项目结构

```
sectools/
├── README.md                 # 项目说明文档
├── start.sh                  # Web服务启动脚本
├── main.py                   # CLI工具箱主程序
├── requirements.txt          # Python依赖列表
│
├── tools/                    # 工具模块目录
│   ├── nmap.py              # Nmap工具配置
│   ├── bloodhound.py        # BloodHound工具配置
│   ├── nuclei.py            # Nuclei工具配置
│   └── ...                  # 其他102个工具配置
│
├── webapp/                   # Web应用目录
│   ├── app.py               # Flask应用主程序
│   ├── index.html           # 首页
│   ├── nmap.py              # Nmap Web界面
│   ├── bloodhound.py        # BloodHound Web界面
│   └── static/              # 静态资源
│       ├── logo.jpg         # Logo图片
│       ├── qrcode.png       # 公众号二维码
│       └── 12-15.png        # CLI截图
│
└── docs/                     # 文档目录
    ├── user-guide.md        # 用户指南
    ├── api-reference.md     # API参考
    └── troubleshooting.md   # 故障排查指南
```

### 核心文件说明

**main.py** - CLI工具箱核心：
- 交互式终端界面（基于curses）
- 工具加载和管理
- 参数配置和命令构建
- 实时执行和输出显示

**webapp/app.py** - Web应用核心：
- Flask应用配置
- 路由注册和蓝图管理
- API端点定义
- 静态文件服务

**tools/*.py** - 工具配置文件：
- 参数定义（flag、name、desc、section）
- 工具元数据（name、category、description）
- 示例命令
- 参数分组展示

**webapp/*.py** - Web界面模块：
- HTML/CSS/JavaScript内容
- Flask蓝图注册
- API接口实现
- 参数配置接口

## 开发者指南

### 添加新工具

**步骤1：创建工具配置文件**
```bash
# 在tools/目录下创建新文件
touch tools/mytool.py
```

**步骤2：编写工具配置**
```python
# tools/mytool.py
from main import BaseTool

class MyTool(BaseTool):
    @property
    def name(self) -> str:
        return "mytool"

    @property
    def category(self) -> str:
        return "信息收集"

    @property
    def description(self) -> str:
        return "工具描述"

    @property
    def params(self) -> list[dict]:
        return [
            {
                "flag": "-h",
                "name": "帮助",
                "desc": "显示帮助信息",
                "section": "基本选项",
                "has_value": False
            },
            # 添加更多参数...
        ]

def get_tool() -> BaseTool:
    return MyTool()
```

**步骤3：注册工具到系统**
编辑 `main.py`，在load_tools()函数中添加导入：
```python
from tools.mytool import get_tool as get_mytool
```

并在返回的字典中添加：
```python
"mytool": get_mytool,
```

**步骤4：创建Web界面（可选）**
参考 `webapp/nmap.py`，创建对应的Web界面。

### API接口开发

**创建新的API端点**：
```python
# webapp/mytool.py
from flask import Blueprint, request, jsonify
import subprocess

mytool_bp = Blueprint('mytool', __name__)

@mytool_bp.route('/api/mytool', methods=['POST'])
def execute_mytool():
    """执行mytool工具"""
    try:
        data = request.json
        target = data.get('target')
        params = data.get('params', [])

        # 构建命令
        cmd = ['mytool']
        for param in params:
            cmd.append(param['flag'])
            if param.get('value'):
                cmd.append(param['value'])
        cmd.append(target)

        # 执行命令
        result = subprocess.run(cmd, capture_output=True, text=True)

        return jsonify({
            'success': True,
            'output': result.stdout,
            'error': result.stderr
        })
    except Exception as e:
        return jsonify({'success': False, 'error': str(e)}), 500

@mytool_bp.route('/api/mytool/params', methods=['GET'])
def get_params():
    """获取参数配置"""
    from tools.mytool import get_tool
    tool = get_tool()
    return jsonify(tool.params)
```

### 测试

**单元测试**：
```bash
# 运行测试
python -m pytest tests/

# 测试特定模块
python -m pytest tests/test_nmap.py -v
```

**集成测试**：
```bash
# 启动测试服务器
python -m pytest tests/integration/ --live
```

## 贡献指南

### 如何贡献

我们欢迎所有形式的贡献！包括但不限于：
- 🐛 Bug修复
- ✨ 新功能开发
- 📝 文档改进
- 🔧 代码优化
- 🌍 国际化翻译

### 贡献流程

1. **Fork项目**
   ```bash
   git clone https://github.com/yourusername/sectools.git
   cd sectools
   ```

2. **创建分支**
   ```bash
   git checkout -b feature/my-new-feature
   ```

3. **进行开发**
   - 遵循代码规范
   - 添加必要注释
   - 编写测试用例

4. **提交代码**
   ```bash
   git add .
   git commit -m "Add: 新功能描述"
   git push origin feature/my-new-feature
   ```

5. **创建Pull Request**
   - 详细描述改动内容
   - 关联相关Issue
   - 等待审核

### 代码规范

**Python代码规范**：
- 遵循PEP 8标准
- 使用4空格缩进
- 函数和变量使用snake_case命名
- 类使用PascalCase命名
- 添加类型注解（Type Hints）

**HTML/CSS/JavaScript规范**：
- 使用语义化HTML标签
- CSS使用BEM命名法
- JavaScript使用ES6+语法
- 代码保持简洁可读

### 提交信息规范

使用规范的提交信息格式：
```
<type>(<scope>): <subject>

<body>

<footer>
```

**类型（type）**：
- `feat`: 新功能
- `fix`: Bug修复
- `docs`: 文档更新
- `style`: 代码格式调整
- `refactor`: 代码重构
- `test`: 测试相关
- `chore`: 构建/工具变动

**示例**：
```
feat(tools): 添加新的端口扫描工具

- 添加masscan工具支持
- 新增Web界面
- 完善参数配置

Closes #123
```

## 开发团队

**服安科技** - 专注网络安全风险评估和渗透测试工具开发

## 版本历史

- **v1.0.0** (2026-07-29): 初始版本发布，集成102个渗透测试工具

## 许可证

本项目仅供合法安全测试使用，禁止用于任何非法用途。使用者需自行承担使用本软件的法律责任。

---

联系方式：公众号搜索服安科技
