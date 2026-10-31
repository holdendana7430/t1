代发 wailian999

[U99] JS：事件监听
来源：http://wt.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://nj.9csxet.cn

[U100] JS：DOM 查询
来源：http://tp.szsharing.cn

document.querySelector(".item")
来源：http://mx.muxihuayi.cn

[U101] JS：classList 操作
来源：http://cb.bjjhwx.cn

el.classList.toggle("active")
来源：http://pu.yuexingan06.cn

[U102] JS：本地存储
来源：http://rs.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lx.muxihuayi.cn

[U103] JS：定时器
来源：http://ld.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zg.colortex.cn

[U104] JS：防抖
来源：http://px.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://le.yuexingan06.cn

[U105] JS：节流
来源：http://dz.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sz.huanxung.cn

[U106] JS：日期格式化
来源：http://ha.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ex.newstarts.cn

[U107] JS：数字千分位
来源：http://qt.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ir.haigaiapp.cn

[U108] JS：随机整数
来源：http://vu.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://io.jctech888.com.cn

[U109] JS：数组分组
来源：http://jd.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ad.panjiajie.cn

[U110] JS：数组分块
来源：http://nq.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dw.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://hf.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://yo.9csxet.cn

[U112] JS：字符串补位
来源：http://zz.haigaiapp.cn

"7".padStart(3, "0")
来源：http://so.panjiajie.cn

[U113] JS：正则替换全部
来源：http://us.hahajie.cn

s.replaceAll("a", "b")
来源：http://py.hahajie.cn

[U114] JS：JSON 深比较
来源：http://mm.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xe.newstarts.cn

[U115] JS：生成 UUID
来源：http://hu.yuexingan06.cn

crypto.randomUUID()
来源：http://iu.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://he.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://am.yuexingan06.cn

[U117] JS：单元测试
来源：http://iw.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://cl.huanxung.cn

[U118] JS：开发服务器
来源：http://qe.szsharing.cn

npm i -D vite;  npx vite
来源：http://po.newstarts.cn

[U119] JS：生产构建
来源：http://oq.asd995.cn

npx vite build
来源：http://la.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://ue.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://hc.muxihuayi.cn

================================================================================
来源：http://au.nszjky.cn

统计汇总
来源：http://ih.hnjuh.cn

================================================================================
来源：http://jr.jianghongdianzi.cn

按语言统计（条）：
来源：http://eg.asd995.cn

Python ......... 252
来源：http://lq.colortex.cn

PHP ............ 252
来源：http://zg.yuexingan06.cn

JavaScript ..... 252
来源：http://yn.wgjwhj.cn

TypeScript ..... 212
来源：http://uz.gzmigu.cn

Java ........... 212
来源：http://av.szsharing.cn

Go ............. 212
来源：http://vx.panjiajie.cn

Ruby ........... 212
来源：http://ey.asd995.cn

C# ............. 212
来源：http://ia.shxzskj.cn

C .............. 30
来源：http://qo.huixinmuqiang.cn

C++ ............ 30
来源：http://rp.521024.cn

SQL ............ 90
来源：http://zy.szsharing.cn

Bash ........... 80
来源：http://dd.szsharing.cn

Kotlin ......... 15
来源：http://hk.yuntaijiaju.cn

Swift .......... 15
来源：http://ox.wgjwhj.cn

Lua ............ 10
来源：http://gc.yuntaijiaju.cn

Perl ........... 10
来源：http://oh.hnjuh.cn

Scala .......... 10
来源：http://jp.hnjuh.cn

------------------------------------
来源：http://tv.nszjky.cn

合计 ........... 2106 条
来源：http://od.haigaiapp.cn

按章节统计：
来源：http://mt.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ue.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mf.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vn.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lk.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ak.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://al.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ja.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hw.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xi.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hf.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bo.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gk.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vg.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ye.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nd.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cl.shtwfgs.cn

Q SQL 专题                              90
来源：http://ss.asd995.cn

R Bash 专题                             80
来源：http://vq.hnjuh.cn

S C / C++ 专题                          60
来源：http://pg.yuexingan06.cn

T 其他语言补充                          60
来源：http://yw.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://ac.hnjuh.cn

------------------------------------
来源：http://pl.hahajie.cn

合计                                  2106 条
来源：http://fa.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://pk.huanxung.cn

使用提醒
来源：http://qc.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://sp.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tf.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://um.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nn.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mo.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dx.shtwfgs.cn

—— 文件结束 ——
来源：http://oq.bookmarksfly.cn

================================================================================
来源：http://ey.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://tv.asd995.cn

Common Programming Examples Cheat Book
来源：http://hn.szxytkj.cn

================================================================================
来源：http://nd.lnxyls.cn

【收录内容】
来源：http://oh.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yj.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://no.shtwfgs.cn

SQL · Bash · C · C++
来源：http://wg.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jk.wgjwhj.cn

【使用说明】
来源：http://po.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ij.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pf.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bf.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ga.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oi.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ga.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qr.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wn.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rc.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lr.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wr.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ew.asd995.cn

【文件统计】
来源：http://uz.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mp.newstarts.cn

--------------------------------------------------------------------------------
来源：http://fa.szxytkj.cn

目  录
来源：http://gh.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://rl.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aq.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://an.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mj.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bh.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vv.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pz.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zt.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://od.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yj.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kg.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gb.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hk.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wu.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hd.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eu.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mx.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cg.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wt.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uw.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://as.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://co.shtwfgs.cn

================================================================================
来源：http://pi.yuexingan06.cn

A. 基础语法与类型
来源：http://vj.gzmigu.cn

================================================================================
来源：http://sf.shxzskj.cn

[A01] Hello World
来源：http://qe.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://zt.asd995.cn

PHP:  echo "Hello, World!";
来源：http://tm.colortex.cn

JS:   console.log("Hello, World!");
来源：http://zs.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gd.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://om.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://jj.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://nj.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hg.szxytkj.cn

[A02] 变量声明与赋值
来源：http://uw.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://py.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gm.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wi.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jm.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://uq.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://ac.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://nh.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sh.jctech888.com.cn

[A03] 常量定义
来源：http://sc.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rn.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://bb.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://fy.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://fw.asd995.cn

Java: static final double PI = 3.14159;
来源：http://uy.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://lz.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://fy.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://zr.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://oi.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dz.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mn.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yz.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://uj.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hr.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pv.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xt.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://uw.muxihuayi.cn

[A05] 整数除法与取模
来源：http://hf.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lq.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fh.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://py.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ux.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://td.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://zu.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://hu.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://yh.newstarts.cn

[A06] 字符串转数字
来源：http://cm.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://rm.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ah.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uj.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hq.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://is.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wj.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://la.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qo.shxzskj.cn

[A07] 数字转字符串
来源：http://au.chemitech.net.cn

Py:   str(42)
来源：http://qq.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://ou.colortex.cn

JS:   String(42); (42).toString()
来源：http://gb.bjjhwx.cn

TS:   String(42)
来源：http://iw.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bm.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://to.chemitech.net.cn

Ruby: 42.to_s
来源：http://cx.haigaiapp.cn

C#:   42.ToString()
来源：http://oa.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://jm.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sr.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vw.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ku.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://an.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://na.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kt.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vy.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dm.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://od.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ka.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aw.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ib.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lw.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dj.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cf.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wr.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ua.muxihuayi.cn

[A10] 生成随机数
来源：http://st.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://kz.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://cq.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qt.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zi.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://zb.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ji.hnjuh.cn

Ruby: rand(1..100)
来源：http://oe.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://bp.huanxung.cn

[A11] 条件表达式（三元）
来源：http://rw.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://xc.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cr.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fe.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zl.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://cn.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jm.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bi.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://po.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://kw.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ii.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uf.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://dg.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://jt.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://js.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mn.521024.cn

Ruby: "Hello, #{name}!"
来源：http://bk.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://ew.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://om.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://tv.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://yv.szsharing.cn

JS:   "第一行\n第二行"
来源：http://ur.colortex.cn

TS:   "第一行\n第二行"
来源：http://dc.szxytkj.cn

Java: "第一行\n第二行"
来源：http://rh.colortex.cn

Go:   "第一行\n第二行"
来源：http://wn.asd995.cn

Ruby: "第一行\n第二行"
来源：http://ve.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://jp.chemitech.net.cn

[A14] 注释写法
来源：http://hg.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sl.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xd.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://gp.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://bu.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wv.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://uh.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vn.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://dq.asd995.cn

[A15] 空值判断与默认值
来源：http://zc.colortex.cn

Py:   value = data or "默认值"
来源：http://xt.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://yu.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://cp.521024.cn

TS:   const value = data ?? "默认值";
来源：http://zm.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dt.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://gc.521024.cn

Ruby: value = data || "默认值"
来源：http://hi.521024.cn

C#:   var value = data ?? "默认值";
来源：http://mu.nszjky.cn

[A16] 真假值判断规则
来源：http://ot.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fr.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tt.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eu.shxzukj.cn

TS:   if (!x) {}
来源：http://mm.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ox.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tp.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lp.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ud.yuexingan06.cn

[A17] 位运算
来源：http://do.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wf.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ep.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ry.lnxyls.cn


<!-- 参考信息 -->