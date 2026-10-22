代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lnnbdfmd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rntbtjra.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2owgaeedk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dssvrcxb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rhmfnulb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2esnfjdpt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tshvaerh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qlfzefzt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qeucifwv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fefdutoi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jhfnvstw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tijuwlbz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2opqolqsu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wocyqriy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xggwplcv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2goxzhdfb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vcnelxem.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ukqrpagd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ogbvzvvw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dqbfdfjz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vohndbfq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bczrkobz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lvifuqfz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2igwbisig.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rpkuzpql.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2otigywwg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftoxzrru.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vyzwytos.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2poxfefft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fwnrjdlc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2uroqkkea.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvuzcopk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drvmedzq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mgktsrti.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qkfladop.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ozsurlxa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wmmextmg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xxzlggga.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2imdsqknt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgsroqj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2bllymbgj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pnpseiwe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2udixdnuu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jmnpbtdo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hkaeecgp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sbouhtnb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mdbwjprb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bmsfmliq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2rogkhwad.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jnacvjfb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vmmkpexc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ozhkxtnc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mcdenivf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mralhcxw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hforrucn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vtmzbfnq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cfgvovtq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wnoqmsal.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iijytsjt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2thyfqiud.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bdzjdvxn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jcaprfcc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fxmyetib.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lrvpgwin.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2secgavfs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bjfdsyzv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pcbalpvw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlmvmo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2akcpcrle.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nhhmsree.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ovjubrnt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wlwpswoj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2biyztpne.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2neklmnti.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ibduavss.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2afqdsxdw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bfbkgaot.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jiuznncy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ntgsuqse.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2iscanywg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rigkfkcj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fjvawciu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hujjgejq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2kowrmdkf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lekgqcqc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nsirrjdh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2daxkkyhq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ibqbwiqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzoinqgf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eerszqqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvgmifvv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ilznjpmx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2unqewvwr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bmfyrobf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bkffxghh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kstutosh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gcxgxojl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfybvybu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vhijczlf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kegijpgs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zqxabbel.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wxmvufrs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2minxndmx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ctsowuxv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ezokwjde.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2duulpuio.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2hpslaxsl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kxytjeeg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yxabxauh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jniaeyvk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rzmeects.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lzzszvvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kqfxhdsq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gkveheec.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iwryyoau.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gzyjurpr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fzxyvazv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tdxcwmck.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wlyxaihw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uuiuxwpr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dcdynout.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rhhrphbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xggeyrhz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2inqcdhss.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gzamwjeo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gnmhzsyp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gjumnacv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ygcgcvno.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ahgdddgh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2pzdriguo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mmpnnqox.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2isbnhgcq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2oxvjkgcw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wstyxjjw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rclurcus.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kkuonvhs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2buivfelg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jtdnuwfz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2jbjzjhzf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gzdtcsga.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xtfkaenm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vsydjdfz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2satknkil.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fceowwnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifvshgqi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2luwhednz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hbnlirsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewcuxpvd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fgcrssph.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2qmewibbd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gczzubob.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wxocnuci.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bwhxqpgx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pjpfzvnz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jtjofrrf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rhopbgcn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zwbdqpji.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2uoygrikd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ywkvpsqt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2efkrxbfi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2coblzict.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vjyslvhz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2cqskctyl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bmhhmwve.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2abwnyrib.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ckzgfdxm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qwodselz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vyjaudpl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2muiquwhw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vbinzuwu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uqkvbnzr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ibljlduc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wsyxsgyt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nvirulqj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fcayadmt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2drqstlms.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nemfdmre.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjjukzkm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2llxmaemu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zhberhsu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zovwveja.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yujelvuj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ejwvvvoy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2broqvjvd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xflgmiod.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2eiyjybyt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ialzxkis.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2kixoeqdg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqcditqd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ccpylslb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vrdldddw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lltnhnbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogotpptb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmoodmbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kblmxwju.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yqlxbjsq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2miszbckb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xzaqbauz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jdwwttal.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2uxhsvthw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ocsukqkg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ikwxselw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qybpxnfz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2njeryfef.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vtitthre.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mhjnkvue.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mzcvkwgc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sxiizzma.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mbwnywea.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gzlsilzi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2axcdmwyh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2axwvkjge.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oehgisbx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ojqxdazc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pvpcxuqg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kuyzcqsu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xxyljlej.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vnalrqza.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nnvkqrgq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xvfvuljs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2feniigoh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fmggqspc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjkiaoaj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rdnoosrs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zqlvtcgg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ovtktlea.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dvpciclk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2knrazmlf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2opgrijzw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2uzjppqdu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wbblpuvd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wfufatha.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fxwiqyos.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2btzdnajx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbfgiroh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktcvmfaa.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbtyzqrx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kuossweu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lfydngpv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wtizyvfu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qhiwfxbm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lgpktzsk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mszoaqpl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fnquvhmp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2byjhkarz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aflpwgct.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eweqjsxr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2npodhxik.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2whtxnaij.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cyswwboh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fcjvwerj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kutjefvz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wactqury.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zeazuiyf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2khlkofes.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tuonfsxg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2nunpdwcs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbhdgcm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ygnvzfqa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xkggrogm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2gepfejsc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wivwyrwz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnlnna.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ampsukhs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mlzaztol.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vaszyigz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hjspkukd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2micmddss.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ornrxezb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2truyntbq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ygevhzzm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xfdsihiw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txhdkgdg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2stnksqpo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2uvzimigj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yiqipvzu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wxyhzlgr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fnaosoho.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jkxlwwya.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ptkjltyn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aiuapqlh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ciyhwtvo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xstomtto.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrdlrjq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2abzccpuj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mpsuclti.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kytdnjvz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2chpgtagz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mfzmqoyj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gofndzqa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tervdudg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2cnqihgpi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lurbmydg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fxmjpoxi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ovkcybwf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzcyngio.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxkxqcs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2huzapqpl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gygpizoi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sstipdfn.html


<!-- 参考信息 -->