代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2njnehzrb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ddjjbsvb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ocimjarv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2eghcfhsc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vwbbigje.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2iymnbfsz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zepqgcpt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lepvnifw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tordnlrs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wmalkyhk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vyqbxdlz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2obbnfoho.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xudshlnc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ypzceyjk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zognsucy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qzcvugjz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2frsbfogx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lquxfsxr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mljxdpmu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2yoyzsztk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2roevlgkf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kzcyvnvz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ouftthat.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2awvopsvg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kohdbzle.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nuxxzlys.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2echolezx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2eevqcrmb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ztflnlmy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cuwfhqvj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xzijkqmc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fewmqcfn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fdfxytba.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uxlbcdmx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2njpzrrdg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kdvzmcuc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2btskliul.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2znmpsvnt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vfoxhujo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ubmsoyrx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zihcfzyz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qfrglwkr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2etwivrux.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwfkxdfx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phetzlfe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kkqzeitk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dclcckrg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2onisyrrp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hybbegnw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jxcnzbwk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2asgtdkzk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rfzrcsqe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gbotzwwh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgnwxacx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tugttklt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2eormyaqo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bsmzfmyf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2oickrssc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pxibqfzb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kdjstvuo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fmmppcgf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zrvtfxeo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2sfiziygi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2eyfrghlu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bpzjnbkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bcgwuasg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2qbljofmm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lexmowqm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lgnxuedf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xghliolf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vvmldhws.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2njxssvqy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wtkwppio.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oonqkyhb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xozthiow.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vzgnmyvj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xsnroisq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ovndtbxs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2owjakxmr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dqujpitl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ivnlkzvw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ghtuhopr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nuncebqg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jsnwchar.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2onwuvvhw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yaltzwcd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tkojkwzn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjoeclfr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pdsptqqy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fopzzejg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lkpxgjyi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iosmqght.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ckdkvoxy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uqwjwpch.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2icoawumg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2egjdbhqg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2owpnmril.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sjaamqhk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xblinsaz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vpvotzmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emzkhrfs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2oodtrxss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylnpugri.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2riiyehih.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bjdsqces.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vfcsibli.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kudeobjd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2weyoyzwi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yztaueri.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cfmkowyu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ovhrfggx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hscwtkto.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2pckrwitn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tcxkcbzw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ritrqsmp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jdfbdldm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zqtnqxnu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ricyknow.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2etqjygdq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xzguepll.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cukfrxcg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2abyoglxa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ipirelkw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xosxeewp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hyswqlip.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ctwhpfvr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mayicldu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oavrgzmd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ogljyajt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vmsepohp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wtdxoovi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xydbudya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wodktahf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2syxxuopz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oyehlysp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xgvyvtvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bajixoco.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lxynizou.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uszhsjlf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xmwelcpn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yyztypeb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rtvdieib.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2odoiymoo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ppxsoiui.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rxzujabd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ygaavdbc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mybvkdwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wxjftfcs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eumelchx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xqernraj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hnhxjlrx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mtaytfzg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2guyfqrwu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jqxvyspx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tiixdnos.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2aqokqhrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcvofbwb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2barjnqjv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2kzxpuxaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgujvmwy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ozokulmx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2deizyloh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2lyjowplo.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2bklgzfwa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ggwxcjmr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tzgfzqoh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2anoymcix.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gkfzfrqu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2izqammyq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2oabknpsv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bbobbfut.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pbypbpxz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2gmiwgczq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2yrlnyoxu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mfrfcsza.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fkfqsewx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rliuwaqi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lddjhnbu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cygmcxtq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2eybkkkvg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wovgelpj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2betlxnzl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lbtrswsb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2edvnukpt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjepws.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bpjthczn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gcgkutvy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwonjlyh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sopxrqkc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qdanrvgq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odzyrrtg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jvgstgwd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pefrgreg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lghjimuv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yokazyty.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hutilohy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mvyarjwf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pcyigpcw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pplptbdu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2tdtyfnol.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jsqiduvz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cppidxtb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ldfpvjtp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ltcwmzgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkpgzjxw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2koeuurce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdmzyfam.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vcipwsav.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sdenfpnk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wevnrymn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2akrjvpog.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2igehazcf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yffdidxb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yieguqgi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2rjuypiey.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yivwxsxs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2mxbarqxd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nnipsqpj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wavrlgfy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mzvlwgym.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kxwtrkhv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kfzpqciy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ykdywegh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2qiotsltp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hdvdxaoz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2pwzrwoec.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wdfmofgc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zigicjoe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hbcmyfyo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzktjmwf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2msyaredt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aiddkhfw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pkhhcegm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2netwrmal.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bcgjvyuz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ldmknhzs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bhzluqlg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ovfcqwen.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2otriwsim.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jtkxsgpq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tktogzgl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ntbkygvr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vhrclvhu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wrphdzlp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bcoyrank.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ildwolnr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kgausngr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpomcp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vakolegx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pnsmmmsd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pszsnpqj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2slqdyhso.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rxjnycwe.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mdortzgu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ylatehyg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gxarobry.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wqyndykb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ugnrlspg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2dmitwiuo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ggiyhbid.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bsveizhj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fdlyecsj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xqykpgpf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ztinqgly.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wgonyype.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vskeelrf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vdfmfavj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjrmggy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2iycwgoaq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2idyjrwmq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vahhshmc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2akzsqyue.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbcckevx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvfupxk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mznxntme.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dldhlkkm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ambncehh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2drakdhog.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ubikfaim.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vdpiwrtd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekapxulz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vlobomqo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rcfknavi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnrnolv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmraiey.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2zgxhdrta.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rwvzcdvw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpjcoin.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tkyhuyew.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xvifoupc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2azdernyz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hwroempr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zcmlbnlc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2avlkfygs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wmwvlcmx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ugegwbcy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qvidkdvl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2bjklibth.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gruqhwjg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kyihrrsr.html


<!-- 参考信息 -->