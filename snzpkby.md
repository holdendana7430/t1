代发 wailian999

[U103] JS：定时器
来源：http://oh.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gf.haigaiapp.cn

[U104] JS：防抖
来源：http://mh.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cq.huixinmuqiang.cn

[U105] JS：节流
来源：http://eb.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rm.nszjky.cn

[U106] JS：日期格式化
来源：http://yp.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ib.9csxet.cn

[U107] JS：数字千分位
来源：http://jh.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gb.shxzskj.cn

[U108] JS：随机整数
来源：http://rq.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zl.huixiangedu.cn

[U109] JS：数组分组
来源：http://yw.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://us.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://ht.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rn.nszjky.cn

[U111] JS：对象转 Map
来源：http://gd.nszjky.cn

new Map(Object.entries(obj))
来源：http://es.szsharing.cn

[U112] JS：字符串补位
来源：http://yo.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://hg.521024.cn

[U113] JS：正则替换全部
来源：http://kw.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://ki.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://ch.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://li.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://ed.szsharing.cn

crypto.randomUUID()
来源：http://gd.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://zc.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://jf.gzmigu.cn

[U117] JS：单元测试
来源：http://ia.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://qb.huixiangedu.cn

[U118] JS：开发服务器
来源：http://vu.9csxet.cn

npm i -D vite;  npx vite
来源：http://nd.lnxyls.cn

[U119] JS：生产构建
来源：http://tg.lnxyls.cn

npx vite build
来源：http://tf.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://yj.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://zl.huanxung.cn

================================================================================
来源：http://zo.szsharing.cn

统计汇总
来源：http://kq.newstarts.cn

================================================================================
来源：http://jm.521024.cn

按语言统计（条）：
来源：http://xh.jctech888.com.cn

Python ......... 252
来源：http://er.asd995.cn

PHP ............ 252
来源：http://mx.shtwfgs.cn

JavaScript ..... 252
来源：http://py.huanxung.cn

TypeScript ..... 212
来源：http://om.panjiajie.cn

Java ........... 212
来源：http://km.lnxyls.cn

Go ............. 212
来源：http://ho.bjjhwx.cn

Ruby ........... 212
来源：http://df.gzmigu.cn

C# ............. 212
来源：http://td.wgjwhj.cn

C .............. 30
来源：http://th.szsharing.cn

C++ ............ 30
来源：http://vz.bjjhwx.cn

SQL ............ 90
来源：http://as.jctech888.com.cn

Bash ........... 80
来源：http://wy.nszjky.cn

Kotlin ......... 15
来源：http://wv.newstarts.cn

Swift .......... 15
来源：http://qq.szxytkj.cn

Lua ............ 10
来源：http://oo.shtwfgs.cn

Perl ........... 10
来源：http://yw.szxytkj.cn

Scala .......... 10
来源：http://jn.521024.cn

------------------------------------
来源：http://rg.hnjuh.cn

合计 ........... 2106 条
来源：http://ut.shxzukj.cn

按章节统计：
来源：http://di.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rw.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qd.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tv.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ls.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://en.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qm.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gq.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wr.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cm.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eh.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sf.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mc.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ps.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kk.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ym.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yv.huixiangedu.cn

Q SQL 专题                              90
来源：http://cf.yuexingan06.cn

R Bash 专题                             80
来源：http://bd.chemitech.net.cn

S C / C++ 专题                          60
来源：http://kh.bookmarksfly.cn

T 其他语言补充                          60
来源：http://je.lnxyls.cn

U 高频实用片段                         120
来源：http://jm.bjjhwx.cn

------------------------------------
来源：http://wt.bjjhwx.cn

合计                                  2106 条
来源：http://zs.asd995.cn

--------------------------------------------------------------------------------
来源：http://uh.lnxyls.cn

使用提醒
来源：http://lo.9csxet.cn

--------------------------------------------------------------------------------
来源：http://to.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ci.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kc.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://go.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tz.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ha.hahajie.cn

—— 文件结束 ——
来源：http://lw.huixiangedu.cn

================================================================================
来源：http://hp.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://dw.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://wh.huixiangedu.cn

================================================================================
来源：http://ko.jctech888.com.cn

【收录内容】
来源：http://rl.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jp.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cy.huanxung.cn

SQL · Bash · C · C++
来源：http://ng.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://la.szxytkj.cn

【使用说明】
来源：http://hu.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qr.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://he.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qj.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cv.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://if.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sa.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ju.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ty.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wa.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cc.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rw.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qu.jctech888.com.cn

【文件统计】
来源：http://ad.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ae.szsharing.cn

--------------------------------------------------------------------------------
来源：http://or.szxytkj.cn

目  录
来源：http://gw.huanxung.cn

--------------------------------------------------------------------------------
来源：http://wx.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xy.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iw.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gq.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eu.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://er.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mz.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ck.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vt.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wm.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jb.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://da.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tq.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://at.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oc.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://il.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ma.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zh.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hm.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ej.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ei.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tx.shxzskj.cn

================================================================================
来源：http://ek.newstarts.cn

A. 基础语法与类型
来源：http://ac.szsharing.cn

================================================================================
来源：http://mh.bookmarksfly.cn

[A01] Hello World
来源：http://pn.shxzukj.cn

Py:   print("Hello, World!")
来源：http://qi.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://os.colortex.cn

JS:   console.log("Hello, World!");
来源：http://os.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ja.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://db.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://xz.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://rt.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zt.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://so.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xo.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fv.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ni.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wm.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://mf.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://zs.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://qc.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pi.shtwfgs.cn

[A03] 常量定义
来源：http://ho.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fa.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://wl.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://pw.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://qn.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://hc.gzmigu.cn

Go:   const PI = 3.14159
来源：http://ax.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://ds.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://ah.wgjwhj.cn

[A04] 判断变量类型
来源：http://ye.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vk.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fy.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wd.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://np.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wx.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nr.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zh.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://uy.chemitech.net.cn

[A05] 整数除法与取模
来源：http://tw.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nx.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bp.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://di.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ss.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://yg.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://af.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://hi.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://cy.yuexingan06.cn

[A06] 字符串转数字
来源：http://my.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://py.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cj.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nh.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ll.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dg.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vf.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ie.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ts.shxzskj.cn

[A07] 数字转字符串
来源：http://yk.gzmigu.cn

Py:   str(42)
来源：http://tq.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://fq.colortex.cn

JS:   String(42); (42).toString()
来源：http://xr.huanxung.cn

TS:   String(42)
来源：http://lq.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mw.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://hx.haigaiapp.cn

Ruby: 42.to_s
来源：http://ui.hahajie.cn

C#:   42.ToString()
来源：http://bx.newstarts.cn

[A08] 取整与四舍五入
来源：http://sx.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wf.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dm.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ve.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://um.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cr.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kl.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hn.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://op.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://fe.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xw.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jc.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rw.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bk.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sl.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gc.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dq.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oo.shxzskj.cn

[A10] 生成随机数
来源：http://wr.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://dn.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://ss.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gn.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bh.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://lt.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://am.nszjky.cn

Ruby: rand(1..100)
来源：http://nj.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://og.huanxung.cn

[A11] 条件表达式（三元）
来源：http://yz.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://bo.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uy.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pu.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oy.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://ta.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ro.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qr.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xr.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://ri.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ow.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uh.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://cu.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ec.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://dv.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kj.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://cu.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://fo.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yx.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://kg.colortex.cn

PHP:  "第一行\n第二行"
来源：http://vj.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://yx.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://gv.lnxyls.cn

Java: "第一行\n第二行"
来源：http://ty.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://hy.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://yq.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://yz.shxzukj.cn

[A14] 注释写法
来源：http://fy.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ot.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bp.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://ic.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://nw.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ub.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://dx.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uj.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://cc.szsharing.cn

[A15] 空值判断与默认值
来源：http://dc.nszjky.cn

Py:   value = data or "默认值"
来源：http://wg.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://ix.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://tn.521024.cn

TS:   const value = data ?? "默认值";
来源：http://al.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ko.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://nj.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://hv.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://lw.nicolike.cn

[A16] 真假值判断规则
来源：http://or.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ij.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ds.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qv.hnjuh.cn

TS:   if (!x) {}
来源：http://fx.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wy.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://so.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rb.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wv.panjiajie.cn

[A17] 位运算
来源：http://qs.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://st.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vr.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rr.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uk.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lt.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://pd.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://yy.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://qv.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fz.9csxet.cn


<!-- 参考信息 -->