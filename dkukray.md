代发 wailian999

[U101] JS：classList 操作
来源：http://oe.lnxyls.cn

el.classList.toggle("active")
来源：http://tr.shxzskj.cn

[U102] JS：本地存储
来源：http://yx.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rn.shxzskj.cn

[U103] JS：定时器
来源：http://tq.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uy.panjiajie.cn

[U104] JS：防抖
来源：http://hb.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.yuexingan06.cn

[U105] JS：节流
来源：http://og.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tv.lnxyls.cn

[U106] JS：日期格式化
来源：http://pp.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vs.lnxyls.cn

[U107] JS：数字千分位
来源：http://fj.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ad.haigaiapp.cn

[U108] JS：随机整数
来源：http://my.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bt.lnxyls.cn

[U109] JS：数组分组
来源：http://hz.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://gu.yuexingan06.cn

[U110] JS：数组分块
来源：http://aq.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wi.lnxyls.cn

[U111] JS：对象转 Map
来源：http://he.lnxyls.cn

new Map(Object.entries(obj))
来源：http://cb.yuexingan06.cn

[U112] JS：字符串补位
来源：http://wb.bjjhwx.cn

"7".padStart(3, "0")
来源：http://mr.nicolike.cn

[U113] JS：正则替换全部
来源：http://wp.gzmigu.cn

s.replaceAll("a", "b")
来源：http://kb.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ja.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ac.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://nv.shxzukj.cn

crypto.randomUUID()
来源：http://kx.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://kq.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://mc.szsharing.cn

[U117] JS：单元测试
来源：http://cl.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://vd.wgjwhj.cn

[U118] JS：开发服务器
来源：http://mh.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://sl.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://tv.bjjhwx.cn

npx vite build
来源：http://gz.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://ad.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://xb.shxzukj.cn

================================================================================
来源：http://tx.shtwfgs.cn

统计汇总
来源：http://um.huixinmuqiang.cn

================================================================================
来源：http://ys.bjjhwx.cn

按语言统计（条）：
来源：http://yn.panjiajie.cn

Python ......... 252
来源：http://rp.lnxyls.cn

PHP ............ 252
来源：http://uf.wgjwhj.cn

JavaScript ..... 252
来源：http://yd.bookmarksfly.cn

TypeScript ..... 212
来源：http://gu.shtwfgs.cn

Java ........... 212
来源：http://se.shxzukj.cn

Go ............. 212
来源：http://qk.huixinmuqiang.cn

Ruby ........... 212
来源：http://at.shxzskj.cn

C# ............. 212
来源：http://ev.9csxet.cn

C .............. 30
来源：http://ir.wgjwhj.cn

C++ ............ 30
来源：http://wi.haigaiapp.cn

SQL ............ 90
来源：http://rv.jianghongdianzi.cn

Bash ........... 80
来源：http://jq.lnxyls.cn

Kotlin ......... 15
来源：http://uv.huixiangedu.cn

Swift .......... 15
来源：http://tm.9csxet.cn

Lua ............ 10
来源：http://cg.wgjwhj.cn

Perl ........... 10
来源：http://zf.gzmigu.cn

Scala .......... 10
来源：http://td.huixiangedu.cn

------------------------------------
来源：http://aw.lnxyls.cn

合计 ........... 2106 条
来源：http://xd.yuntaijiaju.cn

按章节统计：
来源：http://sh.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://im.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pq.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ey.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gw.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wj.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bb.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://le.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sy.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hh.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ao.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yn.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lx.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tf.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dh.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jl.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fi.shtwfgs.cn

Q SQL 专题                              90
来源：http://rt.nszjky.cn

R Bash 专题                             80
来源：http://qh.shxzskj.cn

S C / C++ 专题                          60
来源：http://ph.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://rz.yuexingan06.cn

U 高频实用片段                         120
来源：http://ej.panjiajie.cn

------------------------------------
来源：http://jc.huanxung.cn

合计                                  2106 条
来源：http://qk.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ig.szsharing.cn

使用提醒
来源：http://of.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://nz.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nk.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wq.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sl.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ew.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lr.yuexingan06.cn

—— 文件结束 ——
来源：http://mi.panjiajie.cn

================================================================================
来源：http://ea.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://yl.nszjky.cn

Common Programming Examples Cheat Book
来源：http://sr.521024.cn

================================================================================
来源：http://qy.szxytkj.cn

【收录内容】
来源：http://uu.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ig.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jh.newstarts.cn

SQL · Bash · C · C++
来源：http://mp.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vk.szsharing.cn

【使用说明】
来源：http://xl.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qu.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bi.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nq.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ki.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ul.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gn.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mp.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ak.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jz.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yz.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qi.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ro.shxzukj.cn

【文件统计】
来源：http://ox.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ma.hahajie.cn

--------------------------------------------------------------------------------
来源：http://wn.521024.cn

目  录
来源：http://qe.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://kr.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://in.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ua.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wy.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ek.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cf.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yq.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ha.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://de.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xg.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wr.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nf.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ds.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://he.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uf.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ed.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://up.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kr.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gu.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ew.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gt.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fp.shxzskj.cn

================================================================================
来源：http://px.huixinmuqiang.cn

A. 基础语法与类型
来源：http://ln.jianghongdianzi.cn

================================================================================
来源：http://kj.yuexingan06.cn

[A01] Hello World
来源：http://ng.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://uc.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://do.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://ps.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uc.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://az.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ii.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://ee.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hp.shxzukj.cn

[A02] 变量声明与赋值
来源：http://ue.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bh.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rx.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tl.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dz.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://yb.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://cl.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://nm.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://da.panjiajie.cn

[A03] 常量定义
来源：http://ks.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gi.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://ne.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://sk.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://rb.asd995.cn

Java: static final double PI = 3.14159;
来源：http://ls.szxytkj.cn

Go:   const PI = 3.14159
来源：http://dk.gzmigu.cn

Ruby: PI = 3.14159
来源：http://zw.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://tb.hahajie.cn

[A04] 判断变量类型
来源：http://ba.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pd.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ck.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zx.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://gf.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wc.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fc.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zt.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://us.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://fe.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ui.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ik.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ik.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jy.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://vn.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://bv.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://qm.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://fx.muxihuayi.cn

[A06] 字符串转数字
来源：http://es.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://ic.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ey.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fg.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sz.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yt.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://se.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qy.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rb.shxzskj.cn

[A07] 数字转字符串
来源：http://st.szsharing.cn

Py:   str(42)
来源：http://lv.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://wk.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://ef.szsharing.cn

TS:   String(42)
来源：http://zi.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ky.asd995.cn

Go:   strconv.Itoa(42)
来源：http://fl.asd995.cn

Ruby: 42.to_s
来源：http://qn.huanxung.cn

C#:   42.ToString()
来源：http://fl.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://lj.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nl.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wc.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pt.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sw.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ep.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tk.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://on.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hf.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://wd.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ax.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://da.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xn.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zx.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yv.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bn.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xh.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ar.asd995.cn

[A10] 生成随机数
来源：http://lj.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://cw.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://pn.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wv.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mh.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://cr.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jy.bjjhwx.cn

Ruby: rand(1..100)
来源：http://nn.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://wh.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://uq.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://ql.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ve.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lm.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xo.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://vs.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mq.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gp.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qi.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ut.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xp.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ku.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://oz.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://zy.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://sk.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://li.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://qr.colortex.cn

C#:   $"Hello, {name}!"
来源：http://wj.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gy.nszjky.cn

Py:   "第一行\n第二行"
来源：http://px.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://pn.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://us.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://kn.newstarts.cn

Java: "第一行\n第二行"
来源：http://cc.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://ae.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://cw.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://yp.haigaiapp.cn

[A14] 注释写法
来源：http://gl.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wg.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ad.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://rw.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://jf.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qu.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://gc.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://em.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://ra.lnxyls.cn

[A15] 空值判断与默认值
来源：http://ig.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://ds.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://cr.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://qc.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://ic.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ps.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://kc.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://jk.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://jz.shxzskj.cn

[A16] 真假值判断规则
来源：http://os.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fm.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dg.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ej.chemitech.net.cn

TS:   if (!x) {}
来源：http://id.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://an.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ux.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ed.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vl.jctech888.com.cn

[A17] 位运算
来源：http://iv.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jv.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ky.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jl.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xf.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bh.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qy.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aj.bjjhwx.cn


<!-- 参考信息 -->