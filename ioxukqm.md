代发 wailian999

[U103] JS：定时器
来源：http://af.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tp.bookmarksfly.cn

[U104] JS：防抖
来源：http://ql.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tx.huixiangedu.cn

[U105] JS：节流
来源：http://fk.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xn.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://hx.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pg.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://ne.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qv.shxzskj.cn

[U108] JS：随机整数
来源：http://oh.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oz.hahajie.cn

[U109] JS：数组分组
来源：http://vd.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://bm.nszjky.cn

[U110] JS：数组分块
来源：http://wq.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oj.nszjky.cn

[U111] JS：对象转 Map
来源：http://lc.asd995.cn

new Map(Object.entries(obj))
来源：http://ld.asd995.cn

[U112] JS：字符串补位
来源：http://da.huixiangedu.cn

"7".padStart(3, "0")
来源：http://ik.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://yr.hahajie.cn

s.replaceAll("a", "b")
来源：http://aw.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://wf.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tb.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://yw.huixinmuqiang.cn

crypto.randomUUID()
来源：http://wc.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://wi.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://gj.hahajie.cn

[U117] JS：单元测试
来源：http://qf.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://fg.huanxung.cn

[U118] JS：开发服务器
来源：http://ip.nszjky.cn

npm i -D vite;  npx vite
来源：http://iv.shtwfgs.cn

[U119] JS：生产构建
来源：http://mo.muxihuayi.cn

npx vite build
来源：http://pj.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://da.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://mb.nicolike.cn

================================================================================
来源：http://uo.yuntaijiaju.cn

统计汇总
来源：http://rl.huixinmuqiang.cn

================================================================================
来源：http://br.9csxet.cn

按语言统计（条）：
来源：http://bf.yuexingan06.cn

Python ......... 252
来源：http://hi.521024.cn

PHP ............ 252
来源：http://ic.huanxung.cn

JavaScript ..... 252
来源：http://nw.shxzskj.cn

TypeScript ..... 212
来源：http://mx.yuntaijiaju.cn

Java ........... 212
来源：http://yl.nicolike.cn

Go ............. 212
来源：http://vi.hnjuh.cn

Ruby ........... 212
来源：http://bb.nicolike.cn

C# ............. 212
来源：http://ol.shxzukj.cn

C .............. 30
来源：http://qk.chemitech.net.cn

C++ ............ 30
来源：http://gy.hnjuh.cn

SQL ............ 90
来源：http://wg.chemitech.net.cn

Bash ........... 80
来源：http://av.wgjwhj.cn

Kotlin ......... 15
来源：http://fh.bjjhwx.cn

Swift .......... 15
来源：http://dn.muxihuayi.cn

Lua ............ 10
来源：http://ag.jianghongdianzi.cn

Perl ........... 10
来源：http://nb.nszjky.cn

Scala .......... 10
来源：http://ph.gzmigu.cn

------------------------------------
来源：http://lk.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://nb.colortex.cn

按章节统计：
来源：http://xw.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mo.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cz.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bv.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xm.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nm.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://te.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uu.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vn.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uo.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oj.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yu.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gy.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pr.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lh.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ec.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jt.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://mh.newstarts.cn

R Bash 专题                             80
来源：http://fx.lnxyls.cn

S C / C++ 专题                          60
来源：http://gi.szsharing.cn

T 其他语言补充                          60
来源：http://zn.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://qj.asd995.cn

------------------------------------
来源：http://ao.chemitech.net.cn

合计                                  2106 条
来源：http://xy.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://zk.shtwfgs.cn

使用提醒
来源：http://sz.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://jb.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bl.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://li.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rb.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dz.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xq.colortex.cn

—— 文件结束 ——
来源：http://cm.huixiangedu.cn

================================================================================
来源：http://ou.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://oo.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://ad.yuexingan06.cn

================================================================================
来源：http://ua.jianghongdianzi.cn

【收录内容】
来源：http://pr.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jd.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fg.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://eo.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vj.wgjwhj.cn

【使用说明】
来源：http://rp.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ny.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qk.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://st.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://io.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kt.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zf.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://km.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vi.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xd.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dl.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wi.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mt.jianghongdianzi.cn

【文件统计】
来源：http://lq.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qi.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ad.huixiangedu.cn

目  录
来源：http://jc.colortex.cn

--------------------------------------------------------------------------------
来源：http://iq.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pb.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mc.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://el.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rc.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zd.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lm.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://co.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pt.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cd.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wm.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ht.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jl.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nj.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sg.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hn.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jj.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jf.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://js.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sj.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tq.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zo.jianghongdianzi.cn

================================================================================
来源：http://fy.lnxyls.cn

A. 基础语法与类型
来源：http://yp.haigaiapp.cn

================================================================================
来源：http://tf.nszjky.cn

[A01] Hello World
来源：http://he.szsharing.cn

Py:   print("Hello, World!")
来源：http://xc.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://fn.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://wc.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sf.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://go.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://ql.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://oi.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sl.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://dn.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yf.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ox.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ow.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ou.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://en.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://fa.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://qr.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hv.bjjhwx.cn

[A03] 常量定义
来源：http://zh.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mh.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://gd.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ie.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://gx.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ig.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://qh.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://nw.521024.cn

C#:   const double PI = 3.14159;
来源：http://xe.colortex.cn

[A04] 判断变量类型
来源：http://mf.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fu.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ac.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nl.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://rd.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vf.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mg.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ta.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://qn.szxytkj.cn

[A05] 整数除法与取模
来源：http://lb.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://it.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ue.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://va.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uk.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://ni.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://ff.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dz.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://pc.bookmarksfly.cn

[A06] 字符串转数字
来源：http://ez.asd995.cn

Py:   int("42"); float("3.14")
来源：http://pg.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://up.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xy.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yp.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ao.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pl.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://po.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ot.chemitech.net.cn

[A07] 数字转字符串
来源：http://bp.huixiangedu.cn

Py:   str(42)
来源：http://tp.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://ye.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://yc.szxytkj.cn

TS:   String(42)
来源：http://xf.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://go.colortex.cn

Go:   strconv.Itoa(42)
来源：http://li.shxzskj.cn

Ruby: 42.to_s
来源：http://am.huanxung.cn

C#:   42.ToString()
来源：http://ai.9csxet.cn

[A08] 取整与四舍五入
来源：http://dw.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vw.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://un.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dn.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wt.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nj.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cj.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ql.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xb.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://bf.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uy.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mv.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bp.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jp.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rn.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ft.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bp.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://md.bjjhwx.cn

[A10] 生成随机数
来源：http://jg.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://ip.9csxet.cn

PHP:  random_int(1, 100);
来源：http://ny.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tk.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iv.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://om.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pl.huixiangedu.cn

Ruby: rand(1..100)
来源：http://pe.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://gk.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://eq.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://qy.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ah.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pu.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jj.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://tw.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ng.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nn.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aq.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://ek.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ow.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ix.asd995.cn

JS:   `Hello, ${name}!`
来源：http://lw.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://nj.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://dh.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gq.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://hc.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://va.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://um.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://pv.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://nn.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://da.9csxet.cn

TS:   "第一行\n第二行"
来源：http://og.gzmigu.cn

Java: "第一行\n第二行"
来源：http://cp.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://go.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://fq.huanxung.cn

C#:   "第一行\n第二行"
来源：http://kt.huanxung.cn

[A14] 注释写法
来源：http://ls.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vr.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ki.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://hu.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://rx.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vw.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ta.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zg.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://ut.nicolike.cn

[A15] 空值判断与默认值
来源：http://ee.gzmigu.cn

Py:   value = data or "默认值"
来源：http://mj.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://py.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://nk.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://oz.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rl.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fr.huanxung.cn

Ruby: value = data || "默认值"
来源：http://zx.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://zp.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ra.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ll.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://km.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ef.panjiajie.cn

TS:   if (!x) {}
来源：http://gi.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vk.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jx.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zx.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nq.shtwfgs.cn

[A17] 位运算
来源：http://mm.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tg.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ov.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://um.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ol.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uk.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://is.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://du.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://hb.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://ik.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://na.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bd.newstarts.cn


<!-- 参考信息 -->