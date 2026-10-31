代发 wailian999

[U81] JS：初始化项目
来源：http://zg.jctech888.com.cn

npm init -y;  npm i express
来源：http://pp.szsharing.cn

[U82] JS：package.json 脚本
来源：http://fc.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jg.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://vh.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xr.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://sg.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jq.jianghongdianzi.cn

[U85] JS：可选链
来源：http://ls.colortex.cn

a?.b?.c
来源：http://ul.nszjky.cn

[U86] JS：空值合并
来源：http://fq.521024.cn

a ?? b
来源：http://xx.bjjhwx.cn

[U87] JS：解构默认值
来源：http://fc.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://kd.lnxyls.cn

[U88] JS：对象展开合并
来源：http://xg.huixinmuqiang.cn

{ ...a, ...b }
来源：http://dj.shxzskj.cn

[U89] JS：数组去重
来源：http://oz.shxzskj.cn

[...new Set(arr)]
来源：http://gn.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://cj.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://kd.nszjky.cn

[U91] JS：对象键值遍历
来源：http://lz.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vf.shxzskj.cn

[U92] JS：深拷贝
来源：http://re.haigaiapp.cn

structuredClone(obj)
来源：http://hk.jctech888.com.cn

[U93] JS：模板字符串
来源：http://pn.huixiangedu.cn

`共 ${n} 条`
来源：http://qf.chemitech.net.cn

[U94] JS：箭头函数
来源：http://uf.shxzskj.cn

const double = x => x * 2;
来源：http://nc.nicolike.cn

[U95] JS：Promise 包装
来源：http://gc.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://zx.521024.cn

[U96] JS：async/await 与异常
来源：http://jo.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hr.gzmigu.cn

[U97] JS：并发请求
来源：http://pn.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ck.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://en.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://do.wgjwhj.cn

[U99] JS：事件监听
来源：http://yf.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://sv.nicolike.cn

[U100] JS：DOM 查询
来源：http://tr.huixiangedu.cn

document.querySelector(".item")
来源：http://yl.huanxung.cn

[U101] JS：classList 操作
来源：http://es.newstarts.cn

el.classList.toggle("active")
来源：http://lt.asd995.cn

[U102] JS：本地存储
来源：http://bn.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fp.szsharing.cn

[U103] JS：定时器
来源：http://go.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jq.nszjky.cn

[U104] JS：防抖
来源：http://np.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cc.bjjhwx.cn

[U105] JS：节流
来源：http://qq.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zt.nszjky.cn

[U106] JS：日期格式化
来源：http://uk.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rp.gzmigu.cn

[U107] JS：数字千分位
来源：http://gv.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uo.szsharing.cn

[U108] JS：随机整数
来源：http://ty.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qq.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://pt.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://zl.huanxung.cn

[U110] JS：数组分块
来源：http://ub.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cc.shxzskj.cn

[U111] JS：对象转 Map
来源：http://fb.lnxyls.cn

new Map(Object.entries(obj))
来源：http://hf.chemitech.net.cn

[U112] JS：字符串补位
来源：http://ub.newstarts.cn

"7".padStart(3, "0")
来源：http://op.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://yv.shxzskj.cn

s.replaceAll("a", "b")
来源：http://bb.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://vh.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ta.lnxyls.cn

[U115] JS：生成 UUID
来源：http://bh.521024.cn

crypto.randomUUID()
来源：http://pw.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://jc.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://gc.bjjhwx.cn

[U117] JS：单元测试
来源：http://mt.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://un.gzmigu.cn

[U118] JS：开发服务器
来源：http://mo.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://it.shtwfgs.cn

[U119] JS：生产构建
来源：http://ot.huanxung.cn

npx vite build
来源：http://qw.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://zq.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ri.bookmarksfly.cn

================================================================================
来源：http://tm.9csxet.cn

统计汇总
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://gj.chemitech.net.cn

按语言统计（条）：
来源：http://hw.hahajie.cn

Python ......... 252
来源：http://ea.nszjky.cn

PHP ............ 252
来源：http://fj.bookmarksfly.cn

JavaScript ..... 252
来源：http://qi.lnxyls.cn

TypeScript ..... 212
来源：http://fr.bookmarksfly.cn

Java ........... 212
来源：http://ro.hahajie.cn

Go ............. 212
来源：http://nb.hahajie.cn

Ruby ........... 212
来源：http://yp.nszjky.cn

C# ............. 212
来源：http://hh.shtwfgs.cn

C .............. 30
来源：http://lu.hnjuh.cn

C++ ............ 30
来源：http://sj.shxzukj.cn

SQL ............ 90
来源：http://ir.bookmarksfly.cn

Bash ........... 80
来源：http://is.lnxyls.cn

Kotlin ......... 15
来源：http://rp.9csxet.cn

Swift .......... 15
来源：http://hh.hnjuh.cn

Lua ............ 10
来源：http://fu.asd995.cn

Perl ........... 10
来源：http://ov.nszjky.cn

Scala .......... 10
来源：http://eb.chemitech.net.cn

------------------------------------
来源：http://ao.wgjwhj.cn

合计 ........... 2106 条
来源：http://pv.nicolike.cn

按章节统计：
来源：http://fv.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://di.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sz.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://js.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zs.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jd.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://if.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tp.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ni.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rh.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gi.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bm.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sn.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://up.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kt.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hi.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bg.shtwfgs.cn

Q SQL 专题                              90
来源：http://eu.bookmarksfly.cn

R Bash 专题                             80
来源：http://kv.chemitech.net.cn

S C / C++ 专题                          60
来源：http://tn.bjjhwx.cn

T 其他语言补充                          60
来源：http://us.asd995.cn

U 高频实用片段                         120
来源：http://jo.gzmigu.cn

------------------------------------
来源：http://wp.muxihuayi.cn

合计                                  2106 条
来源：http://oe.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://of.wgjwhj.cn

使用提醒
来源：http://kv.colortex.cn

--------------------------------------------------------------------------------
来源：http://hh.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://az.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xi.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iz.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vg.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bo.nicolike.cn

—— 文件结束 ——
来源：http://qw.nszjky.cn

================================================================================
来源：http://vw.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://xz.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://lu.jianghongdianzi.cn

================================================================================
来源：http://yt.huixinmuqiang.cn

【收录内容】
来源：http://nt.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bj.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fe.szsharing.cn

SQL · Bash · C · C++
来源：http://ce.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mw.muxihuayi.cn

【使用说明】
来源：http://gp.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rb.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nj.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bf.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rx.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ya.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nj.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qj.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rb.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ft.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sv.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cf.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sh.gzmigu.cn

【文件统计】
来源：http://tc.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sn.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://al.shtwfgs.cn

目  录
来源：http://ma.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://bx.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vz.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ot.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://se.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://th.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wg.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lz.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cl.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dy.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hp.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fj.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ba.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fh.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yc.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lo.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pd.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://se.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hv.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hj.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nm.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ct.shxzskj.cn

================================================================================
来源：http://ea.chemitech.net.cn

A. 基础语法与类型
来源：http://mt.chemitech.net.cn

================================================================================
来源：http://mt.hahajie.cn

[A01] Hello World
来源：http://ys.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://vl.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://bl.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://lt.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ch.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://al.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://gk.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://km.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hr.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://vp.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kl.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dk.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ah.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rb.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://ur.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://ta.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://ih.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nq.huanxung.cn

[A03] 常量定义
来源：http://vi.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eu.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://qj.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://dz.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://ht.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://nv.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://ja.colortex.cn

Ruby: PI = 3.14159
来源：http://lm.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://dc.nicolike.cn

[A04] 判断变量类型
来源：http://ge.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ih.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zq.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rz.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ro.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ct.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cu.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://so.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://mo.huixiangedu.cn

[A05] 整数除法与取模
来源：http://em.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ru.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mb.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://od.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bi.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://oa.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://jo.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://xp.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://ub.szxytkj.cn

[A06] 字符串转数字
来源：http://lw.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://jm.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ao.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ip.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yn.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ad.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wo.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fl.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://be.haigaiapp.cn

[A07] 数字转字符串
来源：http://hf.wgjwhj.cn

Py:   str(42)
来源：http://ao.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://jo.huanxung.cn

JS:   String(42); (42).toString()
来源：http://tn.yuntaijiaju.cn

TS:   String(42)
来源：http://hb.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kk.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://gg.szxytkj.cn

Ruby: 42.to_s
来源：http://iz.newstarts.cn

C#:   42.ToString()
来源：http://fc.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://zg.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://au.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rg.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hr.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pv.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qe.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ks.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sa.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kb.colortex.cn

[A09] 绝对值与最大最小值
来源：http://ux.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vg.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bf.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oz.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jc.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bt.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://we.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eq.bjjhwx.cn

[A10] 生成随机数
来源：http://qt.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://of.nszjky.cn

PHP:  random_int(1, 100);
来源：http://da.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ce.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ie.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://is.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vb.szxytkj.cn

Ruby: rand(1..100)
来源：http://gl.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://yt.szsharing.cn

[A11] 条件表达式（三元）
来源：http://ok.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://fd.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qm.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eb.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lv.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://wl.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bb.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nu.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zs.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://xa.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vf.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ch.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://ij.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ys.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://cf.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xi.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://fs.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://in.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://in.nicolike.cn

Py:   "第一行\n第二行"
来源：http://dc.colortex.cn

PHP:  "第一行\n第二行"
来源：http://ae.521024.cn

JS:   "第一行\n第二行"
来源：http://mq.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://ft.9csxet.cn


<!-- 参考信息 -->