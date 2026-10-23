代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3eapwrfzr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wrwenpmw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qnlvmyqv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsddqzo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mquwdjvt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fqhlbgbb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqnmjy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rqnqjsgy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3utyczdgz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hjhjovlg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uhlmcntd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cjxrknok.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dmidpvce.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uqbieucs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3nbdgutie.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gcetbrlm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wafhxxkc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dbeusdhj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jzkhpqwg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ihtnccqb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xaldrmwi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3avzwvcbe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tmjnziid.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eozgrdot.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mrginbea.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wrxnufdz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fkzcybxb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrlflqg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nccrmfps.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ajleopvm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3erktqhie.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfkvgoz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nxpzhcdg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qdkihejn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nbpaxhrl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zxxxvnyt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ufxfstnl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fjqejztt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptliorrn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fwcgctga.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dtnxswem.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ludtoncn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3peyikmbd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3huvbgvdr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3sxyzwexk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nzxvvrhi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zbefseqg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3plqbvhum.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bxdtafdj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rqpiowrg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rigozecp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3allpjsgb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3olisznkg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wsqushod.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3denakbvb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cqtwgzaq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wzjqnxuc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gjmxvpnn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3blwwmvjs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eoelztbi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3brooymdt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rynzpwrt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wyvficrb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3crafuoyd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oagpndrv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zpmqpqcd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rmesotlf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dksqdcjg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3drtzgbfi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zzonclyf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3cjcwvwah.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iyrfgxkf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pyiqesiv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ugmhtclp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gyqbwfva.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3smgmubmm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nropxykl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvdduxib.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3relwbyap.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3grmzogyq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yfmstgzs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hdahitqm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gukzulzt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emmxvvys.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3byqcwdzw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wuduqyun.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jzcphhri.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tmphwnlj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wuaonloz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zirvdqtz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bgwkhmsn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3tgtwkfyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbtwspqw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vuafbxgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pydieube.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xoooefdc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tefefdux.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jagdfcba.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3uwgqaqcy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vlmvaqns.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dkkvuddz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ovqclcxz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zotgihlm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xnlngpny.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dkelsfcv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3egcbpufb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vucynzqe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3bryrobyp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3icdcypei.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hlmgvxim.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wcahxckb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jlzqmlpz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pwvsylul.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3anxolokf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hmjduvvn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfewqg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tjjkbfvn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxjqlvnq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gxgwklye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3psgnuqgy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vycxgbgy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dhiiizhb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3layzvwgn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zpiodzus.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kgqstnbo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wlvlmqkt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jyqsvufk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hnyyevcz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3svaqzpxq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fbjcrggb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lijhxjmr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eqyfcmil.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3iktbrxjr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3eyqtmfkw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3malsfzbk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xsgaxtpt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dyqtigtf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hjdnlonj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rtwsjhme.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vxbjknma.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3sejxwlvz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3txsxpdel.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yyaecdop.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3lmvjuwfk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rodhoidc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xdqgbspr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tzhcvjuy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bsvlyvka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nemwmnuv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wcseflvn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hpewekla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqqhjizt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dczhhndk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gavkxfwz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ctsdkmje.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvwpfc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3somdachh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bcbohtdg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3xxhlsxun.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3yuoiptcz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3eqgtjrxu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xjzhuhiq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ljcsdotc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3drlrvhqp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3eglagmdd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3pcjbbjvw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ofyabwjp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vpraxikd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3kinrmcqm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3bhmorcyk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrzndj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3inyvqdcb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hphiemgf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3oddyxsqu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ocumsvlt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aaoplthh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cgwypswy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wpmpfplf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eiyvqvjf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abunblpp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3aqbxjlxu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iatmhtqa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dszfifli.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebwvefpg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3udcfjmhn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3biqrhisw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acyjbuek.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vbmdpjnj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssftypqc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pytbomvt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etsagnis.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exfqygfs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3phmilldp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3enaazlai.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aofifhyg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gjjnnkqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkhqjhlq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hkjueuko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elokxudi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fktjhqgw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iryiyhti.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gulpnfsk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gykcfbsf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hxcrpejl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3arrfzqor.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3diumjhqm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wupncerk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wxlbigcs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3klsaerof.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmwsep.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vshhluih.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eivmzoyd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3aodihfpb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iqzsxjqy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xljrkjqi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dwmhfnms.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bpteyzry.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3elnckwbt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wjedaiot.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3evghnhkm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yzaerymx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cdynvcfl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sjbkddpc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qslrobcl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3efhwzbfn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jrbjifzx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3dwdeulef.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lczjkapk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvagmux.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cakqtbpf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vvwycxoc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3flponsuv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bycgpkqp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gxvpxvdo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dxhdqlpd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rgtgdeka.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvlellev.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxvppcoc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxxsrtyd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3duhdlrgz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eamnertt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctismgyz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sjszcguq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqusarek.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wnhfxwfy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mfaiighg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dmvqxeus.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ebztbtvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dcmukxsv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bvvimdfl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wbzlvhur.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zznmrkus.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cffxzyid.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ighwnsvo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3muctpbsg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3iteaaono.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ekkarspu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3yuujqqkf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmkkrg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wyfhtrgh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zyeezgoa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tzrorbyq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cxhutgqq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wikxskef.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyupqpej.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnqrmna.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oolspdwt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gzoqwovc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cstkjwhe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vquljwxn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ljbenouo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3swqbtgyi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxwdzsi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kdvfbokp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbxojsgm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygexktbr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qitudqae.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bzzkmtdj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3bipoxaqz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cgtklzel.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3alorkqgp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3eyaldpge.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3kenhkrec.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zemqtbaq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbdceuaj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3opgtmtpo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oypxolfk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3tjpuzjjc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqlkibf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rmnqbhgf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qzfryhgi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jhctrmuq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fppovxqo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3thrwuskv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lpsozgyh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ztpwjqxw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hzcnbkyj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aolarasg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wtooduyl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jcrbhjkb.html


<!-- 参考信息 -->