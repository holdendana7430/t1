代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vusheibq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nfzvhygc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3muoyzrdw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mmrozicg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kynsmvil.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jcbfckoa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dccmqajc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wuetcfhi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fzksmqnf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cnoowazq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mdoycglz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dhrijjwg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mktqazor.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ccdlknse.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lxpmqwsl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wnlemsjr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pshxdhvy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mqmawmpf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cgtpeulh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbgndb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ldmjdgys.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bgmxluml.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ghdathsh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3heubshvc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hfaibjhd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ykqndfbs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sbfpzzbx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zxbnvyzi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ptgxqhza.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vrwpznup.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3igcezwnq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwsqbhs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tkmlbdrr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aqlzwtav.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3smzojtsi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvebrcti.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qbiuwqvi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nsspnmyh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jjqoeuko.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ltgldmgn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vearldgk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lofkznzl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ezwwrkcj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gkovhcfl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kblwbwmc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3segoghgt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3sfemcbay.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3olcawnef.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ejkubijf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vosdzhns.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kkgcdhtm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ritsutil.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3aruczktk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kwzoyqmy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gbngrvsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zoyagqie.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pafvckfy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pokhamba.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3equiphkf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bqdecnhi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ghhincfp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xfoigcqa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pgqaahmx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rvvaqzee.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yquwiyxf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3unleeunh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3prvpkhnf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jvzofpyd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dfqutfyk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3znelhuqk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lgfvhayz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pdvoxnih.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vuqvgbmz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gpfzphel.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3znsjypyv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vuoyaird.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jmyzktkn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hxevcwcy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vyyjxjcl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ikugzquf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lmczkfmn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3twmygnap.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dfkkmmnx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ykxrxknp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tssvnfuj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3estadpug.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3axjmvrez.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ytyczhik.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kphaichu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qcaffvcy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jznfwibj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kfaizveg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhjovekd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vpimvyar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwiqoiev.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ueeqcwyi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wuphsoiv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yigkzovv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ifjoebjw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dnfpgqfu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mcfzatff.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nfvrdhpx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rwnssbmb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vtbkthzb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hgcklwyg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ydxsauno.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hpzsknxr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3abyvvrbz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hqrsshmi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pllvdsre.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qkzhpbhe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3erjdtuzl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ujkklugo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zmixmsve.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fboxkxic.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vqhtofib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3aiciqpkz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vzrqduby.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pknwnyma.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ibswosdu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vgitetba.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3imnnpsli.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3imwojpxw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dprtfrfz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3prlvcgkn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vyxckfix.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eyezfpps.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xgozeyfw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3omjjksvg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mqlmkmkb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3icthzypx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3trbhvyqp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gdhdaycf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yqidcfyb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nuoidhyv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ccevqoyy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3chozhhxx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vjukddcm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tktmwexr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nfhgntrl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvhexx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3upukaowu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3txtbagjt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mhqawtss.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ykjvnvuo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gktqjcnp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vghigrst.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mktndcch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kasszqoj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3muzgghaf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3jjnhwicz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqatymyk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kixgoauz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qenzmuve.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ngdznjbc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3opxipfcu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3njjdtenh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lnfrpaml.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkeaqu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hlzvablb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pqqhhjsg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ztuovwgl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hnbmhwaj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpczau.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3tcdkrakz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3iigiiauh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3emznmkqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3yvlqwhpr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ttlhakvo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hdwpgcql.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fxobuaql.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bsffgprx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zjycwgtf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3cbfdnwty.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cxeoitcr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvupxuxy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iawccxor.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3napawouf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvuamxbp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mmudpfcc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ezqgmocg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xqclmtvs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqvhpzxc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzuufdjj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgrdxgic.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mjtmtlzp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cswzmqef.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zibggihv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hrfihfds.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3srlcuugu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tokvkstg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzobix.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqycoqsb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sysbsvxs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ftidurxz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmshxbmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jehamzly.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyrkwzkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jquhaooy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3apuggsct.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jarivwwg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gtkkjigh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uqxhuqkq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3eozqvxlv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tggnwqhk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ndqrtvds.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fjigpqky.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ckivtggl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwoqqw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3otuapgyh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pvatijjo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3orjsypdy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3kskjhfnp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qxadfxmu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3olemixjk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3nctfalvk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ymixrtqv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3lchutmlk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3sgwnhitb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsmrkfyj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewxlbwep.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xjlgieek.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wktzsjfh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tgnylnib.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rcthqxtv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3whrwxkur.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qmlulgzg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3hosxicqh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mmkslhft.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3eszieqdq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zllfedfz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jesmmicw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3gqvvcjnk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pkckniul.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3brtrhnfp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3fklygxsg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3axvcskei.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yngqsjkf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pnmhbutz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dmvkheft.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mqsitsng.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xahlkwqk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3enlzpdcr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3moxeafum.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mbhhkyzm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iwzhauki.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qkqdzbby.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mngghbsh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rguqjdvi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nrgpeatf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3cdltjzua.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3eldluoca.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zvdusmte.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3nncsjnji.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvgfexl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3rvqobtpf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jzufeegz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rmiuoppv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3febencet.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3shwnrfgj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3krysbnai.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rhgjsfah.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cidqjqwv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3joaeeqrv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ppycecgc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cxrczzlt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ifxoxbqj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwzgtxk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcnwhcn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3racaatwt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3okgxacxx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bozmlkws.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tzfufkgd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cviuaibt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jstzpxcc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iucvlbum.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfsxocw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kkjehjqw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3arlngxum.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vewbagjk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3egwzdhkl.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtztecs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3sxzxkpbi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjwbcgfp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwdmsqza.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcqtekhs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3abanaknb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxxlphe.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yefkepwt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tmheucqr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lcawaexb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3htklnyzl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qnxfgjis.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nkryfaar.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ovegkuii.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3gcabemvd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jwtaxsuz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nlqkwhza.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mcllfeqi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwtxrbeq.html


<!-- 参考信息 -->