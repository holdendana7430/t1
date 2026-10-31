代发 wailian999

[U105] JS：节流
来源：http://kr.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bf.huanxung.cn

[U106] JS：日期格式化
来源：http://rr.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hq.huanxung.cn

[U107] JS：数字千分位
来源：http://on.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xh.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://zd.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://il.wgjwhj.cn

[U109] JS：数组分组
来源：http://bi.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://xm.nszjky.cn

[U110] JS：数组分块
来源：http://nz.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ok.shxzukj.cn

[U111] JS：对象转 Map
来源：http://mb.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://ew.nicolike.cn

[U112] JS：字符串补位
来源：http://th.9csxet.cn

"7".padStart(3, "0")
来源：http://yv.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://mb.shxzukj.cn

s.replaceAll("a", "b")
来源：http://qu.colortex.cn

[U114] JS：JSON 深比较
来源：http://pn.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jv.shxzukj.cn

[U115] JS：生成 UUID
来源：http://kx.bjjhwx.cn

crypto.randomUUID()
来源：http://gf.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ib.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://yj.hnjuh.cn

[U117] JS：单元测试
来源：http://xs.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://td.colortex.cn

[U118] JS：开发服务器
来源：http://hh.shxzskj.cn

npm i -D vite;  npx vite
来源：http://mj.huanxung.cn

[U119] JS：生产构建
来源：http://dm.huanxung.cn

npx vite build
来源：http://ee.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://in.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://ep.wgjwhj.cn

================================================================================
来源：http://oe.nicolike.cn

统计汇总
来源：http://xu.panjiajie.cn

================================================================================
来源：http://jg.bookmarksfly.cn

按语言统计（条）：
来源：http://qf.huixinmuqiang.cn

Python ......... 252
来源：http://xi.521024.cn

PHP ............ 252
来源：http://mi.szxytkj.cn

JavaScript ..... 252
来源：http://ra.hnjuh.cn

TypeScript ..... 212
来源：http://hk.colortex.cn

Java ........... 212
来源：http://hi.szxytkj.cn

Go ............. 212
来源：http://qk.shxzskj.cn

Ruby ........... 212
来源：http://jk.shtwfgs.cn

C# ............. 212
来源：http://cf.szsharing.cn

C .............. 30
来源：http://kf.yuntaijiaju.cn

C++ ............ 30
来源：http://nt.shtwfgs.cn

SQL ............ 90
来源：http://xa.jctech888.com.cn

Bash ........... 80
来源：http://mm.shtwfgs.cn

Kotlin ......... 15
来源：http://so.bjjhwx.cn

Swift .......... 15
来源：http://qh.colortex.cn

Lua ............ 10
来源：http://qw.yuntaijiaju.cn

Perl ........... 10
来源：http://sv.9csxet.cn

Scala .......... 10
来源：http://kt.yuntaijiaju.cn

------------------------------------
来源：http://dx.shtwfgs.cn

合计 ........... 2106 条
来源：http://tc.shxzskj.cn

按章节统计：
来源：http://sm.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fu.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://el.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ph.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uk.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ee.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://an.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yr.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zf.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ed.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tb.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qg.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bs.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sw.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vr.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zn.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jf.bjjhwx.cn

Q SQL 专题                              90
来源：http://rf.bookmarksfly.cn

R Bash 专题                             80
来源：http://lo.muxihuayi.cn

S C / C++ 专题                          60
来源：http://sf.huanxung.cn

T 其他语言补充                          60
来源：http://ha.gzmigu.cn

U 高频实用片段                         120
来源：http://fl.yuntaijiaju.cn

------------------------------------
来源：http://cp.jctech888.com.cn

合计                                  2106 条
来源：http://jg.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xx.nicolike.cn

使用提醒
来源：http://bm.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://cc.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jf.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jm.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lr.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wk.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bw.lnxyls.cn

—— 文件结束 ——
来源：http://au.newstarts.cn

================================================================================
来源：http://jt.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://mi.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://ud.asd995.cn

================================================================================
来源：http://fn.yuntaijiaju.cn

【收录内容】
来源：http://pi.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zn.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mw.shxzskj.cn

SQL · Bash · C · C++
来源：http://fp.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cf.yuntaijiaju.cn

【使用说明】
来源：http://sr.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ev.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pm.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ul.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zv.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fi.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gk.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ng.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wb.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://st.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aj.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tx.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ae.bookmarksfly.cn

【文件统计】
来源：http://ul.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rl.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://cc.9csxet.cn

目  录
来源：http://wp.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ok.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dl.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eq.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ed.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://no.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rd.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rz.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sr.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yy.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qb.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dv.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pu.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://np.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cl.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ry.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zr.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yf.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ah.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ew.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vw.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cu.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zk.nicolike.cn

================================================================================
来源：http://wg.9csxet.cn

A. 基础语法与类型
来源：http://zg.hnjuh.cn

================================================================================
来源：http://qe.szxytkj.cn

[A01] Hello World
来源：http://mg.hnjuh.cn

Py:   print("Hello, World!")
来源：http://yt.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://wl.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://fq.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qy.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://tu.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://gm.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://py.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lw.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://sk.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://am.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uu.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vp.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oc.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://ta.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://yk.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://xi.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qh.lnxyls.cn

[A03] 常量定义
来源：http://du.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qy.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://zz.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://ee.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://om.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://bf.hahajie.cn

Go:   const PI = 3.14159
来源：http://bz.szxytkj.cn

Ruby: PI = 3.14159
来源：http://zp.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://fv.bookmarksfly.cn

[A04] 判断变量类型
来源：http://pd.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bz.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xj.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uh.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://tz.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xc.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rl.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://am.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://nu.szsharing.cn

[A05] 整数除法与取模
来源：http://xy.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zt.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uq.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ot.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dd.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://vh.521024.cn

Go:   7 / 2; 7 % 2
来源：http://xu.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://wr.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://nu.9csxet.cn

[A06] 字符串转数字
来源：http://eo.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://lt.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://te.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lt.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zd.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wq.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kd.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aa.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sm.nicolike.cn

[A07] 数字转字符串
来源：http://hs.nszjky.cn

Py:   str(42)
来源：http://on.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://hr.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://ck.shxzukj.cn

TS:   String(42)
来源：http://qa.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://re.521024.cn

Go:   strconv.Itoa(42)
来源：http://ka.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://wy.szxytkj.cn

C#:   42.ToString()
来源：http://oz.lnxyls.cn

[A08] 取整与四舍五入
来源：http://jb.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://av.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sy.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tv.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tp.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xx.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ys.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hi.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://js.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ww.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://el.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://am.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mm.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ye.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xe.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gu.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://du.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dt.shxzskj.cn

[A10] 生成随机数
来源：http://dk.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://rw.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://yk.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ab.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://di.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://gc.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vs.szsharing.cn

Ruby: rand(1..100)
来源：http://bd.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://zc.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://nz.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://cr.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://es.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ij.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eg.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://dq.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uy.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gy.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://de.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://kc.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cs.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hj.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://jz.521024.cn

TS:   `Hello, ${name}!`
来源：http://jm.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://rc.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gm.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://lc.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://co.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://by.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://kc.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://wo.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://kd.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://jc.shxzskj.cn

Java: "第一行\n第二行"
来源：http://ya.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://tz.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://th.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://ek.panjiajie.cn

[A14] 注释写法
来源：http://no.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mp.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fu.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ph.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://xn.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oz.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://sd.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xh.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://ex.huanxung.cn

[A15] 空值判断与默认值
来源：http://sj.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://kb.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://or.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://yx.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://bh.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jd.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://jt.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://eb.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://mj.asd995.cn

[A16] 真假值判断规则
来源：http://mt.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rw.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ry.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fb.nicolike.cn

TS:   if (!x) {}
来源：http://kr.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dd.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bk.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rk.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oo.bookmarksfly.cn

[A17] 位运算
来源：http://ea.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ui.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ll.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nb.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xk.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qs.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dx.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dd.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://fj.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://qi.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://gf.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wt.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vh.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://eq.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eh.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ro.szxytkj.cn


<!-- 参考信息 -->