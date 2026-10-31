代发 wailian999

[U105] JS：节流
来源：http://qk.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sf.nszjky.cn

[U106] JS：日期格式化
来源：http://xc.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sm.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://oi.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gl.huanxung.cn

[U108] JS：随机整数
来源：http://ut.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://od.nicolike.cn

[U109] JS：数组分组
来源：http://fp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://io.521024.cn

[U110] JS：数组分块
来源：http://zg.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wc.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://pc.shxzukj.cn

new Map(Object.entries(obj))
来源：http://ve.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://le.lnxyls.cn

"7".padStart(3, "0")
来源：http://oi.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://cp.shxzskj.cn

s.replaceAll("a", "b")
来源：http://au.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://bb.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yb.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://re.shtwfgs.cn

crypto.randomUUID()
来源：http://lu.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://xl.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://zr.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://iy.521024.cn

npm i -D vitest;  npx vitest
来源：http://lz.huanxung.cn

[U118] JS：开发服务器
来源：http://pu.shxzukj.cn

npm i -D vite;  npx vite
来源：http://vh.lnxyls.cn

[U119] JS：生产构建
来源：http://xg.szxytkj.cn

npx vite build
来源：http://yw.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://zq.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://ea.muxihuayi.cn

================================================================================
来源：http://uy.hnjuh.cn

统计汇总
来源：http://zx.yuntaijiaju.cn

================================================================================
来源：http://jx.huixiangedu.cn

按语言统计（条）：
来源：http://fa.lnxyls.cn

Python ......... 252
来源：http://hb.panjiajie.cn

PHP ............ 252
来源：http://po.yuexingan06.cn

JavaScript ..... 252
来源：http://ap.newstarts.cn

TypeScript ..... 212
来源：http://yd.shxzukj.cn

Java ........... 212
来源：http://de.nicolike.cn

Go ............. 212
来源：http://bv.shxzskj.cn

Ruby ........... 212
来源：http://ax.szsharing.cn

C# ............. 212
来源：http://gu.colortex.cn

C .............. 30
来源：http://qv.shxzskj.cn

C++ ............ 30
来源：http://nv.huixinmuqiang.cn

SQL ............ 90
来源：http://qw.yuntaijiaju.cn

Bash ........... 80
来源：http://eh.nszjky.cn

Kotlin ......... 15
来源：http://jo.szsharing.cn

Swift .......... 15
来源：http://xj.bookmarksfly.cn

Lua ............ 10
来源：http://ma.huixinmuqiang.cn

Perl ........... 10
来源：http://gf.shtwfgs.cn

Scala .......... 10
来源：http://ce.wgjwhj.cn

------------------------------------
来源：http://oj.jctech888.com.cn

合计 ........... 2106 条
来源：http://mz.bjjhwx.cn

按章节统计：
来源：http://na.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vi.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nb.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vg.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lw.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cg.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lq.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wx.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cn.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ih.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hw.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tb.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://li.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lh.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xq.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://en.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zx.haigaiapp.cn

Q SQL 专题                              90
来源：http://tb.szxytkj.cn

R Bash 专题                             80
来源：http://kp.521024.cn

S C / C++ 专题                          60
来源：http://my.huixiangedu.cn

T 其他语言补充                          60
来源：http://hq.bjjhwx.cn

U 高频实用片段                         120
来源：http://fu.lnxyls.cn

------------------------------------
来源：http://lx.shxzskj.cn

合计                                  2106 条
来源：http://ac.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://hc.panjiajie.cn

使用提醒
来源：http://tg.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ex.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qt.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uv.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gr.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xu.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zi.bookmarksfly.cn

—— 文件结束 ——
来源：http://it.asd995.cn

================================================================================
来源：http://gq.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://so.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://fn.shxzskj.cn

================================================================================
来源：http://oh.szsharing.cn

【收录内容】
来源：http://yv.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yn.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mg.bjjhwx.cn

SQL · Bash · C · C++
来源：http://xo.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ck.colortex.cn

【使用说明】
来源：http://gm.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hr.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tp.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pg.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ow.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xx.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ad.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ln.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ks.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uk.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rn.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uo.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ut.huixiangedu.cn

【文件统计】
来源：http://rx.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xt.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://md.jianghongdianzi.cn

目  录
来源：http://in.9csxet.cn

--------------------------------------------------------------------------------
来源：http://gl.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gy.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hq.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sy.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wk.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tk.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://as.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nn.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mb.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fw.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lq.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ze.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xt.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gg.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lm.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hc.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vz.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oh.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oi.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uy.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hh.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jh.panjiajie.cn

================================================================================
来源：http://el.haigaiapp.cn

A. 基础语法与类型
来源：http://ks.gzmigu.cn

================================================================================
来源：http://gq.nicolike.cn

[A01] Hello World
来源：http://qc.shxzskj.cn

Py:   print("Hello, World!")
来源：http://bk.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://dq.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://kn.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yf.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ne.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://hv.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://rd.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yn.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://qg.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://px.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kx.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vm.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ih.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://zp.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://lx.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://ks.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ij.lnxyls.cn

[A03] 常量定义
来源：http://id.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wn.521024.cn

PHP:  const PI = 3.14159;
来源：http://zm.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://jg.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://zw.asd995.cn

Java: static final double PI = 3.14159;
来源：http://uo.panjiajie.cn

Go:   const PI = 3.14159
来源：http://oy.nicolike.cn

Ruby: PI = 3.14159
来源：http://kg.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://ke.bjjhwx.cn

[A04] 判断变量类型
来源：http://nd.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nd.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tr.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tc.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://wc.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rb.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nw.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mv.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://mf.haigaiapp.cn

[A05] 整数除法与取模
来源：http://hy.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sd.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ha.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yq.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://el.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://ep.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://ff.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ex.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://em.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://ua.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://xg.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dj.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dp.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://js.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://eh.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bs.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kc.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yx.521024.cn

[A07] 数字转字符串
来源：http://mw.chemitech.net.cn

Py:   str(42)
来源：http://mc.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://sk.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://uo.chemitech.net.cn

TS:   String(42)
来源：http://km.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zu.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://cn.huixiangedu.cn

Ruby: 42.to_s
来源：http://au.wgjwhj.cn

C#:   42.ToString()
来源：http://wa.shxzskj.cn

[A08] 取整与四舍五入
来源：http://au.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mg.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gb.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sl.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://az.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wm.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vt.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pw.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bi.521024.cn

[A09] 绝对值与最大最小值
来源：http://cj.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zn.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tr.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fm.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hc.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uq.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wa.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lt.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yk.521024.cn

[A10] 生成随机数
来源：http://jd.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://zg.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://be.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://go.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rh.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://sc.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://is.nszjky.cn

Ruby: rand(1..100)
来源：http://wn.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://vo.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://vd.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://lt.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://we.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gj.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xy.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://be.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zm.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mk.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://za.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://xp.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lc.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cv.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://ee.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://hp.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://mb.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yg.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://tk.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://ms.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rh.newstarts.cn

Py:   "第一行\n第二行"
来源：http://hg.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://ah.9csxet.cn

JS:   "第一行\n第二行"
来源：http://mr.hahajie.cn

TS:   "第一行\n第二行"
来源：http://tf.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://yl.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://wb.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://lx.521024.cn

C#:   "第一行\n第二行"
来源：http://yb.panjiajie.cn

[A14] 注释写法
来源：http://tw.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mj.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bq.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://qi.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://mr.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ga.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://kg.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wv.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://at.gzmigu.cn

[A15] 空值判断与默认值
来源：http://em.szxytkj.cn

Py:   value = data or "默认值"
来源：http://de.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://kt.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://gk.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://qe.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vt.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://sr.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://pw.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://mx.yuexingan06.cn

[A16] 真假值判断规则
来源：http://vc.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yh.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://op.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uf.wgjwhj.cn

TS:   if (!x) {}
来源：http://uu.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zq.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sv.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://at.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yg.panjiajie.cn

[A17] 位运算
来源：http://qo.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gm.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zf.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://px.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jx.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sh.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qc.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://ba.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://vk.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://je.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fh.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fv.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://uv.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yl.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://na.nicolike.cn


<!-- 参考信息 -->