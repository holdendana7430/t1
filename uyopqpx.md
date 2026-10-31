代发 wailian999

[U105] JS：节流
来源：http://cl.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jk.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://nt.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mw.wgjwhj.cn

[U107] JS：数字千分位
来源：http://dt.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://om.bjjhwx.cn

[U108] JS：随机整数
来源：http://qp.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ec.shxzskj.cn

[U109] JS：数组分组
来源：http://pl.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://wi.huanxung.cn

[U110] JS：数组分块
来源：http://rz.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hu.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://nh.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://sl.szsharing.cn

[U112] JS：字符串补位
来源：http://sd.bjjhwx.cn

"7".padStart(3, "0")
来源：http://au.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://zm.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://mo.hahajie.cn

[U114] JS：JSON 深比较
来源：http://fh.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ro.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://ny.chemitech.net.cn

crypto.randomUUID()
来源：http://rw.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://sr.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://uv.huanxung.cn

[U117] JS：单元测试
来源：http://qy.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://uo.panjiajie.cn

[U118] JS：开发服务器
来源：http://gs.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://vf.haigaiapp.cn

[U119] JS：生产构建
来源：http://bp.wgjwhj.cn

npx vite build
来源：http://bo.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://bb.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://jd.huixinmuqiang.cn

================================================================================
来源：http://ym.521024.cn

统计汇总
来源：http://ax.newstarts.cn

================================================================================
来源：http://sv.gzmigu.cn

按语言统计（条）：
来源：http://sd.nicolike.cn

Python ......... 252
来源：http://so.nicolike.cn

PHP ............ 252
来源：http://ih.colortex.cn

JavaScript ..... 252
来源：http://ta.nszjky.cn

TypeScript ..... 212
来源：http://ez.gzmigu.cn

Java ........... 212
来源：http://wy.521024.cn

Go ............. 212
来源：http://ck.jctech888.com.cn

Ruby ........... 212
来源：http://gq.jctech888.com.cn

C# ............. 212
来源：http://bu.szsharing.cn

C .............. 30
来源：http://ll.521024.cn

C++ ............ 30
来源：http://hh.wgjwhj.cn

SQL ............ 90
来源：http://qu.szsharing.cn

Bash ........... 80
来源：http://rq.gzmigu.cn

Kotlin ......... 15
来源：http://dm.shxzskj.cn

Swift .......... 15
来源：http://ol.521024.cn

Lua ............ 10
来源：http://lm.jctech888.com.cn

Perl ........... 10
来源：http://ct.huanxung.cn

Scala .......... 10
来源：http://hk.jianghongdianzi.cn

------------------------------------
来源：http://fx.shtwfgs.cn

合计 ........... 2106 条
来源：http://vf.bookmarksfly.cn

按章节统计：
来源：http://hd.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cd.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uq.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ej.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://we.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ty.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yx.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fx.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uu.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yf.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lv.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lu.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nc.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ob.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ip.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ej.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xg.szsharing.cn

Q SQL 专题                              90
来源：http://mz.huixinmuqiang.cn

R Bash 专题                             80
来源：http://zy.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://mr.muxihuayi.cn

T 其他语言补充                          60
来源：http://ha.jctech888.com.cn

U 高频实用片段                         120
来源：http://qo.bjjhwx.cn

------------------------------------
来源：http://bf.bookmarksfly.cn

合计                                  2106 条
来源：http://jg.huanxung.cn

--------------------------------------------------------------------------------
来源：http://mt.9csxet.cn

使用提醒
来源：http://fp.asd995.cn

--------------------------------------------------------------------------------
来源：http://vg.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mf.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mg.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ow.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cm.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://av.shxzukj.cn

—— 文件结束 ——
来源：http://lv.bookmarksfly.cn

================================================================================
来源：http://yi.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://vn.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://ih.521024.cn

================================================================================
来源：http://wh.huixiangedu.cn

【收录内容】
来源：http://ph.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uo.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ac.wgjwhj.cn

SQL · Bash · C · C++
来源：http://lq.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xb.shtwfgs.cn

【使用说明】
来源：http://rr.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oa.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fk.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ni.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gm.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rz.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ml.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ce.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sb.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iw.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wd.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zi.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ah.hahajie.cn

【文件统计】
来源：http://pc.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fp.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://xc.asd995.cn

目  录
来源：http://ph.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qp.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pz.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gk.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tj.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://un.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kd.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fy.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bz.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ai.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bg.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xd.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hj.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sa.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jp.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lx.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mb.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nq.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gn.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hp.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nt.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gg.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hd.szsharing.cn

================================================================================
来源：http://cj.shxzskj.cn

A. 基础语法与类型
来源：http://rk.asd995.cn

================================================================================
来源：http://vz.panjiajie.cn

[A01] Hello World
来源：http://aq.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://xf.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://yn.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://cp.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cm.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://ba.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://xk.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://uj.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gt.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ho.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sj.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ih.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iy.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qc.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://zs.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ib.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://ke.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gh.nicolike.cn

[A03] 常量定义
来源：http://io.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dz.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://sz.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://dn.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://vf.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://iv.asd995.cn

Go:   const PI = 3.14159
来源：http://lw.shxzskj.cn

Ruby: PI = 3.14159
来源：http://hq.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://qd.muxihuayi.cn

[A04] 判断变量类型
来源：http://qu.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yh.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yk.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gb.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ka.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tt.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fd.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cr.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://bs.asd995.cn

[A05] 整数除法与取模
来源：http://yt.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kp.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zv.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kp.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dd.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://ll.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://yz.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://nz.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://pj.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ex.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://dq.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://es.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iw.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bv.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xd.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fj.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://my.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yf.szsharing.cn

[A07] 数字转字符串
来源：http://ym.colortex.cn

Py:   str(42)
来源：http://vx.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://eb.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://or.bjjhwx.cn

TS:   String(42)
来源：http://vv.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gm.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://bh.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://nt.huixinmuqiang.cn

C#:   42.ToString()
来源：http://mp.521024.cn

[A08] 取整与四舍五入
来源：http://kg.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dy.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bo.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ri.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gt.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ui.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://az.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vu.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ys.asd995.cn

[A09] 绝对值与最大最小值
来源：http://tq.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zt.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kp.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cx.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wg.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rm.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ys.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zw.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nn.szsharing.cn

[A10] 生成随机数
来源：http://jf.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://sc.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://rp.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://br.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pc.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://fr.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jh.shxzukj.cn

Ruby: rand(1..100)
来源：http://xd.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://ch.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://xh.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://xt.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://po.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dz.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hd.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://mw.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kp.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://by.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ez.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://nm.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mt.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hj.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://bn.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://ef.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://hh.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gj.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://ld.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ce.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sf.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://px.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://oi.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://cd.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://db.hahajie.cn

Java: "第一行\n第二行"
来源：http://ze.colortex.cn

Go:   "第一行\n第二行"
来源：http://ya.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://ci.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://de.szsharing.cn

[A14] 注释写法
来源：http://gs.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jz.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wm.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://oq.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://xs.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wx.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://ty.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lm.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://wu.huanxung.cn

[A15] 空值判断与默认值
来源：http://yq.shxzukj.cn

Py:   value = data or "默认值"
来源：http://cq.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://qx.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://yj.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://zk.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nn.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://qw.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://fe.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://us.panjiajie.cn

[A16] 真假值判断规则
来源：http://qa.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uo.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ws.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sl.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://sx.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ak.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tr.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://or.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nz.shtwfgs.cn

[A17] 位运算
来源：http://dv.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://le.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dp.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rs.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yh.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ds.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bg.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wl.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://rs.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://ow.521024.cn

PHP:  ord("A"); chr(65)
来源：http://uo.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zx.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ub.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://ac.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qv.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://wb.shtwfgs.cn


<!-- 参考信息 -->