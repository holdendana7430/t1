代发 wailian999

[U99] JS：事件监听
来源：http://wx.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://tc.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://rf.yuntaijiaju.cn

document.querySelector(".item")
来源：http://nl.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://uh.bookmarksfly.cn

el.classList.toggle("active")
来源：http://ll.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://az.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lk.shxzukj.cn

[U103] JS：定时器
来源：http://gk.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ob.521024.cn

[U104] JS：防抖
来源：http://ia.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://np.szxytkj.cn

[U105] JS：节流
来源：http://zz.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xe.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://vm.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ft.jctech888.com.cn

[U107] JS：数字千分位
来源：http://ui.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ec.huanxung.cn

[U108] JS：随机整数
来源：http://pg.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pi.hahajie.cn

[U109] JS：数组分组
来源：http://th.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://tq.lnxyls.cn

[U110] JS：数组分块
来源：http://fg.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nb.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://bn.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://lk.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://pd.shtwfgs.cn

"7".padStart(3, "0")
来源：http://mr.nszjky.cn

[U113] JS：正则替换全部
来源：http://ai.szsharing.cn

s.replaceAll("a", "b")
来源：http://ha.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://gw.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cm.shxzskj.cn

[U115] JS：生成 UUID
来源：http://yw.shxzukj.cn

crypto.randomUUID()
来源：http://tu.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://lk.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://my.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://aw.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://vs.nszjky.cn

[U118] JS：开发服务器
来源：http://tg.nszjky.cn

npm i -D vite;  npx vite
来源：http://hj.gzmigu.cn

[U119] JS：生产构建
来源：http://rh.asd995.cn

npx vite build
来源：http://ku.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rq.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ab.gzmigu.cn

================================================================================
来源：http://zc.jctech888.com.cn

统计汇总
来源：http://kr.yuexingan06.cn

================================================================================
来源：http://oh.yuexingan06.cn

按语言统计（条）：
来源：http://hy.shtwfgs.cn

Python ......... 252
来源：http://qw.asd995.cn

PHP ............ 252
来源：http://wx.muxihuayi.cn

JavaScript ..... 252
来源：http://dx.huixiangedu.cn

TypeScript ..... 212
来源：http://hb.muxihuayi.cn

Java ........... 212
来源：http://yq.haigaiapp.cn

Go ............. 212
来源：http://mf.chemitech.net.cn

Ruby ........... 212
来源：http://fr.shxzukj.cn

C# ............. 212
来源：http://se.muxihuayi.cn

C .............. 30
来源：http://ap.huanxung.cn

C++ ............ 30
来源：http://yx.shxzukj.cn

SQL ............ 90
来源：http://ma.bookmarksfly.cn

Bash ........... 80
来源：http://cr.9csxet.cn

Kotlin ......... 15
来源：http://ap.huixinmuqiang.cn

Swift .......... 15
来源：http://ne.lnxyls.cn

Lua ............ 10
来源：http://oo.jianghongdianzi.cn

Perl ........... 10
来源：http://xx.nszjky.cn

Scala .......... 10
来源：http://yz.shxzukj.cn

------------------------------------
来源：http://yc.chemitech.net.cn

合计 ........... 2106 条
来源：http://wq.bjjhwx.cn

按章节统计：
来源：http://me.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zp.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://po.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ne.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eg.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vo.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://en.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gn.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wg.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://js.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ll.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uf.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ed.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://au.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cl.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yh.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mh.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://az.shxzukj.cn

R Bash 专题                             80
来源：http://vh.wgjwhj.cn

S C / C++ 专题                          60
来源：http://ee.asd995.cn

T 其他语言补充                          60
来源：http://eo.521024.cn

U 高频实用片段                         120
来源：http://yf.yuntaijiaju.cn

------------------------------------
来源：http://bs.muxihuayi.cn

合计                                  2106 条
来源：http://qf.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://hb.szsharing.cn

使用提醒
来源：http://kf.asd995.cn

--------------------------------------------------------------------------------
来源：http://pb.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hj.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cv.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oe.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://td.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sz.muxihuayi.cn

—— 文件结束 ——
来源：http://um.haigaiapp.cn

================================================================================
来源：http://ma.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://fq.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://wp.yuexingan06.cn

================================================================================
来源：http://rb.huixinmuqiang.cn

【收录内容】
来源：http://xa.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mu.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vh.shtwfgs.cn

SQL · Bash · C · C++
来源：http://po.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ta.nszjky.cn

【使用说明】
来源：http://ly.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cf.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ay.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lo.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ed.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ta.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mn.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mk.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://om.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xo.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://we.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://et.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bk.chemitech.net.cn

【文件统计】
来源：http://ye.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ak.nszjky.cn

--------------------------------------------------------------------------------
来源：http://tf.haigaiapp.cn

目  录
来源：http://uo.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bi.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hc.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://my.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://am.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xc.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yf.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vs.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wi.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://by.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ph.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://te.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wo.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pl.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ya.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aw.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gw.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ch.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gg.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zv.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mx.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ns.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pi.huixinmuqiang.cn

================================================================================
来源：http://qc.gzmigu.cn

A. 基础语法与类型
来源：http://wk.muxihuayi.cn

================================================================================
来源：http://ri.colortex.cn

[A01] Hello World
来源：http://bn.huanxung.cn

Py:   print("Hello, World!")
来源：http://ua.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://st.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://sl.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sc.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://we.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ts.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://qu.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gs.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://yv.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ot.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jj.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mt.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://id.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://mb.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://mn.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://dv.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jg.9csxet.cn

[A03] 常量定义
来源：http://pe.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yi.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://pl.szsharing.cn

JS:   const PI = 3.14159;
来源：http://hf.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://sq.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://ob.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://xn.newstarts.cn

Ruby: PI = 3.14159
来源：http://vr.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://xa.shtwfgs.cn

[A04] 判断变量类型
来源：http://xu.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mq.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sq.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kp.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://tw.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tf.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ug.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uq.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://rl.huixiangedu.cn

[A05] 整数除法与取模
来源：http://vy.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fi.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nj.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jj.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vy.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://zx.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://hp.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://vt.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://gx.521024.cn

[A06] 字符串转数字
来源：http://hk.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://wm.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tv.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wp.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bm.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ta.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ka.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pu.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pw.muxihuayi.cn

[A07] 数字转字符串
来源：http://zu.nszjky.cn

Py:   str(42)
来源：http://ka.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://ws.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://gw.9csxet.cn

TS:   String(42)
来源：http://vf.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fc.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://ow.bjjhwx.cn

Ruby: 42.to_s
来源：http://zc.521024.cn

C#:   42.ToString()
来源：http://ub.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://ln.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eu.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tf.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jh.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bv.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iy.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rf.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://an.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ub.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://bg.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eb.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ns.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oz.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ht.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hl.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nf.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ae.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ub.yuexingan06.cn

[A10] 生成随机数
来源：http://gf.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://iy.9csxet.cn

PHP:  random_int(1, 100);
来源：http://yu.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ik.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wc.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://ou.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yn.nszjky.cn

Ruby: rand(1..100)
来源：http://gi.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://sv.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://qv.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://ws.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://et.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://em.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ic.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://jp.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://na.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wr.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wm.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://lr.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ou.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bh.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://wu.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://wu.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://en.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gj.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://xd.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://ci.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bf.nicolike.cn

Py:   "第一行\n第二行"
来源：http://je.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://py.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://dl.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://uh.colortex.cn

Java: "第一行\n第二行"
来源：http://un.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://fu.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://cm.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://zo.shtwfgs.cn

[A14] 注释写法
来源：http://dy.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://br.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fn.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://px.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://xs.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wk.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://li.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ri.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://ct.nszjky.cn

[A15] 空值判断与默认值
来源：http://pl.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ff.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://bw.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://rh.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://ax.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xp.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://cc.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://gq.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://lw.shxzskj.cn

[A16] 真假值判断规则
来源：http://uv.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pm.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xv.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gl.jctech888.com.cn

TS:   if (!x) {}
来源：http://dt.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pa.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tu.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gv.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ea.panjiajie.cn

[A17] 位运算
来源：http://ap.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rg.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hm.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kv.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uq.chemitech.net.cn


<!-- 参考信息 -->