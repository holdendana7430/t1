代发 wailian999

[U95] JS：Promise 包装
来源：http://fy.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://gi.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://kb.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ix.yuexingan06.cn

[U97] JS：并发请求
来源：http://wf.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ug.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://mp.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zk.9csxet.cn

[U99] JS：事件监听
来源：http://vk.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vy.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://da.jianghongdianzi.cn

document.querySelector(".item")
来源：http://gn.chemitech.net.cn

[U101] JS：classList 操作
来源：http://nr.newstarts.cn

el.classList.toggle("active")
来源：http://in.colortex.cn

[U102] JS：本地存储
来源：http://wq.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qb.asd995.cn

[U103] JS：定时器
来源：http://xy.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gk.jctech888.com.cn

[U104] JS：防抖
来源：http://nn.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nb.newstarts.cn

[U105] JS：节流
来源：http://ex.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fb.newstarts.cn

[U106] JS：日期格式化
来源：http://gj.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pn.huanxung.cn

[U107] JS：数字千分位
来源：http://hr.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gv.9csxet.cn

[U108] JS：随机整数
来源：http://oy.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cr.hnjuh.cn

[U109] JS：数组分组
来源：http://vr.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://nn.huanxung.cn

[U110] JS：数组分块
来源：http://bc.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ks.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://qi.nicolike.cn

new Map(Object.entries(obj))
来源：http://fj.gzmigu.cn

[U112] JS：字符串补位
来源：http://ol.hnjuh.cn

"7".padStart(3, "0")
来源：http://fj.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://xp.hnjuh.cn

s.replaceAll("a", "b")
来源：http://kz.asd995.cn

[U114] JS：JSON 深比较
来源：http://zi.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lz.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://pk.colortex.cn

crypto.randomUUID()
来源：http://im.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://ox.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://bm.shxzskj.cn

[U117] JS：单元测试
来源：http://ii.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://su.hahajie.cn

[U118] JS：开发服务器
来源：http://zs.colortex.cn

npm i -D vite;  npx vite
来源：http://jz.nicolike.cn

[U119] JS：生产构建
来源：http://cm.panjiajie.cn

npx vite build
来源：http://bl.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://jj.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://tx.bookmarksfly.cn

================================================================================
来源：http://kz.huixinmuqiang.cn

统计汇总
来源：http://hv.jctech888.com.cn

================================================================================
来源：http://ro.lnxyls.cn

按语言统计（条）：
来源：http://je.shtwfgs.cn

Python ......... 252
来源：http://cj.lnxyls.cn

PHP ............ 252
来源：http://rv.huixinmuqiang.cn

JavaScript ..... 252
来源：http://rz.nicolike.cn

TypeScript ..... 212
来源：http://xv.shtwfgs.cn

Java ........... 212
来源：http://yp.jctech888.com.cn

Go ............. 212
来源：http://hl.huixinmuqiang.cn

Ruby ........... 212
来源：http://am.gzmigu.cn

C# ............. 212
来源：http://zr.gzmigu.cn

C .............. 30
来源：http://jw.huanxung.cn

C++ ............ 30
来源：http://tg.wgjwhj.cn

SQL ............ 90
来源：http://gu.nicolike.cn

Bash ........... 80
来源：http://dk.colortex.cn

Kotlin ......... 15
来源：http://bw.jctech888.com.cn

Swift .......... 15
来源：http://ak.shxzukj.cn

Lua ............ 10
来源：http://qj.wgjwhj.cn

Perl ........... 10
来源：http://lq.521024.cn

Scala .......... 10
来源：http://lr.shxzukj.cn

------------------------------------
来源：http://kl.hahajie.cn

合计 ........... 2106 条
来源：http://tk.gzmigu.cn

按章节统计：
来源：http://ql.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vi.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zw.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dc.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gf.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tm.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dp.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sg.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cs.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rv.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://up.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://on.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://if.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://he.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aa.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sz.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zc.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://ur.jianghongdianzi.cn

R Bash 专题                             80
来源：http://kq.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://xz.521024.cn

T 其他语言补充                          60
来源：http://ht.szsharing.cn

U 高频实用片段                         120
来源：http://pm.nicolike.cn

------------------------------------
来源：http://nt.9csxet.cn

合计                                  2106 条
来源：http://gb.521024.cn

--------------------------------------------------------------------------------
来源：http://ap.9csxet.cn

使用提醒
来源：http://qb.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://fo.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vw.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bm.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://up.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fg.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sm.shxzskj.cn

—— 文件结束 ——
来源：http://nb.hahajie.cn

================================================================================
来源：http://zk.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://nt.nicolike.cn

Common Programming Examples Cheat Book
来源：http://ew.shtwfgs.cn

================================================================================
来源：http://mh.szxytkj.cn

【收录内容】
来源：http://vv.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zk.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qn.szsharing.cn

SQL · Bash · C · C++
来源：http://gk.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tn.hnjuh.cn

【使用说明】
来源：http://ro.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ag.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ey.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://df.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vh.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pu.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tr.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lx.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gw.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tk.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://my.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fu.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yb.huanxung.cn

【文件统计】
来源：http://ec.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://if.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://hv.lnxyls.cn

目  录
来源：http://wu.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://hj.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ff.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mc.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ot.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zo.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://et.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rz.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sy.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vf.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vk.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vx.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ke.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ff.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fa.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ib.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jl.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fj.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cy.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wo.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lh.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jj.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iy.gzmigu.cn

================================================================================
来源：http://ym.jctech888.com.cn

A. 基础语法与类型
来源：http://zq.chemitech.net.cn

================================================================================
来源：http://bu.panjiajie.cn

[A01] Hello World
来源：http://tr.gzmigu.cn

Py:   print("Hello, World!")
来源：http://hd.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://dr.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://du.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ei.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://at.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://fq.asd995.cn

Ruby: puts "Hello, World!"
来源：http://wk.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qd.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://mq.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kx.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qq.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gc.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xa.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://vy.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://du.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://go.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hq.szxytkj.cn

[A03] 常量定义
来源：http://pp.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cp.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://hs.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://qh.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://tw.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://xo.9csxet.cn

Go:   const PI = 3.14159
来源：http://io.nicolike.cn

Ruby: PI = 3.14159
来源：http://ua.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://wh.huixiangedu.cn

[A04] 判断变量类型
来源：http://of.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aq.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://us.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gn.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://jr.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mc.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fj.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cl.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://kq.panjiajie.cn

[A05] 整数除法与取模
来源：http://bq.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eb.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mj.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mw.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ey.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://df.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://jx.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://oz.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://yo.nicolike.cn

[A06] 字符串转数字
来源：http://po.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://vd.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ws.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sk.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oy.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fw.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ic.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vq.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ej.9csxet.cn

[A07] 数字转字符串
来源：http://ij.yuexingan06.cn

Py:   str(42)
来源：http://co.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://ba.asd995.cn

JS:   String(42); (42).toString()
来源：http://ur.shtwfgs.cn

TS:   String(42)
来源：http://cq.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xo.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://sx.lnxyls.cn

Ruby: 42.to_s
来源：http://rb.muxihuayi.cn

C#:   42.ToString()
来源：http://fz.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://dj.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lv.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ra.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lr.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oe.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gt.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vq.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://az.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ol.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://er.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dx.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lc.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yx.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cs.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ar.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ob.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gd.bjjhwx.cn

[A10] 生成随机数
来源：http://dt.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ac.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://al.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xz.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zi.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://kx.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wc.huanxung.cn

Ruby: rand(1..100)
来源：http://hu.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://yc.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://eq.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ms.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://im.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dy.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ve.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://ds.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ir.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sn.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ub.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://jd.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gf.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dz.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://zd.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://py.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://gg.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fh.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://cn.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://fs.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fh.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://od.asd995.cn

PHP:  "第一行\n第二行"
来源：http://yb.colortex.cn

JS:   "第一行\n第二行"
来源：http://ku.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://pk.szxytkj.cn

Java: "第一行\n第二行"
来源：http://lt.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://xf.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://ds.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://bg.wgjwhj.cn

[A14] 注释写法
来源：http://kg.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ul.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tu.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://rr.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://le.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jj.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://bu.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fa.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://cn.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://at.nszjky.cn

Py:   value = data or "默认值"
来源：http://tk.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://vf.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://pm.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://jp.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ga.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://oj.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://uh.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ny.huanxung.cn

[A16] 真假值判断规则
来源：http://ui.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jd.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yb.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pj.colortex.cn

TS:   if (!x) {}
来源：http://uz.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tz.newstarts.cn


<!-- 参考信息 -->