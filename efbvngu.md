代发 wailian999

[U107] JS：数字千分位
来源：http://sr.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ze.gzmigu.cn

[U108] JS：随机整数
来源：http://pn.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uj.shxzskj.cn

[U109] JS：数组分组
来源：http://rd.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://fa.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://oi.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gu.lnxyls.cn

[U111] JS：对象转 Map
来源：http://zi.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://xu.hnjuh.cn

[U112] JS：字符串补位
来源：http://rg.asd995.cn

"7".padStart(3, "0")
来源：http://xj.521024.cn

[U113] JS：正则替换全部
来源：http://cu.colortex.cn

s.replaceAll("a", "b")
来源：http://xo.newstarts.cn

[U114] JS：JSON 深比较
来源：http://zn.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.521024.cn

[U115] JS：生成 UUID
来源：http://wi.asd995.cn

crypto.randomUUID()
来源：http://sb.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://wd.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://zd.colortex.cn

[U117] JS：单元测试
来源：http://ve.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://uo.haigaiapp.cn

[U118] JS：开发服务器
来源：http://bp.521024.cn

npm i -D vite;  npx vite
来源：http://rl.521024.cn

[U119] JS：生产构建
来源：http://fp.huanxung.cn

npx vite build
来源：http://tm.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://in.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://fa.haigaiapp.cn

================================================================================
来源：http://aw.shxzskj.cn

统计汇总
来源：http://sa.wgjwhj.cn

================================================================================
来源：http://rw.hahajie.cn

按语言统计（条）：
来源：http://td.hnjuh.cn

Python ......... 252
来源：http://hf.9csxet.cn

PHP ............ 252
来源：http://xx.colortex.cn

JavaScript ..... 252
来源：http://kd.colortex.cn

TypeScript ..... 212
来源：http://hi.jianghongdianzi.cn

Java ........... 212
来源：http://tz.yuexingan06.cn

Go ............. 212
来源：http://wv.shxzukj.cn

Ruby ........... 212
来源：http://dv.jianghongdianzi.cn

C# ............. 212
来源：http://zl.muxihuayi.cn

C .............. 30
来源：http://wy.huanxung.cn

C++ ............ 30
来源：http://ox.yuexingan06.cn

SQL ............ 90
来源：http://rf.lnxyls.cn

Bash ........... 80
来源：http://ny.chemitech.net.cn

Kotlin ......... 15
来源：http://wm.bookmarksfly.cn

Swift .......... 15
来源：http://aq.hahajie.cn

Lua ............ 10
来源：http://rm.wgjwhj.cn

Perl ........... 10
来源：http://pw.panjiajie.cn

Scala .......... 10
来源：http://nc.yuexingan06.cn

------------------------------------
来源：http://lc.521024.cn

合计 ........... 2106 条
来源：http://qb.gzmigu.cn

按章节统计：
来源：http://dw.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ud.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nc.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kt.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tj.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pv.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vo.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ey.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tz.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rn.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jh.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vl.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qd.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ez.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vy.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ol.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lp.newstarts.cn

Q SQL 专题                              90
来源：http://mu.jianghongdianzi.cn

R Bash 专题                             80
来源：http://vc.nszjky.cn

S C / C++ 专题                          60
来源：http://zh.huanxung.cn

T 其他语言补充                          60
来源：http://xw.nicolike.cn

U 高频实用片段                         120
来源：http://oq.newstarts.cn

------------------------------------
来源：http://ls.hahajie.cn

合计                                  2106 条
来源：http://bo.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://zp.szsharing.cn

使用提醒
来源：http://jr.huanxung.cn

--------------------------------------------------------------------------------
来源：http://eq.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://li.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bb.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vp.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wx.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ek.shtwfgs.cn

—— 文件结束 ——
来源：http://if.bookmarksfly.cn

================================================================================
来源：http://gb.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://ji.521024.cn

Common Programming Examples Cheat Book
来源：http://wz.shxzskj.cn

================================================================================
来源：http://eh.gzmigu.cn

【收录内容】
来源：http://bv.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fm.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wa.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://fu.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ki.jctech888.com.cn

【使用说明】
来源：http://tw.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iz.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bk.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qe.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hd.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://az.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pe.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://po.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oz.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xr.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lx.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kj.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ih.muxihuayi.cn

【文件统计】
来源：http://iq.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wa.nszjky.cn

--------------------------------------------------------------------------------
来源：http://be.newstarts.cn

目  录
来源：http://vw.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ct.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yn.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gc.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fx.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wf.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kr.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mo.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sd.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mg.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dx.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vc.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ks.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ut.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gy.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://na.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fj.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rz.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://le.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ov.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yl.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://of.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wl.panjiajie.cn

================================================================================
来源：http://ng.hahajie.cn

A. 基础语法与类型
来源：http://hc.szxytkj.cn

================================================================================
来源：http://xa.hnjuh.cn

[A01] Hello World
来源：http://iy.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://vf.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://fx.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://jx.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tf.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://wm.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ph.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://yy.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iy.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://fy.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uf.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eb.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ss.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sc.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://qc.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://sb.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://nj.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nf.jianghongdianzi.cn

[A03] 常量定义
来源：http://tw.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yk.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://vn.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://ha.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://od.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://zv.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://zo.hnjuh.cn

Ruby: PI = 3.14159
来源：http://wt.colortex.cn

C#:   const double PI = 3.14159;
来源：http://bi.newstarts.cn

[A04] 判断变量类型
来源：http://oz.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zj.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zv.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tu.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://gm.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mq.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hx.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yq.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://nd.521024.cn

[A05] 整数除法与取模
来源：http://lw.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dh.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pu.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kk.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hm.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://pb.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://hp.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ev.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://yh.huixiangedu.cn

[A06] 字符串转数字
来源：http://sk.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://de.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nb.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vw.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yv.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wt.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jp.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rn.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ir.9csxet.cn

[A07] 数字转字符串
来源：http://pp.nicolike.cn

Py:   str(42)
来源：http://pc.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://qd.9csxet.cn

JS:   String(42); (42).toString()
来源：http://uz.lnxyls.cn

TS:   String(42)
来源：http://qr.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jm.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://yj.521024.cn

Ruby: 42.to_s
来源：http://bn.bookmarksfly.cn

C#:   42.ToString()
来源：http://pz.nszjky.cn

[A08] 取整与四舍五入
来源：http://dt.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fu.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ju.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yc.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jh.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vi.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bz.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yo.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tv.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://cz.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ep.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ah.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://td.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qp.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://en.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mw.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xk.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gy.panjiajie.cn

[A10] 生成随机数
来源：http://cz.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://jk.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://ko.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yg.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dv.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://uv.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zq.chemitech.net.cn

Ruby: rand(1..100)
来源：http://rb.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://ee.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://rn.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ta.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://if.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hr.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ia.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://hy.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cw.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lp.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ow.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://fw.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ga.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iu.521024.cn

JS:   `Hello, ${name}!`
来源：http://it.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://bd.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://do.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xx.521024.cn

Ruby: "Hello, #{name}!"
来源：http://fm.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://jj.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hl.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://zs.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://nk.szsharing.cn

JS:   "第一行\n第二行"
来源：http://lb.huanxung.cn

TS:   "第一行\n第二行"
来源：http://qc.lnxyls.cn

Java: "第一行\n第二行"
来源：http://wq.nicolike.cn

Go:   "第一行\n第二行"
来源：http://vo.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://xz.521024.cn

C#:   "第一行\n第二行"
来源：http://ad.haigaiapp.cn

[A14] 注释写法
来源：http://kg.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dr.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ns.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://hi.521024.cn

TS:   // 单行；/* 多行 */
来源：http://tc.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bb.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://tv.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ir.521024.cn

C#:   // 单行；/* 多行 */
来源：http://fv.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ey.lnxyls.cn

Py:   value = data or "默认值"
来源：http://dk.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ka.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://jy.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://jd.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ix.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://ug.9csxet.cn

Ruby: value = data || "默认值"
来源：http://cb.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://xs.gzmigu.cn

[A16] 真假值判断规则
来源：http://nl.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sx.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gz.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://so.haigaiapp.cn

TS:   if (!x) {}
来源：http://vl.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ew.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ym.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vg.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zl.shxzskj.cn

[A17] 位运算
来源：http://an.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://po.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tz.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ci.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oz.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tv.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wx.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://pn.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://st.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://el.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hh.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ya.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://vd.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ft.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://jd.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://fi.asd995.cn

[A19] 交换两个变量
来源：http://dm.muxihuayi.cn

Py:   a, b = b, a
来源：http://ng.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xx.wgjwhj.cn


<!-- 参考信息 -->