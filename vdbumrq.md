代发 wailian999

[U101] JS：classList 操作
来源：http://au.gzmigu.cn

el.classList.toggle("active")
来源：http://ec.colortex.cn

[U102] JS：本地存储
来源：http://ws.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mh.haigaiapp.cn

[U103] JS：定时器
来源：http://zv.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ui.hnjuh.cn

[U104] JS：防抖
来源：http://qw.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qn.bjjhwx.cn

[U105] JS：节流
来源：http://ch.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cf.colortex.cn

[U106] JS：日期格式化
来源：http://xl.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://im.szxytkj.cn

[U107] JS：数字千分位
来源：http://om.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cs.bookmarksfly.cn

[U108] JS：随机整数
来源：http://nc.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fj.jctech888.com.cn

[U109] JS：数组分组
来源：http://rj.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://zr.bjjhwx.cn

[U110] JS：数组分块
来源：http://su.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gl.gzmigu.cn

[U111] JS：对象转 Map
来源：http://vg.szxytkj.cn

new Map(Object.entries(obj))
来源：http://jo.huanxung.cn

[U112] JS：字符串补位
来源：http://zl.bjjhwx.cn

"7".padStart(3, "0")
来源：http://zt.hahajie.cn

[U113] JS：正则替换全部
来源：http://xm.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://jz.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://sf.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qj.nszjky.cn

[U115] JS：生成 UUID
来源：http://xh.muxihuayi.cn

crypto.randomUUID()
来源：http://bt.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://jr.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://oq.huanxung.cn

[U117] JS：单元测试
来源：http://en.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://cx.yuexingan06.cn

[U118] JS：开发服务器
来源：http://vx.newstarts.cn

npm i -D vite;  npx vite
来源：http://dk.nicolike.cn

[U119] JS：生产构建
来源：http://uz.shxzskj.cn

npx vite build
来源：http://gg.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://bh.521024.cn

import.meta.env.VITE_API_URL
来源：http://pk.nszjky.cn

================================================================================
来源：http://nk.panjiajie.cn

统计汇总
来源：http://no.panjiajie.cn

================================================================================
来源：http://ha.hahajie.cn

按语言统计（条）：
来源：http://af.yuntaijiaju.cn

Python ......... 252
来源：http://jf.9csxet.cn

PHP ............ 252
来源：http://rd.bookmarksfly.cn

JavaScript ..... 252
来源：http://cr.huixiangedu.cn

TypeScript ..... 212
来源：http://ex.colortex.cn

Java ........... 212
来源：http://ky.lnxyls.cn

Go ............. 212
来源：http://ka.gzmigu.cn

Ruby ........... 212
来源：http://wn.haigaiapp.cn

C# ............. 212
来源：http://tf.yuntaijiaju.cn

C .............. 30
来源：http://pa.yuntaijiaju.cn

C++ ............ 30
来源：http://im.haigaiapp.cn

SQL ............ 90
来源：http://bi.9csxet.cn

Bash ........... 80
来源：http://re.yuntaijiaju.cn

Kotlin ......... 15
来源：http://kz.shxzskj.cn

Swift .......... 15
来源：http://wx.shxzskj.cn

Lua ............ 10
来源：http://pp.colortex.cn

Perl ........... 10
来源：http://ua.chemitech.net.cn

Scala .......... 10
来源：http://uu.huixiangedu.cn

------------------------------------
来源：http://ab.shxzukj.cn

合计 ........... 2106 条
来源：http://uq.szxytkj.cn

按章节统计：
来源：http://eo.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uo.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fo.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oe.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bd.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://na.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zb.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ji.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sx.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qj.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wg.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sd.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ym.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nm.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sg.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://or.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fy.nszjky.cn

Q SQL 专题                              90
来源：http://jp.yuntaijiaju.cn

R Bash 专题                             80
来源：http://ye.gzmigu.cn

S C / C++ 专题                          60
来源：http://as.shtwfgs.cn

T 其他语言补充                          60
来源：http://kw.nicolike.cn

U 高频实用片段                         120
来源：http://fr.hahajie.cn

------------------------------------
来源：http://xu.gzmigu.cn

合计                                  2106 条
来源：http://uf.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://nt.521024.cn

使用提醒
来源：http://lt.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://or.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xu.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cr.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lm.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ag.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vy.chemitech.net.cn

—— 文件结束 ——
来源：http://kk.colortex.cn

================================================================================
来源：http://wz.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://pi.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://as.huixinmuqiang.cn

================================================================================
来源：http://xt.9csxet.cn

【收录内容】
来源：http://el.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gj.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ll.jctech888.com.cn

SQL · Bash · C · C++
来源：http://uj.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qi.colortex.cn

【使用说明】
来源：http://pf.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nq.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tb.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eh.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tw.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oz.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qz.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cf.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vq.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ga.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wt.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jh.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://up.nszjky.cn

【文件统计】
来源：http://hs.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zk.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://vp.lnxyls.cn

目  录
来源：http://us.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://qh.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sj.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://of.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lj.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://si.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ob.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vk.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vz.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fj.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cm.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lg.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oi.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://un.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cl.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vb.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lq.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ko.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ys.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xm.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xl.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pg.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gq.huixiangedu.cn

================================================================================
来源：http://bb.hahajie.cn

A. 基础语法与类型
来源：http://pr.chemitech.net.cn

================================================================================
来源：http://ab.nszjky.cn

[A01] Hello World
来源：http://xg.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://uj.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://qh.colortex.cn

JS:   console.log("Hello, World!");
来源：http://uj.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wn.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ko.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://jn.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://zg.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nk.521024.cn

[A02] 变量声明与赋值
来源：http://ef.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oy.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wn.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cm.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lf.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://uq.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://tq.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://md.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xq.chemitech.net.cn

[A03] 常量定义
来源：http://ss.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xw.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://xr.asd995.cn

JS:   const PI = 3.14159;
来源：http://xh.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://ub.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://dj.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://ah.9csxet.cn

Ruby: PI = 3.14159
来源：http://mx.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://wp.hahajie.cn

[A04] 判断变量类型
来源：http://bo.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uh.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bg.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pt.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://be.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tt.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vb.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bx.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://kf.huixiangedu.cn

[A05] 整数除法与取模
来源：http://nh.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fz.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://eb.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gc.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kt.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://lu.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://we.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://lp.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://lk.lnxyls.cn

[A06] 字符串转数字
来源：http://ew.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://yb.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://el.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jq.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ml.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gj.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ur.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eu.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qu.521024.cn

[A07] 数字转字符串
来源：http://pf.shtwfgs.cn

Py:   str(42)
来源：http://bq.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://tw.nicolike.cn

JS:   String(42); (42).toString()
来源：http://bv.9csxet.cn

TS:   String(42)
来源：http://dn.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xa.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://cm.shtwfgs.cn

Ruby: 42.to_s
来源：http://ot.wgjwhj.cn

C#:   42.ToString()
来源：http://ea.lnxyls.cn

[A08] 取整与四舍五入
来源：http://hs.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hy.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bm.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lg.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gl.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nl.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wx.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zt.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uv.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://qp.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ig.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nr.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gg.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vj.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wz.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dt.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kq.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mx.hnjuh.cn

[A10] 生成随机数
来源：http://lu.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://wu.nicolike.cn

PHP:  random_int(1, 100);
来源：http://zh.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qg.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://io.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://rz.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oa.hahajie.cn

Ruby: rand(1..100)
来源：http://db.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://ii.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://jg.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://iy.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zr.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ia.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ov.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://no.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zt.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oz.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cw.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://nq.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://im.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qg.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://az.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://di.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://tx.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ge.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://am.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://jr.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uo.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://ry.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://ix.nicolike.cn

JS:   "第一行\n第二行"
来源：http://uz.hahajie.cn

TS:   "第一行\n第二行"
来源：http://jd.asd995.cn

Java: "第一行\n第二行"
来源：http://mh.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://gt.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://bd.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://cf.shxzskj.cn

[A14] 注释写法
来源：http://mt.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sj.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eh.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ij.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://rq.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ex.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://va.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rt.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://ov.hnjuh.cn

[A15] 空值判断与默认值
来源：http://wr.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://nz.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://qm.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://qs.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://vo.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zo.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://xk.colortex.cn

Ruby: value = data || "默认值"
来源：http://vy.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://yl.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://xj.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ys.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cs.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zv.colortex.cn

TS:   if (!x) {}
来源：http://gg.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ep.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qc.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://on.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xw.haigaiapp.cn

[A17] 位运算
来源：http://dq.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tx.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bd.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ms.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jl.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wi.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fz.hnjuh.cn


<!-- 参考信息 -->