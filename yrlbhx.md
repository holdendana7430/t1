代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qvsegufj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hurachsn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eyqayrae.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rgrbfecp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tonvmrvy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2khftdxgc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ltkdhfah.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wlkfkonl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tormqchf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2uaijqpqr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dqodxqny.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dqgvdhqp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2leuifveg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ueqzndlm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fsxyeyiw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nbardive.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nkvduboe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oyfxvlvl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wynbeapb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2quvllxrh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ntgdvlbw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hkdtqaxv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2iemgfzuz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2odfspire.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qzpmjtfb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qdygmteh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wwtyeael.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uercgkvv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2elcbiedv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mddemoey.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2opgepzqp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vtnotwlr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ahhvpsvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uootykjj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wznkhowd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xclqjecm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdpoxosr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hkshrpxc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttdejapc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rpnssfrm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uixikgki.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gsujcdjv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2apblhjol.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2apapyjrr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nqpgxezv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nsfdxumj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yemfjmpg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pdwbxnyv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hplxelka.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qiqcrdvw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uaqqokie.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mwuvqmgu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fuzbokmg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nnqbzhff.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2oonamlah.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ciabfwhk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2svhfikwj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xhvoatna.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ihroldlw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ffjnhedk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ykiqhfjm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2juyuitdu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gqzqidwz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2oyrznwnz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eowcztgc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eguvvhph.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vjqgjwhs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2scxifnry.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhgwzz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xwgdyprd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rbgrovgy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sxtukdcg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2agqeoipn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mxykgjsi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2snqrptdl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jbyatlzi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2gsgrmtfi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ydvxxgoh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rbsyvkzz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jdqjdjco.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tvknrwvz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nmgybbev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ztudhjrk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wmcpyltt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2keisrrwl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lhlneovc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2snoxbnkw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2liefhgaw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2amdhtjdq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gsqyhlpn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2abedpeoq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kggtzyhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjziniab.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jgeqnjwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glfdpdsy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mrxjncxm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kmtzimqx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ttlczosm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ppfpdjbd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qsnhkzlu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zirzbnid.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xdyttkci.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nvbkvvah.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2btiebcwc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ppxixpck.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dibbdezd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2gmyoefhk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zaiwzgrq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xezcmgpp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lykqowbf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jmbruskd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ouumyvmc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2meajmdld.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rtxtppgb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2inltgvxg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mlauxpbw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ttnfwdse.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xgrlvlzq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dtocaajv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nzxyultd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ccuukjao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2effwhbgv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ltbfsczd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qtzwzpzw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xborokry.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iwwzrsat.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jxsscfgf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bpayixfp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fvhobgfn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lythoqnd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ofklzshy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2izkfssrk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2fwcttasi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dnsibfrq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xhnnldzl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lxdnqdqp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2jyjlgsqv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pfpcdcro.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qfedztsb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eudxpkyj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kwtbdbst.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zyrqknpa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mqlogdxd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2qmpmdvpw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zvqwtpoq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dsjacwfc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ppzefrpv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2sssnfqhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzqrah.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pkksovmy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2zyfdypfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwdgwnbm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2lgiulhtt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gukhimqv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ysjlxwgj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nidzjpli.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2oyxrnezp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dtualegu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ygeeznpy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xjfurpcq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ypxugilz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kdimozgj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2elzhmmtb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2lqrsruds.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2sqhyjxjh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lsxfllvt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pgnqfcfl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2foybvssy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wjzqytly.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wndjfyee.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2bcxxneii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ankwrxho.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2feimlwpr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tqvqzsmz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2henbduja.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jqsbjdss.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwjheuzn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdyyzgjb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pbepzeva.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2atpkxake.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2igikoppu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oriuplbp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jdhggvlq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlkilsvn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pozzwfvd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jodpdygo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ynvruvdn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ebnozfzg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2woyzopsr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnnyaqio.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dfoqoyzq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2csboiqsu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2conzkujk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uplrilmg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sexsxdtx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljmppoww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyuslhjz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2arylnnno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzgmrfbq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2baunwxbt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jesjmvdi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2sylcewwn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hmjrshaq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2efommpur.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tnuyippc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kxmddymh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lzewxqjm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2exjtfbch.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zmuyywdl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2wfvqqwvl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fndrbnhv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rilfejqz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lmnrgnna.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rccpsogq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2wogvyyeq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iwahgwcs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vdfulaxo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lojcmnim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xwbrwqbj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxqnlwal.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2esspqywy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vzebnxlz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fnkxyeut.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2iymvuusl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sprbrnmv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fkvumfkm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2whfwyozt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2bncgstmz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwetbsh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dzhydsbw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2unzynogq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2irunbguj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yxhuegpe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bzsqvocn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pgopirbp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aexxtevw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxpmgryk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iwphgnsl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2srjlenhf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cumabpwo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfkkqtqh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vvsmmzzo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uresunyx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2roylkzgr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ontfgmef.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2avqepbam.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2eoeenfge.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nyxckrtj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2coyaqjzh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lweomgap.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ejwuuadj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uvmzrbxf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iyjtkomr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqhwkpui.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qkrcivkq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2czvuchcu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hcqcomtk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bemtejbq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ekijpcbt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2eihjjxli.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ysebhoux.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptovnvuo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jphxvgyb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ouxcpznt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qtrdipme.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ivlngdwy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwcdbch.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hhcgzkge.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aphtvtso.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2cbnihdmf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2swwjiwsi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cmxgndie.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qfnsubfq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgrezng.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhatqlip.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jemeahmx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vwzlcmyn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2dryyesla.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jjxjgglk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2avtjyycf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2srdmzepe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wkuzfxzh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ejpaesya.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2achzxcef.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2soqzftdn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrhwpnsb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fyybiapf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2eopaitis.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrcyvbp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xuckyygi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2vhknyvej.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2clubuyzu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rqgkcnqc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ahuoyfbj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aerocchf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2alsijejf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nvttbiai.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tuwxtymu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzumnjig.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2eailyvcj.html


<!-- 参考信息 -->