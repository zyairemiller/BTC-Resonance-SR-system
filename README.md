<p align="center">
  <img src="https://img.shields.io/badge/version-2.0-blue?style=for-the-badge" alt="Version">
  <img src="https://img.shields.io/badge/platform-Windows-lightgrey?style=for-the-badge" alt="Platform">
</p>

<h1 align="center">OKX Resonance</h1>

<p align="center">
  <b>加密货币多维度技术分析桌面应用</b><br>
  Multi-Dimensional Crypto Technical Analysis Desktop App
</p>

---

## 这是什么？

**OKX Resonance** 是一款加密货币技术分析桌面工具，自动从 OKX 交易所拉取行情数据，通过多个维度帮你分析市场状态。

- **趋势方向** — EMA144/169 双均线判断多头/空头/缠绕
- **支撑与阻力** — 6 维评分找出历史关键价位（Super / Strong / Weak）
- **成交量分布** — POC、Value Area、HVN
- **清算热力图** — 模拟多杠杆档位的潜在清算位置
- **订单墙** — 实时买卖盘挂单压力
- **综合置信度** — 8 因子 0-100% 评分，支持三种策略模式

不依赖 OKX API Key，打开即用。中文 / English / 日本語。

---

## 使用教程

### 1. 下载

从 [Releases](https://github.com/yourusername/okxresonance/releases) 页面下载最新版 `OKXResonance.exe`（约 154MB）。

### 2. 启动

双击 `OKXResonance.exe` 运行，无需安装 Python 或任何运行环境。

首次运行 Windows 可能会弹出 SmartScreen 警告，点击「更多信息」→「仍要运行」即可。

启动后会自动打开浏览器进入仪表板页面（`http://127.0.0.1:18080`），同时弹出桌面窗口。

> 如果只想用浏览器访问（不弹桌面窗口），用命令行 `OKXResonance.exe --no-gui` 启动。

### 3. 首次确认

启动后会弹出免责声明弹窗，确认后进入主界面。

### 4. 界面概览

| 区域 | 内容 |
|------|------|
| **顶部栏** | 品种标签页（BTC/ETH/XAU/XAG/现货）、实时价格、Guide 按钮、语言切换 |
| **K线图** | 蜡烛图 + EMA144/169 叠加，上方切换 1H / 4H / 1D 周期 |
| **右侧面板** | EMA 趋势卡、S/R 共振卡、Volume Profile、订单墙、清算热力图 |
| **底部栏** | 连接状态、运行时间 |

### 5. 切换品种和周期

- 点击顶部标签切换品种，等待几秒加载数据
- 点击图表上方 **1H / 4H / 1D** 切换 K 线周期
- S/R 共振可独立选择时间周期：1H / 4H / 1D / ALL（跨周期合并）

### 6. 怎么看分析结果

#### EMA 趋势

| 状态 | 含义 |
|------|------|
| **GOLDEN_CROSS** | EMA144 在 EMA169 之上 → 偏多 |
| **DEATH_CROSS** | EMA144 在 EMA169 之下 → 偏空 |
| **ENTANGLED** | 两线交织 → 方向不明，建议观望 |

#### S/R 共振

| 评级 | 分数 | 含义 |
|------|------|------|
| **Super** | ≥5 | 高可信度关键位置 |
| **Strong** | ≥3 | 较强参考 |
| **Weak** | <3 | 弱参考 |

#### 置信度

| 等级 | 分数 | 含义 |
|------|------|------|
| 高 | ≥75 | 多个维度方向一致 |
| 中 | 50-74 | 部分一致，可参考 |
| 低 | 25-49 | 信号模糊，谨慎 |
| 极低 | <25 | 方向不明，建议观望 |

### 7. 策略模式

右侧面板可切换三种模式：

| 模式 | 适合 |
|------|------|
| **Aggressive（激进）** | 短线 / 高频 |
| **Balanced（平衡，默认）** | 日内 / 波段 |
| **Conservative（保守）** | 中长线持仓 |

### 8. 代理设置

如果你使用 v2rayN 或 Clash 等代理，程序会自动检测 SOCKS5 端口（10808 / 7890 / 1080）并走代理，无需手动配置。

### 9. 激活（可选）

不激活也能正常使用基础行情分析。激活后可解锁更高频率的数据刷新：

- **OKX API Key**（推荐，免费）：创建只读 API Key，粘贴到激活页面即可。验证后永久有效 + 30 天免考核
- **USDT TRC20 支付**（29.9 USDT）：支付后填写 TX Hash，激活 30 天

> **删除 API 授权信息**：如果绑定了错误的 API Key 或想清除授权，删除 `C:\Users\你的用户名\.okx_trading\activation.json` 这个文件即可，程序会回到未激活状态。

---

## ⚠️ 免责声明

本软件仅供教育和研究目的使用。

- 加密货币交易存在极高风险，可能导致全部资金损失
- 所有分析输出**不构成投资建议**
- 作者不对因使用本软件产生的任何交易损失承担责任

> "信号"、"置信度"、"支撑"、"阻力"等术语均指基于技术指标的计算输出，不代表任何交易建议。

---

## 📮 联系

- **Telegram**: [t.me/okxresonce](https://t.me/okxresonce)
- **OKX 推荐码**: `4870869`
