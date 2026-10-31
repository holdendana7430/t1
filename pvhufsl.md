代发 wailian999

[U103] JS：定时器
来源：http://pt.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aj.haigaiapp.cn

[U104] JS：防抖
来源：http://rp.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vc.hnjuh.cn

[U105] JS：节流
来源：http://ae.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mv.huixiangedu.cn

[U106] JS：日期格式化
来源：http://ps.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zp.bjjhwx.cn

[U107] JS：数字千分位
来源：http://se.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://os.shxzukj.cn

[U108] JS：随机整数
来源：http://wa.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dd.huixiangedu.cn

[U109] JS：数组分组
来源：http://xo.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://sb.9csxet.cn

[U110] JS：数组分块
来源：http://om.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vy.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://lr.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://jp.szxytkj.cn

[U112] JS：字符串补位
来源：http://rs.shtwfgs.cn

"7".padStart(3, "0")
来源：http://qj.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://gn.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://bs.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://kh.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sb.shxzskj.cn

[U115] JS：生成 UUID
来源：http://vu.haigaiapp.cn

crypto.randomUUID()
来源：http://hv.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://rj.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://ia.colortex.cn

[U117] JS：单元测试
来源：http://rj.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://rw.hnjuh.cn

[U118] JS：开发服务器
来源：http://vf.hnjuh.cn

npm i -D vite;  npx vite
来源：http://hp.nicolike.cn

[U119] JS：生产构建
来源：http://py.bookmarksfly.cn

npx vite build
来源：http://wx.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://qq.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://fz.shtwfgs.cn

================================================================================
来源：http://cy.nszjky.cn

统计汇总
来源：http://jj.haigaiapp.cn

================================================================================
来源：http://iy.newstarts.cn

按语言统计（条）：
来源：http://gs.gzmigu.cn

Python ......... 252
来源：http://mi.szxytkj.cn

PHP ............ 252
来源：http://my.shxzukj.cn

JavaScript ..... 252
来源：http://ji.haigaiapp.cn

TypeScript ..... 212
来源：http://bo.nszjky.cn

Java ........... 212
来源：http://gu.shxzukj.cn

Go ............. 212
来源：http://di.521024.cn

Ruby ........... 212
来源：http://ty.jianghongdianzi.cn

C# ............. 212
来源：http://qb.shxzukj.cn

C .............. 30
来源：http://py.9csxet.cn

C++ ............ 30
来源：http://ug.hahajie.cn

SQL ............ 90
来源：http://lv.jctech888.com.cn

Bash ........... 80
来源：http://ex.hnjuh.cn

Kotlin ......... 15
来源：http://dt.newstarts.cn

Swift .......... 15
来源：http://hq.newstarts.cn

Lua ............ 10
来源：http://vc.9csxet.cn

Perl ........... 10
来源：http://wx.szsharing.cn

Scala .......... 10
来源：http://nu.hahajie.cn

------------------------------------
来源：http://ay.yuexingan06.cn

合计 ........... 2106 条
来源：http://gr.huixiangedu.cn

按章节统计：
来源：http://ra.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ng.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ye.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ct.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rw.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cx.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jd.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pw.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bd.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gz.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ma.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vd.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pv.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rb.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dj.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://la.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ms.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://us.bookmarksfly.cn

R Bash 专题                             80
来源：http://hi.szsharing.cn

S C / C++ 专题                          60
来源：http://sm.haigaiapp.cn

T 其他语言补充                          60
来源：http://vj.chemitech.net.cn

U 高频实用片段                         120
来源：http://fv.haigaiapp.cn

------------------------------------
来源：http://kk.9csxet.cn

合计                                  2106 条
来源：http://jc.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://di.lnxyls.cn

使用提醒
来源：http://zc.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ib.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jd.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sc.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://io.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sb.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gq.bjjhwx.cn

—— 文件结束 ——
来源：http://ey.shxzskj.cn

================================================================================
来源：http://xc.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://qq.521024.cn

Common Programming Examples Cheat Book
来源：http://mf.shxzskj.cn

================================================================================
来源：http://os.9csxet.cn

【收录内容】
来源：http://ze.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kz.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pn.panjiajie.cn

SQL · Bash · C · C++
来源：http://xx.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ph.hahajie.cn

【使用说明】
来源：http://bj.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://um.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wc.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qh.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vm.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pu.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jm.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ps.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gy.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ih.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nr.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yg.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bt.yuntaijiaju.cn

【文件统计】
来源：http://kc.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rl.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://dm.bookmarksfly.cn

目  录
来源：http://fo.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ph.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bl.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ls.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ah.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bj.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fp.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xn.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zw.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jn.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sz.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rd.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hh.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ga.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eb.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ao.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hq.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ec.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://we.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vg.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rv.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nw.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nv.colortex.cn

================================================================================
来源：http://cr.shxzskj.cn

A. 基础语法与类型
来源：http://nd.colortex.cn

================================================================================
来源：http://zo.huanxung.cn

[A01] Hello World
来源：http://cv.gzmigu.cn

Py:   print("Hello, World!")
来源：http://fu.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://xb.521024.cn

JS:   console.log("Hello, World!");
来源：http://ab.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tr.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://js.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://ao.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://xc.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zx.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ll.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yd.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xk.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dl.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uc.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://vw.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://bh.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://nn.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ah.gzmigu.cn

[A03] 常量定义
来源：http://mh.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zx.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://va.hahajie.cn

JS:   const PI = 3.14159;
来源：http://wk.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://wc.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://js.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ol.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://kk.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://iv.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://ri.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://if.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jm.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hx.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://cb.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fr.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bg.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cs.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://rf.hahajie.cn

[A05] 整数除法与取模
来源：http://cv.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jk.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ut.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ac.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rk.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://wr.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://yj.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://zs.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://ny.shxzskj.cn

[A06] 字符串转数字
来源：http://be.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://oa.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xk.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sx.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wl.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nu.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uo.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uh.asd995.cn

[A07] 数字转字符串
来源：http://mt.nszjky.cn

Py:   str(42)
来源：http://lo.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://pj.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://of.nicolike.cn

TS:   String(42)
来源：http://sv.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cp.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ex.bjjhwx.cn

Ruby: 42.to_s
来源：http://zc.szsharing.cn

C#:   42.ToString()
来源：http://oo.hahajie.cn

[A08] 取整与四舍五入
来源：http://xb.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gq.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ah.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hd.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jz.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mh.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ha.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nb.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sp.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://ho.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qk.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zl.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ay.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qp.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://og.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mu.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hh.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://du.hnjuh.cn

[A10] 生成随机数
来源：http://dt.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://dy.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://em.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yj.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hn.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://uw.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pw.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://bu.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://wz.szsharing.cn

[A11] 条件表达式（三元）
来源：http://tg.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://dy.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bj.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hp.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bz.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://ay.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oj.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sp.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pq.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://cx.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wj.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cr.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://gt.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://sg.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://ul.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xa.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://im.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://ts.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bv.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://io.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://qv.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://ti.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://le.lnxyls.cn

Java: "第一行\n第二行"
来源：http://lc.newstarts.cn

Go:   "第一行\n第二行"
来源：http://lq.colortex.cn

Ruby: "第一行\n第二行"
来源：http://nm.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://yz.lnxyls.cn

[A14] 注释写法
来源：http://kf.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gv.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fp.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://sa.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://cw.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://es.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://oa.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bm.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://tu.nszjky.cn

[A15] 空值判断与默认值
来源：http://wz.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://av.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://nm.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://gi.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://as.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ob.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://hu.hahajie.cn

Ruby: value = data || "默认值"
来源：http://ih.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://vh.szsharing.cn

[A16] 真假值判断规则
来源：http://bz.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ro.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yu.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://as.huanxung.cn

TS:   if (!x) {}
来源：http://qw.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dg.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rz.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jm.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wu.shxzskj.cn

[A17] 位运算
来源：http://eo.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vm.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rg.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kr.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://li.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vl.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://jj.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://il.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://cl.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iw.shxzukj.cn


<!-- 参考信息 -->