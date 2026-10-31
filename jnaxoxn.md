代发 wailian999

[U105] JS：节流
来源：http://pr.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ko.nszjky.cn

[U106] JS：日期格式化
来源：http://vc.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oz.yuexingan06.cn

[U107] JS：数字千分位
来源：http://ap.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ae.asd995.cn

[U108] JS：随机整数
来源：http://sw.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tz.huanxung.cn

[U109] JS：数组分组
来源：http://mh.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://rx.hahajie.cn

[U110] JS：数组分块
来源：http://ff.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ix.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://qg.gzmigu.cn

new Map(Object.entries(obj))
来源：http://qf.haigaiapp.cn

[U112] JS：字符串补位
来源：http://wz.haigaiapp.cn

"7".padStart(3, "0")
来源：http://dn.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://ed.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://gr.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://jz.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dm.gzmigu.cn

[U115] JS：生成 UUID
来源：http://wh.shtwfgs.cn

crypto.randomUUID()
来源：http://ev.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://fg.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://vk.shtwfgs.cn

[U117] JS：单元测试
来源：http://jp.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://bn.panjiajie.cn

[U118] JS：开发服务器
来源：http://uc.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://ej.9csxet.cn

[U119] JS：生产构建
来源：http://cj.lnxyls.cn

npx vite build
来源：http://tt.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://oq.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://rd.huixiangedu.cn

================================================================================
来源：http://mr.shtwfgs.cn

统计汇总
来源：http://uo.shtwfgs.cn

================================================================================
来源：http://ba.huanxung.cn

按语言统计（条）：
来源：http://wn.shtwfgs.cn

Python ......... 252
来源：http://ga.szxytkj.cn

PHP ............ 252
来源：http://jt.shxzskj.cn

JavaScript ..... 252
来源：http://fz.panjiajie.cn

TypeScript ..... 212
来源：http://wa.shtwfgs.cn

Java ........... 212
来源：http://lt.shxzskj.cn

Go ............. 212
来源：http://og.bookmarksfly.cn

Ruby ........... 212
来源：http://zr.shtwfgs.cn

C# ............. 212
来源：http://te.shtwfgs.cn

C .............. 30
来源：http://cp.huixiangedu.cn

C++ ............ 30
来源：http://ov.szxytkj.cn

SQL ............ 90
来源：http://dj.nicolike.cn

Bash ........... 80
来源：http://pu.shtwfgs.cn

Kotlin ......... 15
来源：http://tb.9csxet.cn

Swift .......... 15
来源：http://nb.shtwfgs.cn

Lua ............ 10
来源：http://us.hnjuh.cn

Perl ........... 10
来源：http://fh.szsharing.cn

Scala .......... 10
来源：http://up.nicolike.cn

------------------------------------
来源：http://oc.bjjhwx.cn

合计 ........... 2106 条
来源：http://pk.colortex.cn

按章节统计：
来源：http://ty.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ir.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pf.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iu.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oe.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sf.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ca.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jz.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lo.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wb.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wh.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bi.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kq.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ux.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iw.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://le.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tf.bjjhwx.cn

Q SQL 专题                              90
来源：http://cz.haigaiapp.cn

R Bash 专题                             80
来源：http://fw.shxzskj.cn

S C / C++ 专题                          60
来源：http://ah.bjjhwx.cn

T 其他语言补充                          60
来源：http://ld.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://hf.shxzukj.cn

------------------------------------
来源：http://rv.hahajie.cn

合计                                  2106 条
来源：http://rj.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://hw.szsharing.cn

使用提醒
来源：http://dw.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://bc.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nk.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qg.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ak.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fp.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ib.nszjky.cn

—— 文件结束 ——
来源：http://xi.gzmigu.cn

================================================================================
来源：http://um.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://lq.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://gd.wgjwhj.cn

================================================================================
来源：http://qo.panjiajie.cn

【收录内容】
来源：http://lx.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rs.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://an.panjiajie.cn

SQL · Bash · C · C++
来源：http://qh.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hu.colortex.cn

【使用说明】
来源：http://pa.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qx.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://io.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ci.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ba.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://na.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ok.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hf.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hf.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sj.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://px.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://km.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://un.huanxung.cn

【文件统计】
来源：http://ua.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oq.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://dp.yuntaijiaju.cn

目  录
来源：http://oe.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://bv.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wb.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ks.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zv.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pf.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qu.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bq.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lh.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uq.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cz.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yf.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dm.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wv.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://st.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://km.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gc.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nv.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eg.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fn.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ze.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dy.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bs.newstarts.cn

================================================================================
来源：http://nf.jianghongdianzi.cn

A. 基础语法与类型
来源：http://nn.huixiangedu.cn

================================================================================
来源：http://sj.huanxung.cn

[A01] Hello World
来源：http://xg.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://po.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://qj.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://gs.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sa.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://je.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://di.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://ll.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zi.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ck.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hj.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xe.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sd.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xe.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://lm.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://to.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://wf.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nh.shxzukj.cn

[A03] 常量定义
来源：http://ks.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jv.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://as.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://ku.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://lm.521024.cn

Java: static final double PI = 3.14159;
来源：http://dv.newstarts.cn

Go:   const PI = 3.14159
来源：http://mk.panjiajie.cn

Ruby: PI = 3.14159
来源：http://yk.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://jl.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://dj.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sc.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qv.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mf.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://kk.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fq.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pk.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://in.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://or.yuexingan06.cn

[A05] 整数除法与取模
来源：http://la.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ks.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gu.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wh.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xb.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://lc.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://wk.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://gp.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://yd.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://xv.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://mk.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mn.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fh.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xx.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pr.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gp.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sr.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qz.newstarts.cn

[A07] 数字转字符串
来源：http://tm.gzmigu.cn

Py:   str(42)
来源：http://bo.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://gz.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://ig.wgjwhj.cn

TS:   String(42)
来源：http://cs.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ui.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://ql.9csxet.cn

Ruby: 42.to_s
来源：http://hr.yuntaijiaju.cn

C#:   42.ToString()
来源：http://kb.nicolike.cn

[A08] 取整与四舍五入
来源：http://ar.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ic.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wp.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qr.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ip.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xh.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aa.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://aw.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lh.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://tr.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uh.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dl.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jj.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pf.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bd.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rp.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sy.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ns.haigaiapp.cn

[A10] 生成随机数
来源：http://rr.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://th.521024.cn

PHP:  random_int(1, 100);
来源：http://ah.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ba.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rb.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://ob.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iw.9csxet.cn

Ruby: rand(1..100)
来源：http://pm.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://ps.nicolike.cn

[A11] 条件表达式（三元）
来源：http://ac.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://gy.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sl.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sd.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xk.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yj.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ad.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ft.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uo.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://qe.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://if.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://id.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://bo.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://hf.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://ai.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wz.521024.cn

Ruby: "Hello, #{name}!"
来源：http://vj.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://uc.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hl.szsharing.cn

Py:   "第一行\n第二行"
来源：http://rc.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://le.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://xv.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://ty.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ud.hahajie.cn

Go:   "第一行\n第二行"
来源：http://lt.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://cu.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://pr.9csxet.cn

[A14] 注释写法
来源：http://ri.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://li.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://du.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://yi.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://zx.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cd.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://bo.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ws.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://zz.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://ym.szxytkj.cn

Py:   value = data or "默认值"
来源：http://ld.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://vs.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://ev.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://be.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wh.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://pa.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://ll.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://hc.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://kb.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ot.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ak.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ms.521024.cn

TS:   if (!x) {}
来源：http://xw.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tu.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vw.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jq.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yuexingan06.cn

[A17] 位运算
来源：http://po.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://in.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://js.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vr.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ku.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xx.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ta.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ck.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://bd.521024.cn

Py:   ord("A"); chr(65)
来源：http://ll.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://on.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://it.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://js.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://ar.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dh.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://xr.jctech888.com.cn


<!-- 参考信息 -->