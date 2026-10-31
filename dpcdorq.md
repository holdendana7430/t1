代发 wailian999

[U105] JS：节流
来源：http://pa.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oe.bjjhwx.cn

[U106] JS：日期格式化
来源：http://iy.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jt.shtwfgs.cn

[U107] JS：数字千分位
来源：http://yp.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ew.newstarts.cn

[U108] JS：随机整数
来源：http://sq.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yg.bookmarksfly.cn

[U109] JS：数组分组
来源：http://qw.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://xi.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://aw.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tp.shxzukj.cn

[U111] JS：对象转 Map
来源：http://lb.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://bs.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://zd.bjjhwx.cn

"7".padStart(3, "0")
来源：http://lh.szsharing.cn

[U113] JS：正则替换全部
来源：http://qa.521024.cn

s.replaceAll("a", "b")
来源：http://nm.9csxet.cn

[U114] JS：JSON 深比较
来源：http://on.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ur.nszjky.cn

[U115] JS：生成 UUID
来源：http://fs.huanxung.cn

crypto.randomUUID()
来源：http://hz.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://so.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://ml.szxytkj.cn

[U117] JS：单元测试
来源：http://ya.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://hr.haigaiapp.cn

[U118] JS：开发服务器
来源：http://nn.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://xh.shtwfgs.cn

[U119] JS：生产构建
来源：http://zw.hahajie.cn

npx vite build
来源：http://jo.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://wk.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://tn.huixiangedu.cn

================================================================================
来源：http://yg.shxzukj.cn

统计汇总
来源：http://qm.bjjhwx.cn

================================================================================
来源：http://hx.haigaiapp.cn

按语言统计（条）：
来源：http://qf.szxytkj.cn

Python ......... 252
来源：http://at.panjiajie.cn

PHP ............ 252
来源：http://ec.huixiangedu.cn

JavaScript ..... 252
来源：http://yf.szxytkj.cn

TypeScript ..... 212
来源：http://nz.shxzskj.cn

Java ........... 212
来源：http://ka.colortex.cn

Go ............. 212
来源：http://hd.hnjuh.cn

Ruby ........... 212
来源：http://hc.colortex.cn

C# ............. 212
来源：http://fw.huanxung.cn

C .............. 30
来源：http://pn.haigaiapp.cn

C++ ............ 30
来源：http://uy.jianghongdianzi.cn

SQL ............ 90
来源：http://ul.521024.cn

Bash ........... 80
来源：http://ol.panjiajie.cn

Kotlin ......... 15
来源：http://rs.521024.cn

Swift .......... 15
来源：http://ig.jctech888.com.cn

Lua ............ 10
来源：http://ts.nszjky.cn

Perl ........... 10
来源：http://rv.panjiajie.cn

Scala .......... 10
来源：http://wp.9csxet.cn

------------------------------------
来源：http://me.gzmigu.cn

合计 ........... 2106 条
来源：http://kc.bookmarksfly.cn

按章节统计：
来源：http://uy.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ih.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cy.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rq.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ae.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qt.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jc.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lx.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fa.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zf.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dq.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ay.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ly.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sk.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ig.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ac.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wo.shxzukj.cn

Q SQL 专题                              90
来源：http://ra.szxytkj.cn

R Bash 专题                             80
来源：http://mg.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://jz.asd995.cn

T 其他语言补充                          60
来源：http://qo.huixiangedu.cn

U 高频实用片段                         120
来源：http://we.szsharing.cn

------------------------------------
来源：http://hz.yuexingan06.cn

合计                                  2106 条
来源：http://xb.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ud.bjjhwx.cn

使用提醒
来源：http://wz.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://cm.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qa.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://js.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rf.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gy.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ds.shtwfgs.cn

—— 文件结束 ——
来源：http://tm.lnxyls.cn

================================================================================
来源：http://md.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://te.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://hq.wgjwhj.cn

================================================================================
来源：http://ul.9csxet.cn

【收录内容】
来源：http://bn.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://em.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ay.wgjwhj.cn

SQL · Bash · C · C++
来源：http://xu.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oz.bookmarksfly.cn

【使用说明】
来源：http://xa.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hr.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ae.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vu.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xx.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ro.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fi.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qr.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gm.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fu.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xj.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vi.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://si.jctech888.com.cn

【文件统计】
来源：http://tp.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ko.szsharing.cn

--------------------------------------------------------------------------------
来源：http://gx.yuexingan06.cn

目  录
来源：http://ft.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://bz.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bz.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cx.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://li.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zm.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jf.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ij.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cd.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ud.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://my.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ae.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kc.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zg.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dc.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wo.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jj.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://og.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mq.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zg.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wk.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fp.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://td.newstarts.cn

================================================================================
来源：http://hf.colortex.cn

A. 基础语法与类型
来源：http://qs.yuexingan06.cn

================================================================================
来源：http://vm.bjjhwx.cn

[A01] Hello World
来源：http://xd.shxzskj.cn

Py:   print("Hello, World!")
来源：http://nj.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://us.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://ri.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jw.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://wo.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://gt.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://iw.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ni.hnjuh.cn

[A02] 变量声明与赋值
来源：http://ix.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wj.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fq.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zk.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://an.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://jb.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://ig.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://mb.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qw.jianghongdianzi.cn

[A03] 常量定义
来源：http://ce.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://im.colortex.cn

PHP:  const PI = 3.14159;
来源：http://jf.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://js.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://yu.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://vn.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://tp.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://zl.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://jh.bookmarksfly.cn

[A04] 判断变量类型
来源：http://jg.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qw.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hj.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jx.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://vy.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ql.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nl.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://nc.521024.cn

[A05] 整数除法与取模
来源：http://do.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qv.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kn.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://de.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ro.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://wc.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://ln.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://xo.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://dn.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://cz.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://kx.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nf.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sy.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uo.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xr.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gy.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cq.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sd.nszjky.cn

[A07] 数字转字符串
来源：http://wb.haigaiapp.cn

Py:   str(42)
来源：http://mv.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://it.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://lw.szxytkj.cn

TS:   String(42)
来源：http://ng.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hs.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ad.bjjhwx.cn

Ruby: 42.to_s
来源：http://rp.jctech888.com.cn

C#:   42.ToString()
来源：http://xg.hahajie.cn

[A08] 取整与四舍五入
来源：http://al.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vg.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://va.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ky.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nv.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uw.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ad.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ah.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jj.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://cd.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vv.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ru.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ee.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tp.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kk.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uk.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://il.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rz.nszjky.cn

[A10] 生成随机数
来源：http://sw.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://xw.colortex.cn

PHP:  random_int(1, 100);
来源：http://nz.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sa.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://om.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://rf.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hd.shxzukj.cn

Ruby: rand(1..100)
来源：http://ek.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://sx.hahajie.cn

[A11] 条件表达式（三元）
来源：http://lx.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ft.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dj.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uk.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sf.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://sm.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qq.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://md.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vb.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://uu.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lh.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rb.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ol.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://xg.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://cx.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iu.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://sr.colortex.cn

C#:   $"Hello, {name}!"
来源：http://qq.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hg.hahajie.cn

Py:   "第一行\n第二行"
来源：http://qr.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://oo.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://gk.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://si.9csxet.cn

Java: "第一行\n第二行"
来源：http://yk.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://qf.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://nq.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://ha.yuntaijiaju.cn

[A14] 注释写法
来源：http://tf.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kh.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://re.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://mi.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ds.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fg.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://ft.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ci.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ar.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://nw.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://qj.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://yd.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://mi.521024.cn

TS:   const value = data ?? "默认值";
来源：http://yj.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nz.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://nh.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://ug.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://vn.szsharing.cn

[A16] 真假值判断规则
来源：http://sm.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hy.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xx.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jl.colortex.cn

TS:   if (!x) {}
来源：http://rn.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nr.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dm.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oz.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rq.szsharing.cn

[A17] 位运算
来源：http://aa.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oh.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vb.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uc.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nr.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ag.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ek.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kx.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://vc.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://qm.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://ll.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bo.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jv.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://jf.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://la.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://qa.szxytkj.cn


<!-- 参考信息 -->