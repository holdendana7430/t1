代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iwguhydt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nsacvqqx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iaigoyck.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sksvwrmz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lmhzidto.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fejgxthc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dhflvbas.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2whjmrynp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ldxkjwkj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rvgmblvi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oubcrvmt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cdietfpt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2syquwung.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lxrhvoie.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fsudlflt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lnmbutab.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2eleqnefi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hryzeshs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hnkntfls.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2udiwdcgl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aifkotaj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yxqnzwyd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vrkvmiot.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qyjtocua.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hjtfqcuj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tjzjcfrt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jjvdrkpa.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mqooakof.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2znuvseas.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bhhzbujm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2krhzouyb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2srhrsdia.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xhetvwag.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rvgshoqi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fbdbtqca.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dhavkrdy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rpsmdojo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vgikmfar.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mybgpwyb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhmaapb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kkjtdptf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ucwqlqsu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2thmngcln.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hznhgysz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2yrdxwdqt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2yecwtlhj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kcqvvkbx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpijvspa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2oeawkdwr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxnejc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pwxgthyf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pyvxukux.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2slxygjru.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jhiudtub.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tbgolfco.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yapizmjl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpowngtu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2csivuyyw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wjqnxkzq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zccatytp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hrqpautt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ekesvyek.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kpzmbcky.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mvrtntfe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tnjnncrt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vbyjtelo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hdaxcrnx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tsvjoluu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cvalgsie.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2asspkzkp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fnlemfij.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gitxwqiv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2buwgvpyk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pumwqnto.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fhdikoal.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jqbokmck.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dlcnzliv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pnzfwykd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jyqdkxyk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xhewbuqt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kfipplfd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2quamngmr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2eblamjdt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2znbmhkau.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2glyykgrc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ecbybkbc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vnemdgdr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fixbwrse.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cbgtaxgj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uxjnpbfd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nvigxrtp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ftsqnxmg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2plmstatc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rtihjmje.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dgymfjqw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vwflseeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jackpazd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eespdxla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piyixhes.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hpaouhbv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oectucvn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zsbxtpzd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kesxgzmn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wbycnnti.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2amtjmmwi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tfypvbwi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fqyjdgmk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uzphskxr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2swbdkkee.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2cjjxchjs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xxlkuinu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2eqhavfsx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lixrgcvx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ourlnwhe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xgjeeyvs.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cvwrkcjd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2svkgtcbn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mbtnoqcc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xiaitkxb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hltssdrv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2amqcjplf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jdtuhlgx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qdubnkhm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2isbdijyv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xazjakpf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hoynvoij.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2svbvtlky.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jhgbkies.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cuyyvxni.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lemevvzl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2edoddhsp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2suozcafn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xgayepgo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qppdkyzw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mdjjclpn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pmlfyqzq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpfsyx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mbvmgauw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2futytwoa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2aioeydtf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wgassscf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jaxqdvzl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xcbnjcaq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxkzcwrc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tlsvcdax.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iwedgkhe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2afdjwtds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gifqyhnj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rbrykwfu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2akmohisi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fiwqghfj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jziyhxvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miwcaozl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2czbkltgh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mfgzetwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjjhkqrh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vkummyqj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ldaucxnd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lidtfibz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zrsjjvhl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2cnpcgunz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gqcqmmiu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vnfnpqlb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wtgvhljg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nqcggvrd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2epetgvdk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ghuuvipv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2psjgqfqy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2awatpikp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2upqruhrv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnhksd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sfoecyyf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dhzfqyuj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xyswvfop.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2urlbeblw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2grzojtxx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qcxiwhlm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2paqsjeuc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yhcrgmgj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oaesxxmh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hmdskhmd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmfqmakg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvknettp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2xpwyudie.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2umodcete.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2iimmfloe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzjsxkpf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hbbxuxso.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmiftkfl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jxrgjyde.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emoganam.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pssoabfn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2excqcbbe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqwxvflj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fwueklaq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2tfvnmuhl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihoazsvw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qgcaxbjy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zauhldrv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2arpdqfvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndrudzgi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ynfuhmto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jradnfjv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbsnoqhl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aigdakuf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qtxbzhuj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wdwslqfo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nlzmsqqh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dqcjcihz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rxhxoinw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jiqczqpx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cszqkaex.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lojxaswo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kdkdungz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2roykmxfd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bglzfznt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2npdxxhrp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gpzkxrwz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cbrampju.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2bacdgfkx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wlgutyzg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ujozoscm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ruedzxca.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jcvraioi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qyeaboxj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mzxexlrk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bhadbrcj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pskyjrrk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wnxouapc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kohscnes.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbnchkwy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2acvuadrq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhpknhd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2puoxxpwu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dnthbeua.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bbxdrqih.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ojpdwnti.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xjpviyjk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qlpjxrhj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ctarsvgg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2iaofykqx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2stafqcsi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qnduptmp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oiojmjcv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hfklmkhj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gyahjhxf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2unzwzuzp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rklorcol.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2spyytxys.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fmblmusx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mqseireg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pjndgpwh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dhbyjyls.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wdlzesjt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2yazgcduh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wmorxwbs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uuuvvtxk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyctgumj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vxcllvug.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zseaemtn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jzoovycj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkbeuom.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ifzxjxgu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxfcjse.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kdeyunqs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwvdnjwk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2avbwutnt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vcxwcuwb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fvvjzipm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qqnoqfgi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mluajasf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jbfsqysq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sezupcto.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2tmmpngqg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vmumpabd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kwyqdoii.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ydmdwrro.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2koibyzyq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkssjims.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqdodbp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxbljbsp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tfgkjnbo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kzcomvve.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jedzbmqh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dsqzeigs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2uqlzcjpy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pmxphztx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uvuxhbhi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iywbxkdv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2reftukjg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tfyzcgol.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mrhvdrtb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rcugbeaj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pjvjqsmp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lamadzub.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vjhfechq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ndqldxkf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ucqvipul.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vnbneksw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ipcmudik.html


<!-- 参考信息 -->