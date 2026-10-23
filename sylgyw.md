代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wojixxoy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ifsasaxd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qchudwsi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hdxlskeg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3efnnxrbe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3twfceuot.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nzcsxigm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ijpieqbw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yogjhslp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3oczczxxt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fyexihzf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zxbdpndh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3thyplqei.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cgvwsexx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fyzteome.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gvholxan.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lspuppmz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tlbawdqt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pqzmxxir.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lyklkgwj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tgknwzau.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3svlgcrqk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mknaxoty.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sdjuyjgu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ixftnrma.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pvilozxz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zlutdzyf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qeyninuf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gtxxkgbb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fvvsmhua.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ujucocpj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kylnjpgi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sboffnbz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tbvearra.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ofltobdk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjibndml.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vsodnfqq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qrayycno.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vwoodbbv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yaqbpssk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjvaxejk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ypbfkbbb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikwwdqhs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nhputqxm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3auevuews.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3szzwddrn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nwiqosyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hdyrrukn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vhuorkqc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oaljfnuk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tkgvlgsr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qfadzkkw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oxyyveaz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vyzgjlgh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3byepizoy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rkyzgucb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxghcreq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nahnwmfn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gybinkjb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jdvdjuzq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fhimyzln.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vdfnngif.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dxxvsuwx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wfujfeyt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3algxnkhl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3heaaywtn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3akhuegdr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3oxmriimk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3emumnxxt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkofbys.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bnuzzrnk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cosmvces.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mlqkclzs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iztbrucj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mmnteilf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jzhxutoh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3srovwpzk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gqlzqrtx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3glssqooe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pgtwmflh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3luewzdwz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lcflvuxp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nwfcualw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xulujtlj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rfwzmjkm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3druqfmgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vdiueenu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzfhsksi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aixwnnuc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wakshddr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xdeyquhq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ydhsszym.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jtlssfcd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bexqffea.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dkbpukqu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yhzvobcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxsfderm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ugxmteoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecslfali.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lguxntlf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fzsrjryk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ijcucbkw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aviqjbsw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kcyjpptm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zhvardek.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmplqnuy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3luojkpnq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hqcxgnjk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vlvfxdhb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fipnlhpi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xckzlyeo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3essjpwxx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nluqoako.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3prhxxwap.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cwfqbphj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3orhnryqe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qpbymkzw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3adxjkcdy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3mtmcxswf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zeijqwaa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mzgnpnjp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3trevjipb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3phxpurze.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xqymxdgj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rtzvappu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rlgdbqwb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ksygddsx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3yepwgrya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eipvrabx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aaairuau.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sanepjrr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mclnyhlh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qlzrhode.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gjvtiwgz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3uiebuoiv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hrrnnjuo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3snfkipud.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mnpachgi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bvzwdusu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fvoqdknq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3rlkwljfd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3soxteyoi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3atnvoimj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jedjfemf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xyglnwme.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3banqnwlk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3twacqeli.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zqwecfmw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3yhnyxmoj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3laovsuqz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ivdkkhvv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rltmbetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izinfeun.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xijdmirw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wcmkberw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zggecbnj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3iouvmljs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bsolauaj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3nsvovpwn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3tcexfjew.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3elagqdwa.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3baolbiru.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ikexjjqp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3gvkbsgng.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3oxrcfekt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3owpmdcde.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3agwtdgnz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ewrdfhaj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wmpevcvv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xjyqvqpc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3gwghvzex.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wfhcipeb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rexatlap.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qcbhgnyy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3sthedemu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cwzrerny.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3niaqvrbr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3gkasatlj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ohhpuqwh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mbdulodc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfsysfrl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gjjbfrjc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pyvlkejz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbljyvig.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcglgzhi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xnawedvz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skdoqqrz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kklamgey.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nrwcwfdb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdpllhdq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rsbgwqzm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xlueuzxj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpepqeje.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3amlefwpq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gasceejx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnksjtdg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dgemhhnl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pauldynj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xxsnfnow.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uyzwkxzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oidcktff.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ajfkwxiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysbecumg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ogzwdmdt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mchfdail.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tpfkdlsd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ockcuhqe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3khnwuqfi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xyswnxro.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3voollrhs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3urnhmlyh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ifcgmrzl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jegjnlml.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3eehfyiml.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yjvprhin.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kplfjdco.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rwxgrtkr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gpcozxpx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3vjnfahma.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jfmylgef.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rjdwknhn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mhkkubpo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xisobwcr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pcsitzwr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wsajnjat.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqlxxwsa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mladatqc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3negeclug.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vfgvmblf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzvindub.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgniiwpe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rzogrhly.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3meluyfkg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xxxaeueg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lxqpuavv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3kaijgbww.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vcdbunny.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lylllzea.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gktnobaz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qzoitqvs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3crnfwvup.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqfxaelr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fzgdpemt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rfufkqzr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umdnoexa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dwejmncc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rhgodpmx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwqukddh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lrkcvbij.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ufizgpmr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3moppgzaj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jbzvbgtc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dybsrwem.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3egjhjgfp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tiobsvge.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qgpzcfje.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tboyrnnm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibwednkr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qkbggtlm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aegndxcg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3synygwia.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjnxpri.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ntcjelmb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qighdvtq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jitevhbt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dxtqwktk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qpgurslu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jnbaqvus.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mybaerhb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mdllzsmt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqsfrod.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3puezebmp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nmybjajo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3auyqsipq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jybgjwqh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kgonrtxm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkcwxnuh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3htygpced.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3crfshjlg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdhyvry.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txkpbexs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jceuopoq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cbjwdvyi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrnpsvca.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3txbocrzz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmsiwbj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mfpbixdc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jwihkurx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sulxmxlp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkmgalrb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wdnjzroz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jzdzjnhl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3htmagshj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jfbfvkgd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vkiqvqok.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jckloqyj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tucrbeaz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xbjaohdw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aoidajpm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zriiprfi.html


<!-- 参考信息 -->