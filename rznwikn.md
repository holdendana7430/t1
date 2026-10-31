代发 wailian999

[U107] JS：数字千分位
来源：http://ki.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qb.asd995.cn

[U108] JS：随机整数
来源：http://wo.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ob.muxihuayi.cn

[U109] JS：数组分组
来源：http://lw.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://wk.gzmigu.cn

[U110] JS：数组分块
来源：http://uz.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fo.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://es.lnxyls.cn

new Map(Object.entries(obj))
来源：http://jo.szxytkj.cn

[U112] JS：字符串补位
来源：http://eu.hnjuh.cn

"7".padStart(3, "0")
来源：http://zu.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ln.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ve.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://bb.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zj.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://qr.chemitech.net.cn

crypto.randomUUID()
来源：http://am.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ur.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://gu.huixiangedu.cn

[U117] JS：单元测试
来源：http://ku.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://so.shxzskj.cn

[U118] JS：开发服务器
来源：http://ba.9csxet.cn

npm i -D vite;  npx vite
来源：http://nh.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://sl.nicolike.cn

npx vite build
来源：http://xc.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://tl.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://ec.shxzskj.cn

================================================================================
来源：http://fy.asd995.cn

统计汇总
来源：http://ep.szsharing.cn

================================================================================
来源：http://yh.szxytkj.cn

按语言统计（条）：
来源：http://sr.9csxet.cn

Python ......... 252
来源：http://eu.hnjuh.cn

PHP ............ 252
来源：http://qi.wgjwhj.cn

JavaScript ..... 252
来源：http://or.huanxung.cn

TypeScript ..... 212
来源：http://qs.bookmarksfly.cn

Java ........... 212
来源：http://wk.szsharing.cn

Go ............. 212
来源：http://yy.huanxung.cn

Ruby ........... 212
来源：http://al.huixiangedu.cn

C# ............. 212
来源：http://tf.521024.cn

C .............. 30
来源：http://je.bjjhwx.cn

C++ ............ 30
来源：http://gi.panjiajie.cn

SQL ............ 90
来源：http://yv.yuexingan06.cn

Bash ........... 80
来源：http://if.shxzskj.cn

Kotlin ......... 15
来源：http://gv.jctech888.com.cn

Swift .......... 15
来源：http://nr.shxzukj.cn

Lua ............ 10
来源：http://bh.hahajie.cn

Perl ........... 10
来源：http://gf.newstarts.cn

Scala .......... 10
来源：http://ue.huixinmuqiang.cn

------------------------------------
来源：http://fw.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://ff.521024.cn

按章节统计：
来源：http://lg.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qw.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dr.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rx.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wk.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jo.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pl.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ew.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mr.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ze.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jk.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://da.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oj.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bb.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cr.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://np.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vc.szsharing.cn

Q SQL 专题                              90
来源：http://ru.shxzukj.cn

R Bash 专题                             80
来源：http://pv.haigaiapp.cn

S C / C++ 专题                          60
来源：http://vc.hahajie.cn

T 其他语言补充                          60
来源：http://zg.chemitech.net.cn

U 高频实用片段                         120
来源：http://aq.gzmigu.cn

------------------------------------
来源：http://vw.521024.cn

合计                                  2106 条
来源：http://vh.521024.cn

--------------------------------------------------------------------------------
来源：http://tp.colortex.cn

使用提醒
来源：http://wc.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ia.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ou.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lc.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qb.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fr.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wo.nszjky.cn

—— 文件结束 ——
来源：http://tz.panjiajie.cn

================================================================================
来源：http://ep.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://fa.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://me.szsharing.cn

================================================================================
来源：http://xl.huixiangedu.cn

【收录内容】
来源：http://xo.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lu.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pg.jctech888.com.cn

SQL · Bash · C · C++
来源：http://hw.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wr.szxytkj.cn

【使用说明】
来源：http://ea.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://da.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lv.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sw.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ph.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://el.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cq.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bx.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ye.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://up.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fe.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qt.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sb.newstarts.cn

【文件统计】
来源：http://lu.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qu.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://yv.newstarts.cn

目  录
来源：http://jc.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ga.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jc.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fd.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hn.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bc.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kb.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://df.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lk.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hd.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yv.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bg.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rx.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://no.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xu.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qp.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gq.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kj.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vq.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iu.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tq.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ta.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yv.bjjhwx.cn

================================================================================
来源：http://co.yuexingan06.cn

A. 基础语法与类型
来源：http://bh.hnjuh.cn

================================================================================
来源：http://kw.nszjky.cn

[A01] Hello World
来源：http://qy.shxzskj.cn

Py:   print("Hello, World!")
来源：http://fu.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://vd.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://ua.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fu.521024.cn

Java: System.out.println("Hello, World!");
来源：http://vl.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://fu.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://rz.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fk.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://zh.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fi.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bi.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tr.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://or.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://vn.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://yh.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://px.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://db.bookmarksfly.cn

[A03] 常量定义
来源：http://of.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ne.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://ih.huanxung.cn

JS:   const PI = 3.14159;
来源：http://db.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://sn.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://gl.521024.cn

Go:   const PI = 3.14159
来源：http://kf.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://et.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://mo.muxihuayi.cn

[A04] 判断变量类型
来源：http://aa.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://el.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ez.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vn.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://aw.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://us.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wl.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://be.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://zx.shxzukj.cn

[A05] 整数除法与取模
来源：http://ay.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zl.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jo.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cs.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vs.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://lu.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://ky.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ap.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://kv.nszjky.cn

[A06] 字符串转数字
来源：http://fx.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://hx.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lw.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xy.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bx.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vg.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kb.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://md.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zo.newstarts.cn

[A07] 数字转字符串
来源：http://sv.hahajie.cn

Py:   str(42)
来源：http://da.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://lq.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://sg.szsharing.cn

TS:   String(42)
来源：http://va.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qb.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://cp.panjiajie.cn

Ruby: 42.to_s
来源：http://co.shtwfgs.cn

C#:   42.ToString()
来源：http://gn.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://ul.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zd.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ux.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zd.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yw.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://np.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ii.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pt.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vw.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://vd.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kt.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bq.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xh.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ku.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rm.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fk.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ki.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pj.jianghongdianzi.cn

[A10] 生成随机数
来源：http://lr.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://wv.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://qp.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qe.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bi.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://am.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ut.panjiajie.cn

Ruby: rand(1..100)
来源：http://dd.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://oo.colortex.cn

[A11] 条件表达式（三元）
来源：http://ze.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://xu.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ai.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hy.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://be.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ef.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wg.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ji.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ws.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://pr.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xv.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yf.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://di.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://vh.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://wm.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zk.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://of.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://cb.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vz.asd995.cn

Py:   "第一行\n第二行"
来源：http://jg.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://iq.asd995.cn

JS:   "第一行\n第二行"
来源：http://ku.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://ac.521024.cn

Java: "第一行\n第二行"
来源：http://tm.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://dq.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://wf.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://zy.panjiajie.cn

[A14] 注释写法
来源：http://pp.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ez.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eq.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://be.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://gq.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://as.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://zj.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vp.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://sn.szxytkj.cn

[A15] 空值判断与默认值
来源：http://pd.shxzukj.cn

Py:   value = data or "默认值"
来源：http://ds.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://yj.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://dy.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://mw.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sb.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://fu.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://rs.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://xi.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://ny.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pl.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://it.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rh.haigaiapp.cn

TS:   if (!x) {}
来源：http://ru.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mq.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tq.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hn.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lh.shxzukj.cn

[A17] 位运算
来源：http://pu.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://af.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gj.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://df.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wt.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sd.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xp.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://cm.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://ps.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://lm.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://li.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tr.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://wj.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://db.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://ms.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://hv.jctech888.com.cn

[A19] 交换两个变量
来源：http://ki.newstarts.cn

Py:   a, b = b, a
来源：http://bf.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vc.huanxung.cn


<!-- 参考信息 -->