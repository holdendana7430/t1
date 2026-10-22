代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvirju.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2opxrojrj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2txzrdbqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2brehcxuh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xxryloss.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mjlvoqkd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zedyzxpl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfkbsya.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wlcujxsc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkzccecd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqnmtt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bzipggbe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jvwtalfj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gqpdvtzm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nyxccsfl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lvhbacxp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kqcfeihg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uwcngdam.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zdlpkpjf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hepsqdhy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rkfqzhlo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jadpxhwy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2oosdndtu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqihhiso.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gokvmfcl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2udfmtfsn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2smphdeoe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtxpkip.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvrjrbzh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kppbemnq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bchnndso.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hhvuasjs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ewercgep.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jakubtcz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jjvuoopq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ednekngr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2umcncqzm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vfleinxk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ceibwdka.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zicsdikr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2viegkqxo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ujlhcbij.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nkaktszy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yltnfdip.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wtzarvkn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2riynlpmt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2txzjusgf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bvskslpb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2emgsgeff.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lkkxfnjz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2otndzczj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2evmkbaal.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ujcykdyl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qrcstpry.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bzyfmane.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kzhbcboq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tlvlzare.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ouunqbex.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2schjzvkc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rgoaocjs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2oacyekif.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jikdwppm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2cbrzyoid.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lytnaooe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obdvosdp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2unnspnrs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vbovqqyl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2psjmlckn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aejqjfuq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dybrobxd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2clnteuwo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxowzfb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rrpsghjr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mnlkqjzi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hssrvoao.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrllqjpg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tpgrfesq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2oyeuaoyw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2alslvdvo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wxucmdme.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2nyuezygu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vdhiiyah.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2acbcvboa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wvqwbhhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkypxatn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2baigbijp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwjwgyat.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xeuuyzhz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vwmaiuhw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ixrebxkr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jivxcjnm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rbvqtqvj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hcgndcqg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aedjktkj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2suourkqn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zuvdmnrc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mcgtxbyn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dckkwhgx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2apfiuxwc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2obopbixd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zsenveap.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lhwogxvn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2liqbbcgr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2qpepamra.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vcbhkutn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gnoqsmcp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lsgvgxtw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pwaehzfi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gedlxsmz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qoeavatz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xidwfmau.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hokruiej.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fspodsov.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rpgacazb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hjfjmury.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2suyykael.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xyvopxwx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qkrbwpwi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hhzrfjhu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nodufyvs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdrwokha.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lwqdnsqu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mqzmaipn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tmqbiyvz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qqsxdghk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ufbvnqgv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ilymzfyq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhrqde.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2qxyuaczd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2klggufrt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ntpihfhl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zpdfybib.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2edbzvuei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yenclbwt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jjuzxclm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2sdwyyfru.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2upkujmde.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2duhvhppl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gobcvkhw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hgvsqolk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qytwkhos.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pqcslnex.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ogzvokss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nviiwmvb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kiygmmod.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2exlssajp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kxhpdhcl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hbxatoxh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2owzhggqe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tssesxwu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gwdkwijc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dyhmfmfh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2psgtpszn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qfaydxbz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zdxgnuzl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2uxsyqjfr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bnbecedx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uyaswlgh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2uvdsgvjk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nhnvwwtr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2prqfogpc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ipjginux.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dlecirnu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2udtsginj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ymgnqokg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wjujnvco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qilrgtbo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2sneujirr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcqwndsr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eguyhzxv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wytdslfy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wegkzguq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ewgddysx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2velzspio.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vnrgtiau.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gkltqgax.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uqtfjruq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lllymntt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2glewjozv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fmrtkldu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ailsyhuk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2oxqncsbu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fydunesg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bouiilvp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hvgmqzdz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhqhxsbi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mxtkhndn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyjuilzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btgafmsj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfjfhgfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovvunggz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xkwsruox.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2raynstiv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2mltbblzp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tlxeoknd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xzoivyaz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yffhumgl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2chbwwwjo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjyywa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fhynyqla.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nujbwaye.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ysegasvw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yivanfkr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ummbanbl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2umjhnbif.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jbxoextd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ajrnelsv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iqkkptfk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2httilklt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zrttslmb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ifukwxlr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxaysigz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lnzwmxab.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dvdbelzn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jopamoxy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xciymfrc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kjjnvsdh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ydourlbi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mnixfzhm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cgrzqkng.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gpapzycf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mslwlfgb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kpaxizml.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bipqnxez.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rwnmmzfd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ctyalilt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vzyvapvm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tsaxlats.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2doxwnwks.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ndlngvxy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qsgdlous.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2midgmqxb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2etvxfkfw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cknncrtn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tohlglhi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dondxgpw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2slsoalvu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2djoyzwij.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2kymvbilc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nylcxbho.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2akotvirx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hmubsrvw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ugazgimb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cnyizqov.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rovueykh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lavqbrlh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pqkbffxf.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cimksmeh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zbuadqgf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ycbpctuh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2porlxasq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2aycttvvd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ftsfbewr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wutndkjr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ewnnhqih.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dducyqte.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nmyudpja.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bpnlvwgk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tntxpabb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xtvcvgim.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgstrx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hjhvvrix.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lzmrgrol.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2eqoeswxm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcqffrbi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdprtexc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzqorpmb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kcujpzeg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2votsewpo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ymfucbpj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2eefwzleq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mbsqbdeu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nxerubbg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2utxmbtgf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ccqxuwfz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2idngnvsf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2owpgznhm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tcwzfnkk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2aoogtfuu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pljejbqh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2oqeprfwj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xgosnqjb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pgarvuem.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2afnhjvmu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2woyeoicd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mduidjqn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iihvgkss.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2njnjfvnp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2znqwzubl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cwlqlwyq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2bgdijhoo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2bfpoqdrn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bivfyarw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vmcokapg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ohyyfaes.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2njkybblu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hfwqqtgk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ibzgpewp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fnuwivkx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2scldqcnv.html


<!-- 参考信息 -->