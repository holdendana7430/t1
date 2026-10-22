代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bdqjqopc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2iaigdqnx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bzliuyen.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ldawcbnj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2edfjcstp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gdnyhjhs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yzrazdiq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jiaouppa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dwxmmmqu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dyfjhzod.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ysobmthl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2evqcvfxd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rbquddmu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zxgrsnmw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cymzarzo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2suqbsade.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gmxgxiel.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ulvzgnrp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2juqffjrv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vbxaasav.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gpknbhgx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2szjnwihs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ctotdbty.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2moywpulu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yacluasy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jnwkzrcs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2efunubmk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oeooeqja.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dskwfgwa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kumgqnsx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lvthvdob.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbdokqbe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2izabgkth.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hloblebi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsccrtwo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xnkgzswa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2pdfyrikx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hzmuxyfp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2gwugfkmx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cpcyqyrk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2utadnrhl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2atomkjxq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cqrsesia.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tpcnlhzt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lellzpgd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rqdcmikj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pybxngxx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rupfyvlo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2aonskbtx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vpkobmuq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2kklprord.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxuquv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mdanxcvt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wsnnuzdx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cxhxnwus.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2liplvqwy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gpqnmhxo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pnxirwcx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vxncgqle.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gcpzskcc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uxgpkgel.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwhmvmy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fstflngg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2sdfardtx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tefaehor.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zlcmzoyj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2daqnhxgw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjhbyvsm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bfytzjhv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2umuexkml.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vxfhibrf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zdyrzuoj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ytzanpju.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qqgzgcry.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2szemqpsw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvqtrwh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2islmqett.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2prbxsbfi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xurpdhwq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqdjxolp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2katjmbzd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rigimlmx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dnddonlf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2moulqedh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zgunflep.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zhvjnrkv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gbigutty.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2afohqtep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiabzoex.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rjlqhtma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrjqqdmk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2poezloeu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xcfewgeq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2efeyekil.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2yvlurdcy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2vhhhegnz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2adtpbdcm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2csrzdryn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cxjjxhws.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rbdzfwjk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2crbhmspp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tylxzlyi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ixnulrdz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kbztwyfs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qpaaaeza.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pvdkemqd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2eafgmbmv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2emljmhkw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dolreuet.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ftyqglto.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cvxsnfrv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2fifzkkkq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2blqijpmo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gaappnqd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lvdmkevi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rgwgodow.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nrarxwzx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jqxdcowm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bufawjpt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2netstvxn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aonvlwvk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wqyqqoox.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hrcjbzve.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ccrxkgeu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pqmdktul.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jhynkclw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zaiotanq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ggcdqdrv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2aczgeisr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rfpwgedv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eoefttau.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkbvky.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2afdirnbt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ekchlmed.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wowpxtre.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dwfvqhwr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zcjgissm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tudvevpo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lwmknksn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gdwgvgjg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2mmpncurx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ezxxokgs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2mtvvzqad.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2mvvriojf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjodwvhx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tcdefmwb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jabvpmue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojyvgzku.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2joihyqmy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2favemgos.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2imapbdtp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wwpfaxpi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2iycrqknv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hlyuyvgw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tpwjkdnb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tbbsoygk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nuzsrxta.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2fdvwbuzh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cezoywdg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2nnepmvkr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2tawhuvoz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sdtuchod.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2czruolst.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2btpfexqi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jgxzkxsy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bwwevels.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2mjirwlfs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2crfzwsfu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pqyzpahf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2nvrfeejh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iwhwhyep.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2libybasy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2idjnhjla.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qpwvlsqc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lrwjfftc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iuymhfok.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxfsjqiu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcpzfsxv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hiybckwm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uarlardm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2symkkqvb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pvnfzdae.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ayvjbyoo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ngokvsmr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2peqjvmby.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnbgpqsu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mmxxmctg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfgfdgef.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ibvotywq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2prmxpfns.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ebfuxaoo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pluoygsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcuzbhrc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2skuyysvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyuwoame.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkpjjdpc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eajuiomf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2dsxqkrhq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qgfabbpk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2nhntkhux.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vatpeowy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rsiosyhw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2eojedeoo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ubzgusri.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2xwyjadsi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2nqwaabim.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dnqpharw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xmampgpv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2usmibqco.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tlzusfcn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpuywt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwruqk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lqgpattc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2kmpdfwxu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2twpsmjjy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jguxrigj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yewakfuq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bsyfshwy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqzwytd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fruqbloi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2txpjvssg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lnupjwbs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pudtzecz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rxfbfulc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ngjjqtsr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2annudwsd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pelhvlna.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2gasgzknj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2njrtdayz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rdjkmluy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2iejkllng.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lyzokvby.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ywujcris.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rgslodyx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zqzehvhs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ywbstczy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fbqqimzd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2emeebcac.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hmmwqfzz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmcwvvxl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wwcxujba.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2foqhoisa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hdcupyaq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jkswyscg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2unuzluen.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oxeqogen.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2srirniai.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2osqjcmtz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ajgljjpj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dikctoox.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ihfgyvah.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mgqmslur.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2oausfarx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ukbmyynv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kfamadnn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bgaxzgyz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cpoyfxhr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xbsgqwrr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lbxfkwca.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2udlvazoq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vraldtda.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mycmygyn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bplihdet.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kavceovv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2elagpwwg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2amluqbzd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ifijipsz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uybyoqie.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvyxznnl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqonmoez.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2empezula.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dtlusmeq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuntwkbk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tbmvprny.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2snzxvzjc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2boooqglj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gmcncgxh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsoefmh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2majxjqhm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2brzmdovh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ukqishoa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2auijhurs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uuubxxto.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2obfppzfc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tldeqilv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dlpcxyaj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gwtcmnlt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cydrbhpl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mwoalvvp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ribogqtu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jjytdyig.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2nymmzwxd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hjwnuflb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tpskfzjb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eclbfzkp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqmfhcvt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xikthmrm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2btlagmoo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2avsxtjzu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkvrhmh.html


<!-- 参考信息 -->