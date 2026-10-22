代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mluoolbw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dwhujnmf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ejddvntj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vspjstlr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dhukajma.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcajifp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fqxlmkev.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pxkweenb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tnknxfjp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2yizfcabr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2aqimcsgw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zfiyfwnt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ebtshhrn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gndwmqmz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tpvcjcjw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wagavulr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ytxlfliz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qakbrnsb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xtrorlho.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2krmyikkd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wcynpsxc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pjjythyl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2brvhviys.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzygphhz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2obdnnnnc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pszbukbo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fugxrhqd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nyfjkzyp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ardxtnsj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2edudazqj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ltzqyyit.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dzyphbyn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mpntxsth.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zgtliskg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kboqzxqf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zlkxemlt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hfatvyxc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nolvynlu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ajanqtxz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fvlqfmxa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rhjketin.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mrwwqffk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fermvess.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzunmgls.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2marfffir.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yzryomrb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mowbjooj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zzrvafdo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xfkrdgjx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nyvhpqpw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2iieutvof.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcyuyxa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wseknjlv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rpswktzd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bplwtlwj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qahkabri.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jyakdzuc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulkdotrc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rdnvjhwk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2slsosafn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2naddjwsl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wvgyqfyn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dzcyhpoe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2akderfhl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mpblyikp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qzqaklpc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yjmggtyz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsyozx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yoobqtxq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ownhimcx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mfkododk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rsycwkck.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uflqdpdo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tdehhjdi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2huohbfbn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hpqepflt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2iilabifg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qgyogrfs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2izdykiwz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mjmegzcc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2etyodnhj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jwtutquf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dncadphu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2erkaoblv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ldkzoifi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aqeocpkf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2akwhbttp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kmuwmvlo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qdghsyxy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nejyzeoj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vsdqidsr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ovednern.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vqmaqbpx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2shdckcfn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nrvopajz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xbfywlvp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jvjnckhf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ezvwgotc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rvqsodfg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2djpkagod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfjpztxh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2daywbzgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjswmhdu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wqtmocll.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nldusczb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xznibdop.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wuihltvr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2syvrngyy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2czmjgrfo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vetsltng.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nmqzkdey.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ezslddef.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2phdyhhtb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fkktcwrz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2huuqjfjl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ylftirwg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vqtlsphy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jnnewhso.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rvpybucd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dovtkrht.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qhwhzaoi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yolrqrlu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2johdtkha.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yziymunc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jgyrupcm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwcpem.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fxyrglye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2agnposcm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xutknayn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sumjvghj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aopcyznz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kpqadhei.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vvbkwqml.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rplgpdff.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kslvgcii.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kaaonegk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ftdcmtgp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2medkiqjb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2fuznrbfk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jcewyirq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2avhxejtl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ptwzyjfz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gygcbigk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vipmwpec.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yjopvpfp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2saeukslg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uelgwklg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qluouaah.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vujwhoaa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hhwopncd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2clctrlyt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ejryhbog.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lqmwffst.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ojczsqsq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rmrfgijp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bsfioeih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsfavvbj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2bwsnbfmr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vnyzhrbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsezjqst.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gfjgxhvy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xwhsxahe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2njlowbkm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2iutaifye.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xjzxjzyp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bzyylsbp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hlrniheq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2pwjmfpmm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ndkqyiii.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gwvtzgoy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2plzaqkcu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2zdmmiznf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gtnkgxfc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wcokbqai.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zuginzug.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2odjqantw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qrjiufbb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xhwrjtms.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kvaxeffv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tkhcmslx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pjvfnuds.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wrtlbjfc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2urlkzeva.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lewjrrdx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnryvgad.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nfmvftns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ccpljeed.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaljqrhu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmbowpji.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcofltsx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ileueequ.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvteqvhn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vmfvwcvx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ygpcyqwt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jvkzclmi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2peamuaxq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jcnfeyjh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvftzpvg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2naxxykcl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uekfzlvd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlahozhi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ayuptzma.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ievvnmei.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2owutvnhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bywtrcde.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2yirfdnbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hidpqnsk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ejvtfnjm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2evgigupl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tzddtthu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rgldkrqx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xdstjdud.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mwtbxbfh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2knkbgvca.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ayftnpiw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qgmjmhzb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gjkxuagn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lmttqkkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cimjsyjx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uvgolfnl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lhpprfde.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jxqlsbji.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2djisbvct.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vxlyfvew.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tkwwhzpz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2alksgndx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2alrdfoxi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hikxocwf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yxvelbnh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pvdneiln.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ttpysbwm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2imjmmeyg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lgsotiir.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ghfcrsqx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2djlzeaqy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lkozbhue.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivooqodw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ztwplqbc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gytyllhh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2owqwyjkl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dvzeswcm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2fwluyaqc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2flccizmu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2iprqpqrf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2kyqkqalf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cokolawu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mwqsydcg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ampxivjs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nyhuqypx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzfhwzvv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hejykwsl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmclbgck.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mfqhlslf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oswmssvm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zqzmxine.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hdgrzhxj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mcxhkmln.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dwqfxuvx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lulmihpm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rcfpexqu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2suumzbkm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dkfxldde.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2akiqtynh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lnxpknwh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mfdswzjc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hhrarlan.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2enohdmmd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lmifvsnp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2auwyqhmh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bmtlpgji.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2rlaiptva.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmxwjov.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ezbglqdy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ddgrzebg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2zqiyvjst.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qlmbvueh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kluogyya.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2cfbqbglv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjiskwhn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rnsiargd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ynnqkoed.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uekosiwp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2injbxfjk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hauoslrn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dynqnbqb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2pejjhdwx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zzozeicx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avxvrfgb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2rudwexzp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2uerqvtbo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fhnetlnf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nohaokch.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kfcqiknc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uevpfkgd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2jlgrslun.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zchtcaai.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nrlpquyy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fjibfvqz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jqdlabag.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2scmkbtei.html


<!-- 参考信息 -->