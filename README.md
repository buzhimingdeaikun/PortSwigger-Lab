# PortSwigger 实验室漏洞复现笔记

> 基于 PortSwigger Web Security Academy 完成的实战实验记录。
> 包含 Web 安全核心漏洞（SQL注入、访问控制）的完整复现过程、Payload 构造、原理分析与修复方案。

---

## 📂 已完成实验目录

### 🛡️ SQL Injection（SQL注入漏洞）

✅ **[Lab1-WHERE子句注入](./SQL%20Injection/Lab1-WHERE子句注入)**  
✅ **[Lab2-登录绕过](./SQL%20Injection/Lab2-登录绕过)**  
✅ **[Lab3-UNION攻击确定列数](./SQL%20Injection/Lab3-UNION攻击确定列数)**  
✅ **[Lab4-UNION攻击查找包含文本的列](./SQL%20Injection/Lab4-UNION攻击查找包含文本的列)**  
✅ **[Lab5-UNION攻击从其他表获取数据](./SQL%20Injection/Lab5-UNION攻击从其他表获取数据)**  
✅ **[Lab6-UNION攻击在单列中检索多个值](./SQL%20Injection/Lab6-UNION攻击在单列中检索多个值)**  
✅ **[Lab7-查询Oracle数据库类型和版本](./SQL%20Injection/Lab7-查询Oracle数据库类型和版本)**  
✅ **[Lab8-查询MySQL和Microsoft数据库类型和版本](./SQL%20Injection/Lab8-查询MySQL和Microsoft数据库类型和版本)**  
✅ **[Lab9-基于条件响应的盲注](./SQL%20Injection/Lab9-基于条件响应的盲注)**  
✅ **[Lab10-带时间延迟的盲注](./SQL%20Injection/Lab10-带时间延迟的盲注)**  

---

### 🔓 Access Control（访问控制/越权漏洞） 

涵盖信息泄露、未授权访问、基于 Cookie 及 URL 参数的权限绕过、IDOR 越权等典型业务逻辑漏洞。

✅ **[Lab1-未受保护的管理员功能](./Access%20Control/Lab1-未受保护的管理员功能)**  
✅ **[Lab2-无保护的管理员功能，URL不可预测](./Access%20Control/Lab2-无保护的管理员功能，URL不可预测)**  
✅ **[Lab3-用户角色由请求参数控制](./Access%20Control/Lab3-用户角色由请求参数控制)**  
✅ **[Lab4-用户ID由请求参数控制 - IDOR越权](./Access%20Control/Lab4-用户ID由请求参数控制%20-%20IDOR越权)**  
✅ **[Lab5-用户ID由请求参数控制，用户ID不可预测](./Access%20Control/Lab5-用户ID由请求参数控制，用户ID不可预测)**  

---

### 🎭 XSS（跨站脚本攻击） 

涵盖反射型 XSS、存储型 XSS、XSS 与 CSRF 组合利用及 WAF 绕过防御等典型跨站脚本攻击手法。

✅ **[Lab1-将 XSS 映射到 HTML 上下文中，且没有编码](./XSS/Lab1-将%20XSS%20映射到%20HTML%20上下文中，且没有编码)**  
✅ **[Lab2-将 XSS 存储为锚属性，并用 HTML 编码双引号 href](./XSS/Lab2-将%20XSS%20存储为锚属性，并用%20HTML%20编码双引号%20href)**  
✅ **[Lab3-利用 XSS 绕过 CSRF 防御](./XSS/Lab3-利用%20XSS%20绕过%20CSRF%20防御)**  
✅ **[Lab4-将 XSS 映射到 HTML 上下文中，大部分标签和属性被屏蔽](./XSS/Lab4-将%20XSS%20映射到%20HTML%20上下文中，大部分标签和属性被屏蔽)**  

### 🔜 持续更新中...
下一步计划：**XSS（跨站脚本攻击）**、**文件上传漏洞**、**逻辑漏洞**等实战实验。

## 🛠️ 使用工具
- **Burp Suite**（抓包、重放、Intruder 自动化爆破）
- **Google Chrome / Firefox**（调试与 Payload 发送，F12 开发者工具）
- **PortSwigger Web Security Academy**（漏洞靶场平台）
- **Markdown + GitHub Pages**（实验笔记归档）

## 📌 实验说明
每个实验目录下均包含：
1. **完整的攻击过程截图**（请求、Payload、结果回显、Lab 完成标志）。
2. **企业级漏洞报告**（包含漏洞描述、复现步骤、原理分析、影响评估及修复建议）。
