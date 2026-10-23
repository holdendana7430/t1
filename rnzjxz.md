代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rcyycgtd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wjeouxoz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xmgwnamy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3knmhmihh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ottwkjbg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmqelbh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3khosjcfw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ouuaarwz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3guyendrm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hnduvwjk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fbjenecw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3thaynrzm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xmduiyma.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vvyvuruc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qoiqipra.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3akercmxl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qsmvhicu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wwhugvwr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3uhedzoaa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rlawonvl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjnhzt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ywzlssum.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bisfjoml.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fztaxftk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hlpznjrh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ajnsobly.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3fellyugq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tdbykjky.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3zyypxnru.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3aiyqdqyl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kjbxhaup.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aailjczo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cbuuyczv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3gytfdfgq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jkdrbgat.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3trtukdla.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zexznswq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wzajgfqj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gpqvdpjw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqspffiq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ihehwloh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3anducfwf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jnlrdqut.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkzorze.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3lyqcezfm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cioehxez.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvwwydvm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kfbapitu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bkwfpnbn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ynxmfgol.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3madrpmai.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfnjnh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3njkuocak.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oltmaxvp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gypglgcq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bgpbzomo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xncbjksr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ifxtchom.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zptwpbzi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzdeeta.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mcbjgilg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mofbtgzy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dltoeaqx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lrqwdgna.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hayqklnn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hrwxqsvo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3chnppqau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xcilxnwt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3typckpga.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pojfbjdg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tryjcxyw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tvnaozlk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hcaxyvnm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qocwwvfg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qqyqqgbm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gihpdwgr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvesqfuv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qxswehmr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yvmvneel.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3znfpvvtv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3prkixlrl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jqtehbly.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kkukfwnv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gpkaswgf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kqymlrfh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhktgrwr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pwiuzlrm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3psrwclne.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ffaqcwxv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3znczywjd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gfajpino.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogzokyyu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hbvjkhss.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bkcidcxg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3whjyogia.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hqusmcrq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rrxawtrr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yoyfdyvs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3serrwhqe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xaosaqpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmixkzmf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xmafngpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgawtope.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gtgmsoqc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ymcsydcn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lucmyhsl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3mqdmzbnm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nymkymmk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxjmtfnz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yajbwcok.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xcnyrork.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rrathxsz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dzegrgkm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rseequol.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3baweyvgk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hwzajugy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ikojvnoq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yvfewyxd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3brkbtutk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3crfuimfi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uqzkhjev.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmgbjslq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yxuxzyqs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3djfltbjk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3slgryfmd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jddfzgtn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kgmavevp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vycadiip.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bvlcfexh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tlgadvor.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3betzxweh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3shtlmwdq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gyppanty.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3detzlugv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qbxkxzxl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bygxffdl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mnuebtfg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pweahqek.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3avuobjhj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hlgeabza.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kycktnzc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zbgiayhy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3fcodjhwt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pukeiokt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dbzxvlme.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iuygmksz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zdiubuoq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3odlukpem.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3okqyzttx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nacxdwyp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gbpkjnsc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ijtbosod.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bcequoux.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hdjdlgoo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ljtodipj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3powalezp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btshxuch.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ahvpqhqp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ioaiftuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3facbcnwr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3mrviracc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bzxgduke.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3scylxpbx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3idxoxzzy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ihalvlov.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3igxydcxf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zuwfeuhf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3scqgkyyw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3svoyzhtg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3tudjzqnf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3svcyregj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yddxvxjb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bpovkgse.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rwkdemfv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3frulsfbc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3lzurhebq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hlvnyvcy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rowkmflw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dzwywxso.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3oqfqynpb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xlgwwmbe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xmtsigpq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3skyjpcae.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njlwlpjw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3czobegjh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tcenslcn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqobsrpb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sombpyfk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cgrksklg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vknqewgs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3irttoxwd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xvhrkesx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3babipfay.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3efpoowhk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3couapbbe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tkwghmyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shltcors.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esrkbwjq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdimixae.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjajthno.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3isnckwkt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbuuklsg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jhlhqiax.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdllcqmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3figfsqtr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rtmvsshu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3octrbfod.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fykmqbyb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fkvdzmgd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pyjltqwk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dacfrbxi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3uriimlaf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3svpavpvj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dtnlrgvz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hnzntdnh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gdcuysmg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mifotjcp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3geibbrqg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qdgoarqh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hynvkmkf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3umwskpvu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qbfndhnr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3nsaluwsb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3inknhysw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wsyahbgq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3hcrzxked.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3spmjzvpn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tyzbappt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xnjyesrm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3otkqufue.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qzvoqlec.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jwqywlob.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jznnixvc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ykfvneex.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gxvdqzcu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3xmlwlyha.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyqfdoo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pzbhwzur.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fohhgyhx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jwbxkqkk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lmggqono.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xejqrmfk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ggvtpfad.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ykhzenyi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xivbdssz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wjgqxfao.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yhpoqaxi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bwcagrhm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rustkbga.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmytmtli.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sxiejloj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3idiqvpec.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qghnlzcv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uptnsbwa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rouiflor.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kvknwrpp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbimyjs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bozheoyc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tnxmdsxd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3knosqore.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3koqnbpyy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rksgncjv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ifumheil.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dlqytran.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pntfewnh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3flvvocng.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aviyybez.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3thvjvdib.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3khhoybhw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hrijllhn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3khxmjmjw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjhphyl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ekppaiwo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fovuxvub.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3obgiyirp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jdaaawbf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ooevexyu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3pyngjgql.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3olihpgav.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3prypwjcp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yczyxdvg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjyvmzhq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbzmpwho.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cesfytkw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3btvpzrdn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3opzfvbvr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3morugrgt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gszbdmzr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vzufixpq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xviromep.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tctwtwwa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqgfmwkt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vwwrgcja.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqlosmal.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wdwyapcp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vpxgzryb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3sdhwkpea.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ovbvyzhm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vfatcbov.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dsvcikvm.html


<!-- 参考信息 -->