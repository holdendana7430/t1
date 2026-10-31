代发 wailian999

[U101] JS：classList 操作
来源：http://gu.521024.cn

el.classList.toggle("active")
来源：http://oz.hnjuh.cn

[U102] JS：本地存储
来源：http://lj.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bf.yuexingan06.cn

[U103] JS：定时器
来源：http://tx.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pr.nicolike.cn

[U104] JS：防抖
来源：http://uo.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zq.nszjky.cn

[U105] JS：节流
来源：http://xx.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ma.szxytkj.cn

[U106] JS：日期格式化
来源：http://gv.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xl.huanxung.cn

[U107] JS：数字千分位
来源：http://ia.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ry.wgjwhj.cn

[U108] JS：随机整数
来源：http://tm.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ve.9csxet.cn

[U109] JS：数组分组
来源：http://ax.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://uq.panjiajie.cn

[U110] JS：数组分块
来源：http://pw.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://db.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://yd.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://sm.shxzskj.cn

[U112] JS：字符串补位
来源：http://wd.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://wa.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://rw.newstarts.cn

s.replaceAll("a", "b")
来源：http://ge.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://no.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://in.szsharing.cn

[U115] JS：生成 UUID
来源：http://ja.colortex.cn

crypto.randomUUID()
来源：http://bl.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ro.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://nk.lnxyls.cn

[U117] JS：单元测试
来源：http://ir.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://xk.nszjky.cn

[U118] JS：开发服务器
来源：http://bh.hnjuh.cn

npm i -D vite;  npx vite
来源：http://bo.newstarts.cn

[U119] JS：生产构建
来源：http://zk.9csxet.cn

npx vite build
来源：http://qp.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://fq.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://fw.huanxung.cn

================================================================================
来源：http://vp.521024.cn

统计汇总
来源：http://vt.jctech888.com.cn

================================================================================
来源：http://oy.muxihuayi.cn

按语言统计（条）：
来源：http://hn.jctech888.com.cn

Python ......... 252
来源：http://jj.haigaiapp.cn

PHP ............ 252
来源：http://sr.huixinmuqiang.cn

JavaScript ..... 252
来源：http://ju.hahajie.cn

TypeScript ..... 212
来源：http://ic.bjjhwx.cn

Java ........... 212
来源：http://sl.huixiangedu.cn

Go ............. 212
来源：http://jw.hahajie.cn

Ruby ........... 212
来源：http://jy.521024.cn

C# ............. 212
来源：http://cj.shtwfgs.cn

C .............. 30
来源：http://qk.bjjhwx.cn

C++ ............ 30
来源：http://hh.nszjky.cn

SQL ............ 90
来源：http://wj.hnjuh.cn

Bash ........... 80
来源：http://rl.bjjhwx.cn

Kotlin ......... 15
来源：http://mh.shxzskj.cn

Swift .......... 15
来源：http://iw.521024.cn

Lua ............ 10
来源：http://cg.wgjwhj.cn

Perl ........... 10
来源：http://ns.muxihuayi.cn

Scala .......... 10
来源：http://ix.nicolike.cn

------------------------------------
来源：http://qe.szxytkj.cn

合计 ........... 2106 条
来源：http://bj.szxytkj.cn

按章节统计：
来源：http://ai.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fu.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hw.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mq.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://no.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://no.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lh.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://om.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lm.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yx.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hf.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gm.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fw.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tq.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wg.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ld.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ti.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://ns.panjiajie.cn

R Bash 专题                             80
来源：http://yp.shxzukj.cn

S C / C++ 专题                          60
来源：http://ez.newstarts.cn

T 其他语言补充                          60
来源：http://nq.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://ks.shxzukj.cn

------------------------------------
来源：http://cy.521024.cn

合计                                  2106 条
来源：http://xv.9csxet.cn

--------------------------------------------------------------------------------
来源：http://lu.yuntaijiaju.cn

使用提醒
来源：http://nh.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ny.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qe.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mj.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bf.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://em.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://un.jianghongdianzi.cn

—— 文件结束 ——
来源：http://cj.shxzskj.cn

================================================================================
来源：http://zs.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://xq.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://ww.shxzskj.cn

================================================================================
来源：http://by.shxzukj.cn

【收录内容】
来源：http://ow.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ll.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pr.hahajie.cn

SQL · Bash · C · C++
来源：http://di.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ix.bookmarksfly.cn

【使用说明】
来源：http://wv.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yh.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jp.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yp.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qj.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kq.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sv.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bm.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ar.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://se.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fm.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xe.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qp.bjjhwx.cn

【文件统计】
来源：http://fv.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sc.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://pt.521024.cn

目  录
来源：http://by.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://mp.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dn.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tr.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://no.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vt.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mp.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ix.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rr.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ki.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wm.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://at.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yn.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wn.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qw.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ef.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ki.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bb.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cy.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hg.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ea.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yd.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mf.9csxet.cn

================================================================================
来源：http://kn.szxytkj.cn

A. 基础语法与类型
来源：http://gf.yuexingan06.cn

================================================================================
来源：http://li.nicolike.cn

[A01] Hello World
来源：http://ih.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://vc.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://zs.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://uh.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ev.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://no.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://lj.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://dk.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eo.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://sp.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ii.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xh.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dk.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mu.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://bv.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://og.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://wa.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ck.yuexingan06.cn

[A03] 常量定义
来源：http://lg.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jc.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://lj.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://wu.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://my.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://bj.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://eu.colortex.cn

Ruby: PI = 3.14159
来源：http://dg.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ze.hahajie.cn

[A04] 判断变量类型
来源：http://nv.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vh.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ah.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yy.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://oy.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kn.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rf.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://da.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://wy.asd995.cn

[A05] 整数除法与取模
来源：http://nx.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xq.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oc.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qm.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eq.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://zc.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://ny.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://fa.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://mk.bjjhwx.cn

[A06] 字符串转数字
来源：http://fg.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://nb.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cv.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lr.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://if.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yv.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ws.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jy.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cj.asd995.cn

[A07] 数字转字符串
来源：http://eb.9csxet.cn

Py:   str(42)
来源：http://av.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://hn.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://av.nszjky.cn

TS:   String(42)
来源：http://jy.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xz.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://ed.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://zk.huixinmuqiang.cn

C#:   42.ToString()
来源：http://zm.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://us.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qu.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bm.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sh.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://il.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://it.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fj.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://oq.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zb.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://wd.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xg.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cn.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sw.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qb.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xy.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lu.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cq.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ex.521024.cn

[A10] 生成随机数
来源：http://fu.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://lt.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://nz.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fx.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wq.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://bl.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lb.nszjky.cn

Ruby: rand(1..100)
来源：http://my.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://hg.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://ym.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://ht.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hr.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sg.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://il.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ha.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bx.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tw.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lm.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://pd.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qo.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kv.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://kx.521024.cn

TS:   `Hello, ${name}!`
来源：http://el.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://oc.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mk.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://vf.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://hi.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ae.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://gm.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://mx.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://db.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://hl.nicolike.cn

Java: "第一行\n第二行"
来源：http://wy.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://wz.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://ex.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://pz.bjjhwx.cn

[A14] 注释写法
来源：http://ws.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zr.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://my.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://li.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://fi.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ym.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://ej.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zf.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://ao.lnxyls.cn

[A15] 空值判断与默认值
来源：http://ou.lnxyls.cn

Py:   value = data or "默认值"
来源：http://mo.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://jv.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://oy.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://yp.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dw.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://wn.nszjky.cn

Ruby: value = data || "默认值"
来源：http://sv.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://qp.shxzukj.cn

[A16] 真假值判断规则
来源：http://ww.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mm.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yb.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ju.nicolike.cn

TS:   if (!x) {}
来源：http://zr.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jg.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cd.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ap.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mp.huixiangedu.cn

[A17] 位运算
来源：http://be.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aw.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pw.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wh.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://md.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://if.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zk.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.jctech888.com.cn


<!-- 参考信息 -->