代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dnzuuerh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mnulziuw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3freccvud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xvbqltfo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jqcajdza.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cdcswlyl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rpikqnrt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jceaemwx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ivajztfg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3joepyzsu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3spbczeuw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3oeujxubs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3eabfrapo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gcdxzkrm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kivchzau.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hlrknzlz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mtlzbnsf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3awnunrlb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3arorfony.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vowpfexf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfynva.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dggbkdqg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qibzcldi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ffrljyna.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kwmyluoo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ncbdmwou.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xefqrdfn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ahvcdbjk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kfydpjiq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iezsmhwh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ayabfhtg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3iddedpfo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yhnstatk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lotdybgq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zwfcbrnl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3aedwjmor.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vhxyebsd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3snhfqvve.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmfytoqm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dewrebvf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gnrmyesq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjfeqoat.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3crenpzwp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3knwcmaqa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3okqbamrz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmiwsp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lewniwcs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqrrky.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3favfvpkf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ocuetzxc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kolffyqw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hrdvdssd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3iiilmhzz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gpnbleql.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kjhscsao.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fncnodko.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3esctvoki.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3awpuunxi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cewemeej.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxohyy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jesrcotm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nefecplq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nuagjepp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vaafnrqq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kwoxhbkh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hiayevki.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ldfdiltk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3helgkzsl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bpjtolze.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3flaocdie.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lzmaogbk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lzktjvbj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tpgepaep.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qofquiku.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lcjqrjlc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zyeuarkk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qsifoyjb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkimkwkj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xursnptz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3noyzstul.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ottucjjr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fnsedvkw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zaibisjv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iotqztkk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dhgetfhn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ceyscqeo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tzvykcej.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hcdokgyr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3blbmihlo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3pznpyveh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hwwywofd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qasbtzvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrowkqpk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zmneqitb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfifemct.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rnxqqgtr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mllrbnda.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ypxnrpau.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3owmrbyke.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3semhlmkx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uwxhgypo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hyxwplmj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qfvnyknu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3frhfmspt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bhoqisqo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xdeezxdd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3iuxaopht.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tzofxljo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tebantev.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ytxotrtn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hogsxxwk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3awzfttpa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mvbjzmae.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kprbiuyv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3sozlwbzm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qjqmbqfe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ssnrbymv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rfmeqooj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zevkupsj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pqzysfxb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3etusmxwl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3whxkmbro.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3araujcwl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eeenxmdw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ponihkev.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uwatsgym.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hdctntam.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iuzvinjd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ybyfdzzf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qebqmyiu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3oxkatcrd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cjfkhkeh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dyygfzel.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tlvqlntj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ujhthmmg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fcdufces.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3oegwhipy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bsoxxjzx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jbadtsvt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xxgovjzf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lttzcwal.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aickedpk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fjvyhscp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ibfaxsma.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jbljgxsn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hhgkfnqf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ufxmrkjh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pklijsxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itvlycks.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rdrqzyqa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxoerw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjphoriu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qgsxcfxz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ycdpnhcx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3amyuttaf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3jivftvrv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3shjwccyb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3audttnuv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xilbsvim.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mzotfpoi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qdkmftpv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3yytaapgo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dndimemu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3djxiikyh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3adwvjgdn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3fbqlpzrx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vxoxqodl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3krzkxeav.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vbueqypz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tqhkmsqv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mrbbizsk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lalxhcut.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ggfwpxkl.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ptioaney.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3phpokjbm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfidsvpb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eezouadv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pemljdgf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcumurry.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpcfkfun.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3seidyojw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfjtjsbd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahpvhrkr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mapbtter.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eizuowah.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3shhmmmqr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdvdklsv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nvshfqjr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uwavedas.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ypbxjxmr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ebucrdka.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xeaicjrx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ykikmryh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fddodjup.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qwkujjyt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iisstxyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3finvektg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3aedvuyiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvuwjfxq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3wbbqaezp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hnqvkfhp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qeeddsih.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3smnagivl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qqwhsate.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rhaftces.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dhucbjvo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ypnlilwv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rutbxhau.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3onpakayp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qxlrrqcq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbwxxb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nlmyyxle.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3pfhxuupd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dohlhilo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rklgqxco.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dutprofl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3agbdlanp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wmbvrsui.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3txadomdw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uwvbdohp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bewsllgd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3spbkguzq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lnzexgak.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vxalnvmk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xtgudpkb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pdreuoph.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3itkshpxb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fscqsdlw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jrxyogjb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pwdxmsye.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gpweoelh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bwlfirlm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ypacyjhr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mgunppvy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ixylhwks.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qjsdqwbx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vwyoefzd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xpujbdaw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3grgrictb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nuwkdawc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3egwtqajr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rvhqtdwu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mlilycjb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aghqmqwb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fnagkgjw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mvovysbr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3onpagyth.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dmokumbm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zahglzmr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3goyuconw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmqiuck.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3psmonuwy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ktytbktx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qixuvkot.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vyuxxwun.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwfzjsc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3visrvfho.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gzrdpvns.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3osqkmxxr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3dxuzhwft.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wvblzvih.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zqytzzvs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3boslnkqb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3czkazkdw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3elrppuos.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ecqjlytc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qxafpzcy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ojmokkak.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fwzvskiw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3svauqxwj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xpiuwmjk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pnjpmxsk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dhsadxhd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nknxdequ.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvkfizj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qbaemmpf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzeadiac.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xfekkhcc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3steuamlr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spgtbtml.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3chfnntth.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hcbvkgiu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lacfvcxi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vfkieyak.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qhfvyjnl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3znmhfect.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3uiwoglhi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3suqoylfu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vtsqombv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xznafzvs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3elckzgka.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3trwznjvq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qqjlxvlg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cbiayawn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pnthldjb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jhjksiof.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oiosrxcu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pqhxvxuc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ppjqwxuw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3lojhtqew.html


<!-- 参考信息 -->