代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://bs.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oi.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://yv.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ce.jctech888.com.cn

[U85] JS：可选链
来源：http://qx.521024.cn

a?.b?.c
来源：http://cj.huanxung.cn

[U86] JS：空值合并
来源：http://ht.nszjky.cn

a ?? b
来源：http://nx.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://hx.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://od.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://tv.asd995.cn

{ ...a, ...b }
来源：http://au.colortex.cn

[U89] JS：数组去重
来源：http://zu.yuexingan06.cn

[...new Set(arr)]
来源：http://ob.asd995.cn

[U90] JS：数字数组排序
来源：http://mm.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://ou.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://pe.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mv.shxzukj.cn

[U92] JS：深拷贝
来源：http://vp.shtwfgs.cn

structuredClone(obj)
来源：http://zq.chemitech.net.cn

[U93] JS：模板字符串
来源：http://pf.shxzskj.cn

`共 ${n} 条`
来源：http://rl.shxzskj.cn

[U94] JS：箭头函数
来源：http://he.shxzskj.cn

const double = x => x * 2;
来源：http://cd.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ky.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://ai.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://xm.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ol.shtwfgs.cn

[U97] JS：并发请求
来源：http://ou.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://ni.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uq.szxytkj.cn

[U99] JS：事件监听
来源：http://fk.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://sy.nszjky.cn

[U100] JS：DOM 查询
来源：http://el.nicolike.cn

document.querySelector(".item")
来源：http://uf.newstarts.cn

[U101] JS：classList 操作
来源：http://fo.chemitech.net.cn

el.classList.toggle("active")
来源：http://of.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://vt.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yb.haigaiapp.cn

[U103] JS：定时器
来源：http://qh.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lh.szxytkj.cn

[U104] JS：防抖
来源：http://zl.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vb.chemitech.net.cn

[U105] JS：节流
来源：http://cx.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ie.chemitech.net.cn

[U106] JS：日期格式化
来源：http://kx.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://js.huixiangedu.cn

[U107] JS：数字千分位
来源：http://yu.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rq.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://zg.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sp.szsharing.cn

[U109] JS：数组分组
来源：http://ma.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://ll.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://do.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jd.nicolike.cn

[U111] JS：对象转 Map
来源：http://ch.szxytkj.cn

new Map(Object.entries(obj))
来源：http://xl.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://nb.muxihuayi.cn

"7".padStart(3, "0")
来源：http://xf.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://va.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://th.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://lm.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bt.hnjuh.cn

[U115] JS：生成 UUID
来源：http://kb.newstarts.cn

crypto.randomUUID()
来源：http://mj.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://oj.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://yb.muxihuayi.cn

[U117] JS：单元测试
来源：http://ng.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://vh.huanxung.cn

[U118] JS：开发服务器
来源：http://bm.nicolike.cn

npm i -D vite;  npx vite
来源：http://bd.shxzskj.cn

[U119] JS：生产构建
来源：http://xl.szxytkj.cn

npx vite build
来源：http://je.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://lm.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://kr.huixinmuqiang.cn

================================================================================
来源：http://ue.521024.cn

统计汇总
来源：http://ts.yuntaijiaju.cn

================================================================================
来源：http://zf.shxzukj.cn

按语言统计（条）：
来源：http://ah.colortex.cn

Python ......... 252
来源：http://eq.huixinmuqiang.cn

PHP ............ 252
来源：http://zm.gzmigu.cn

JavaScript ..... 252
来源：http://ny.hnjuh.cn

TypeScript ..... 212
来源：http://po.huanxung.cn

Java ........... 212
来源：http://dy.hahajie.cn

Go ............. 212
来源：http://pr.9csxet.cn

Ruby ........... 212
来源：http://wk.shtwfgs.cn

C# ............. 212
来源：http://yp.newstarts.cn

C .............. 30
来源：http://fh.521024.cn

C++ ............ 30
来源：http://bo.panjiajie.cn

SQL ............ 90
来源：http://qv.jianghongdianzi.cn

Bash ........... 80
来源：http://gv.hahajie.cn

Kotlin ......... 15
来源：http://pi.newstarts.cn

Swift .......... 15
来源：http://xv.shxzskj.cn

Lua ............ 10
来源：http://sv.haigaiapp.cn

Perl ........... 10
来源：http://dv.newstarts.cn

Scala .......... 10
来源：http://fr.panjiajie.cn

------------------------------------
来源：http://kb.hnjuh.cn

合计 ........... 2106 条
来源：http://fj.gzmigu.cn

按章节统计：
来源：http://tb.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nd.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ps.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pe.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ee.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vl.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fy.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nl.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mf.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mq.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fw.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mo.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ch.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://le.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lh.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jl.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ht.shtwfgs.cn

Q SQL 专题                              90
来源：http://pn.bjjhwx.cn

R Bash 专题                             80
来源：http://ka.hnjuh.cn

S C / C++ 专题                          60
来源：http://jp.colortex.cn

T 其他语言补充                          60
来源：http://un.colortex.cn

U 高频实用片段                         120
来源：http://as.asd995.cn

------------------------------------
来源：http://wc.bjjhwx.cn

合计                                  2106 条
来源：http://ma.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://or.huanxung.cn

使用提醒
来源：http://es.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://jw.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ay.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://es.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rs.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fj.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ct.muxihuayi.cn

—— 文件结束 ——
来源：http://nt.chemitech.net.cn

================================================================================
来源：http://zg.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ln.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://yj.hnjuh.cn

================================================================================
来源：http://tp.shtwfgs.cn

【收录内容】
来源：http://om.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kl.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vv.shtwfgs.cn

SQL · Bash · C · C++
来源：http://tl.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mv.9csxet.cn

【使用说明】
来源：http://hw.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jy.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gn.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wf.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nh.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ay.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mf.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bj.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ue.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fr.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ku.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lr.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vl.panjiajie.cn

【文件统计】
来源：http://va.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ve.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://vk.haigaiapp.cn

目  录
来源：http://gq.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ak.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bg.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kh.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tb.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vx.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dk.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lo.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://db.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cl.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oo.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ny.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jg.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qj.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dm.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wp.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tk.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tg.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vo.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sf.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rt.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yl.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ny.9csxet.cn

================================================================================
来源：http://qa.hahajie.cn

A. 基础语法与类型
来源：http://qt.newstarts.cn

================================================================================
来源：http://tp.gzmigu.cn

[A01] Hello World
来源：http://ra.colortex.cn

Py:   print("Hello, World!")
来源：http://bw.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://eb.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://qa.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ti.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://fa.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://zx.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://ei.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jk.nicolike.cn

[A02] 变量声明与赋值
来源：http://xa.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pq.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ms.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rz.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nt.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://rz.521024.cn

Go:   name := "Alex"; age := 20
来源：http://wx.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://iu.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xn.yuntaijiaju.cn

[A03] 常量定义
来源：http://ur.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pk.colortex.cn

PHP:  const PI = 3.14159;
来源：http://bm.hahajie.cn

JS:   const PI = 3.14159;
来源：http://rs.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://gr.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://gd.newstarts.cn

Go:   const PI = 3.14159
来源：http://lh.hahajie.cn

Ruby: PI = 3.14159
来源：http://db.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://ce.hnjuh.cn

[A04] 判断变量类型
来源：http://xo.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ys.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ln.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yj.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://mk.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yk.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pr.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://si.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://id.hahajie.cn

[A05] 整数除法与取模
来源：http://sj.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ru.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qd.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dd.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ij.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://bj.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://qk.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://wg.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://zp.huixiangedu.cn

[A06] 字符串转数字
来源：http://uo.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://kv.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lz.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://im.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mp.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tl.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pl.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ja.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cv.nicolike.cn

[A07] 数字转字符串
来源：http://ig.lnxyls.cn

Py:   str(42)
来源：http://xj.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://cx.newstarts.cn

JS:   String(42); (42).toString()
来源：http://nu.yuexingan06.cn

TS:   String(42)
来源：http://ay.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ch.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://wf.bookmarksfly.cn

Ruby: 42.to_s
来源：http://ni.hahajie.cn

C#:   42.ToString()
来源：http://ee.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://et.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mn.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mb.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qa.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bo.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cz.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://az.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://el.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ea.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://qx.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rk.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yk.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jw.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yp.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://my.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sg.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ye.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zf.huixiangedu.cn

[A10] 生成随机数
来源：http://ez.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://de.521024.cn

PHP:  random_int(1, 100);
来源：http://qy.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sc.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vh.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://fj.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eb.shxzukj.cn

Ruby: rand(1..100)
来源：http://vc.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://tq.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://lz.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://dk.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://md.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://on.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kx.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://hn.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qh.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tx.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pf.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://da.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fo.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://re.asd995.cn

JS:   `Hello, ${name}!`
来源：http://yn.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://vp.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://xd.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hy.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://fv.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://nm.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cw.szsharing.cn

Py:   "第一行\n第二行"
来源：http://ve.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://fv.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://to.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://tb.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://vk.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://ta.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ld.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://qr.hahajie.cn


<!-- 参考信息 -->