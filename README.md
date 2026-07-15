# PortSwigger-Lab

# PortSwigger 实验室漏洞复现笔记

> 基于 PortSwigger Web Security Academy 完成的实战实验记录。
> 包含完整的 SQL 注入漏洞复现过程、Payload 构造、原理分析与修复方案。

---

## 📂 已完成实验目录

### 🛡️ SQL Injection（SQL注入）

| 编号 | 实验名称 | 核心攻击手法 |
| :--- | :--- | :--- |
| ✅ **Lab1** | [WHERE子句中的SQL注入漏洞，允许检索隐藏数据](./Lab1-WHERE子句注入) | `' OR 1=1--` 绕过查询限制 |
| ✅ **Lab2** | [SQL注入漏洞，允许登录绕过](./Lab2-登录绕过) | `administrator'--` 绕过密码验证 |
| ✅ **Lab3** | [SQL注入UNION攻击，确定查询返回的列数](./Lab3-UNION攻击确定列数) | 递增 `NULL` 探测列数 |
| ✅ **Lab4** | [SQL注入UNION攻击，查找包含文本的列](./Lab4-UNION攻击查找包含文本的列) | 注入字符串定位文本回显列 |
| ✅ **Lab5** | [SQL注入UNION攻击，从其他表获取数据](./Lab5-UNION攻击从其他表获取数据) | 读取 `users` 表获取账号密码 |
| ✅ **Lab6** | [SQL注入UNION攻击，在单列中检索多个值](./Lab6-UNION攻击在单列中检索多个值) | 字符串拼接 `||` 合并数据 |
| ✅ **Lab7** | [SQL注入攻击，查询Oracle数据库类型和版本](./Lab7-查询Oracle数据库类型和版本) | 利用 `v$version` 指纹识别 |
| ✅ **Lab8** | [SQL注入攻击，查询MySQL和Microsoft数据库类型和版本](./Lab8-查询MySQL和Microsoft数据库类型和版本) | 利用 `@@version` 指纹识别 |

---

### 🔜 持续更新中...
下一步计划：**盲注（Blind SQL Injection）** 与 **XSS（跨站脚本攻击）**。

## 🛠️ 使用工具
- **Burp Suite** / 浏览器开发者工具
- **PortSwigger Web Security Academy**
- **Markdown + GitHub Pages** 笔记归档

## 📌 说明
每个文件夹内均包含：
1. **漏洞复现截图**（请求、Payload、结果、完成标志）。
2. **企业级漏洞报告**（含漏洞描述、复现步骤、影响及修复建议）。
