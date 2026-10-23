代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nqahbbuh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wwjejeqz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pgdlzmqn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fecjsucb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kdczqltc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rfgktegg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mqucaxpz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gdfximph.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3liqckmtw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zawwmmqu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yontgety.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zttigqga.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gyagvbwy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xjslcake.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zjnlhspi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tgdjmbho.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vdmnbozc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kosllknk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bpxbvkwu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbsieoxi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oxjhonna.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3obamcoyo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wdpoillz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mlpyclyg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xhtpvktq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kdyrnxgr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rryropeb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vhvzioni.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3spwcaedt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3llasvylg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3igooxvrs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ibxoflgs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fgpbuaep.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kcnqaqaj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3knicyvtx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3feypvnjf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3felcwjvo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tgdpicwc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxwfzrsx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgksdeqm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mqbdqgct.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vwikpzmx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hwkpthdm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ftmlcxge.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wjrxdpxr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wpewojgf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cybiyipb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3odcxxwmq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gprbxcra.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kkpgtsxf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3baobxllb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xqjevwmg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3sjkuelia.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kpzormzm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lvwvruuv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3taxmyuun.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dixczwac.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lfnryayo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xxdkdlgd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3uctkccjv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pfecskhq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3oonqzcfu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3phxtaonu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3buytofqt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wiwxdlem.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ncdizmev.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dcmtzgrn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nwrqozpa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3afhfkcbj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkycrr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rrlrqlld.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rzxsfqyu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lldynipd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iwozubdo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hvtkitzq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qfevkuyf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3caixgydd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rwfjkqcq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tjygckel.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dmcvegzm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3uaiwucem.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yjqzpmpk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hblkrtsl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fddeqmkr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3crbhdfgy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oijreppm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3udbihcnq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjqvxygi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ppbbfiyc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3acywwcoq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rtzrutgm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zjupomlw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pyvveqhc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ipvkzmug.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xgkjxxox.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wtyjoonb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suqwlkwp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jrhdrnln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nesmjmjj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3sicscbyk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uhclhjpw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mkivdwmb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tsjqrahg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qjmeymuz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pmtkgudx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lnxtidcc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xeqqmqde.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3epgxiguq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3attyjcqi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ekoojsdw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fsaynkgh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jcghycxg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ndatftqq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vngknmoh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lzciadcf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3guakhayz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jamhlgso.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mgphnlsc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ngnljoyf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rwwwshoi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mujzwzuo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hmbivzln.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aopwkaym.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3axccodiz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yekwrkue.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3thalrhzq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yyrehevi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yooesdys.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xtspgwga.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3csbtekpa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vjtriief.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ippxykwg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uxyjcpjz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oxzvnzfj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pucxmlmb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eruxpvtd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3iwkdifxi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xvmahwcs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zmjfztyp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hqrtooxk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fbdgcdpr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fbtnlwhc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xieckkoj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mvmucsbi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3yfuxbvdt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qfugovtk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cmdbwslf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vnciifoa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vwxnkthf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qyewtmvx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3vlvymajz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mdqqfnld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eggnhiok.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3tdvqemyv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3sykdspmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frakkkrp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nzxclhlc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3hmsfgmoi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ltaepdhs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3kfkwxcru.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hdwzjpku.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3axjblbxo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3igecmojs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ctxkxezp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3muxzzzkg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fhzimetl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jnxebxuw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xwuuxmpx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ylpikcxr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nftuaiet.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bsfhsebe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3odljipzx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3xabzgsel.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jmhnqbiw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ccxlhhbe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3nogidndb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bpcrvusm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hngxuzbw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xfghxryn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aocvrelv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ohliioew.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3usvtrzin.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3brjqiyjz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3amqtqwox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3amydeopn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exxvozrk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wfuzzqag.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfbfdq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gpewkvoj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ixjavdrs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wjahbddk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kvxxxist.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldldgdaf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdnmfyvg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rtmruftu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zjnaxjld.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vefnjdkq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pgbwrnop.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tioomucl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dovroggr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwuprtwp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qjycjkkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayiaumxt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqjupznf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jtscixkn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3wehglwwi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lckicnps.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mcyuzlgg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ulkxoffd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uaiuduku.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3oorhxcjo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mkwryzcr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dvrebfnv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dxuyyyjz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lcpprxqz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vrajzmyb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jtcuoblq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3njlrkzeb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ufwupoyx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qqgxvocg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sjoyvtcw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vidprlkf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jlmkhqml.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fiqkttcv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gubbktmw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rnnskfoy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qofljldo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3seccduqk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nzruqtpc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sxeomhju.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3saygzyph.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3scytqfpq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqxdfcq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xvxyikqv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uuyteqyl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xnzhrxjx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3kbwxnksr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zxfwgzte.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3mjufutxb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gycjekuy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ndgetsxi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eqezaeuo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eisuvptr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lrjpzudo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fswhfznr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyftxngy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qwkhnrhy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iijgvmmt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3aruulcld.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3giknmykq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hgfrgfhk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3aqzdjrwp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3crnbfuoo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tryhbxac.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wugsaggn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hjqwxswx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nljyvtwa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynmfzbbe.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qksmqkjv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdkpshg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3iyxpajvl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nadrzubf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vndhoxxv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmqlyhc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ciaflgpt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bastuomf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xlnabmua.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sifkemqo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lsoxreig.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqqqzhz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fzgyifht.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ctimazfy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tagpjpdt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vrainmdf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wxgylweu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lqpbvoxx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cboqtzqn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ziyzwdkz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwfkeyz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3krbqvfgr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xjplttso.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bxeiphxe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mzzhwaql.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyeuvbj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lbgaldnc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fxrnvrvt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wmrfhduw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ilkjexuk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjnsqryx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zvdynerx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ixktrjeb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhbblbm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3riqesuxg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3fnegvbic.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yckjhccy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vblnbyrp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wztqprtk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rgdnpnly.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ckeinbjt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jlxqbtld.html


<!-- 参考信息 -->