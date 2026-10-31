代发 wailian999

[U99] JS：事件监听
来源：http://vj.521024.cn

el.addEventListener("click", e => {})
来源：http://kn.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ca.hnjuh.cn

document.querySelector(".item")
来源：http://hu.haigaiapp.cn

[U101] JS：classList 操作
来源：http://hz.asd995.cn

el.classList.toggle("active")
来源：http://qw.szxytkj.cn

[U102] JS：本地存储
来源：http://ne.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kf.hnjuh.cn

[U103] JS：定时器
来源：http://tb.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://au.yuntaijiaju.cn

[U104] JS：防抖
来源：http://mw.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kk.yuntaijiaju.cn

[U105] JS：节流
来源：http://ti.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fg.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://cs.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eh.muxihuayi.cn

[U107] JS：数字千分位
来源：http://nu.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://af.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://uj.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ei.bookmarksfly.cn

[U109] JS：数组分组
来源：http://cp.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://am.huanxung.cn

[U110] JS：数组分块
来源：http://dk.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pw.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://vy.gzmigu.cn

new Map(Object.entries(obj))
来源：http://cr.wgjwhj.cn

[U112] JS：字符串补位
来源：http://sc.9csxet.cn

"7".padStart(3, "0")
来源：http://cr.shxzukj.cn

[U113] JS：正则替换全部
来源：http://wr.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://je.newstarts.cn

[U114] JS：JSON 深比较
来源：http://fi.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dk.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ur.9csxet.cn

crypto.randomUUID()
来源：http://bk.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://iw.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://wp.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://yj.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://jm.yuexingan06.cn

[U118] JS：开发服务器
来源：http://do.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ry.bookmarksfly.cn

[U119] JS：生产构建
来源：http://yl.huixiangedu.cn

npx vite build
来源：http://eh.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://tr.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://je.bookmarksfly.cn

================================================================================
来源：http://hi.huanxung.cn

统计汇总
来源：http://ix.chemitech.net.cn

================================================================================
来源：http://ek.bookmarksfly.cn

按语言统计（条）：
来源：http://ym.jctech888.com.cn

Python ......... 252
来源：http://wi.chemitech.net.cn

PHP ............ 252
来源：http://ux.asd995.cn

JavaScript ..... 252
来源：http://zy.shxzskj.cn

TypeScript ..... 212
来源：http://jm.nszjky.cn

Java ........... 212
来源：http://xn.bjjhwx.cn

Go ............. 212
来源：http://ca.haigaiapp.cn

Ruby ........... 212
来源：http://nl.colortex.cn

C# ............. 212
来源：http://yf.huanxung.cn

C .............. 30
来源：http://vs.lnxyls.cn

C++ ............ 30
来源：http://lg.shxzukj.cn

SQL ............ 90
来源：http://hp.jianghongdianzi.cn

Bash ........... 80
来源：http://gh.521024.cn

Kotlin ......... 15
来源：http://vh.haigaiapp.cn

Swift .......... 15
来源：http://st.yuntaijiaju.cn

Lua ............ 10
来源：http://ij.szsharing.cn

Perl ........... 10
来源：http://fi.gzmigu.cn

Scala .......... 10
来源：http://xy.panjiajie.cn

------------------------------------
来源：http://mq.muxihuayi.cn

合计 ........... 2106 条
来源：http://oh.9csxet.cn

按章节统计：
来源：http://hb.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://we.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://am.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dc.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cr.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kg.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vd.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vn.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://or.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dg.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xf.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ec.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nf.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bi.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lj.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uw.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xl.jctech888.com.cn

Q SQL 专题                              90
来源：http://jf.huanxung.cn

R Bash 专题                             80
来源：http://hc.bjjhwx.cn

S C / C++ 专题                          60
来源：http://ei.shxzskj.cn

T 其他语言补充                          60
来源：http://xe.9csxet.cn

U 高频实用片段                         120
来源：http://ri.hnjuh.cn

------------------------------------
来源：http://fx.muxihuayi.cn

合计                                  2106 条
来源：http://wl.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://kh.nicolike.cn

使用提醒
来源：http://ek.szsharing.cn

--------------------------------------------------------------------------------
来源：http://pv.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iv.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xa.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yl.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rj.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sn.szxytkj.cn

—— 文件结束 ——
来源：http://il.521024.cn

================================================================================
来源：http://cm.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://zx.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://my.chemitech.net.cn

================================================================================
来源：http://kw.lnxyls.cn

【收录内容】
来源：http://su.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ar.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gq.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://qc.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xm.huanxung.cn

【使用说明】
来源：http://jt.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lj.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pr.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tw.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ch.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ql.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vi.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ys.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xb.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dk.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ib.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ji.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vx.muxihuayi.cn

【文件统计】
来源：http://wn.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ia.szsharing.cn

--------------------------------------------------------------------------------
来源：http://nj.521024.cn

目  录
来源：http://zd.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://eq.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kz.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://id.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gy.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fv.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wq.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ps.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qu.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cg.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jn.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sg.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hk.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kz.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kv.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yz.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xs.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hp.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sp.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dz.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kl.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sr.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wi.wgjwhj.cn

================================================================================
来源：http://lt.huanxung.cn

A. 基础语法与类型
来源：http://dc.haigaiapp.cn

================================================================================
来源：http://bs.nszjky.cn

[A01] Hello World
来源：http://xn.gzmigu.cn

Py:   print("Hello, World!")
来源：http://mh.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://zy.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://vz.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sw.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://fo.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://im.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://do.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://za.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://rb.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fh.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yl.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sr.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nz.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://ni.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://sj.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://ir.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aj.muxihuayi.cn

[A03] 常量定义
来源：http://wp.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yb.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://jx.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://eh.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://uw.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://le.asd995.cn

Go:   const PI = 3.14159
来源：http://ia.shxzskj.cn

Ruby: PI = 3.14159
来源：http://zs.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ya.szsharing.cn

[A04] 判断变量类型
来源：http://hr.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zt.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ue.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fg.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://tt.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://es.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dv.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rw.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://fs.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://rl.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cs.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ap.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pn.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ez.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://zp.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://rd.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://mk.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://pz.gzmigu.cn

[A06] 字符串转数字
来源：http://yk.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://na.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://au.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dk.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zx.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sp.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ii.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ei.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qt.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://mg.yuexingan06.cn

Py:   str(42)
来源：http://bk.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://tg.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://km.huixinmuqiang.cn

TS:   String(42)
来源：http://lc.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bu.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://ue.muxihuayi.cn

Ruby: 42.to_s
来源：http://pz.newstarts.cn

C#:   42.ToString()
来源：http://sl.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://xr.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lj.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wd.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ld.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xz.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xf.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zo.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xp.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://by.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://ot.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yz.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zb.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gr.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fz.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nz.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ae.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iw.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://is.chemitech.net.cn

[A10] 生成随机数
来源：http://lf.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://hs.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://vt.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jh.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://np.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://ji.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qy.shxzskj.cn

Ruby: rand(1..100)
来源：http://hp.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://ew.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://yp.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://vl.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ae.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jf.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ly.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://zq.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ex.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oc.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fs.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://dv.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xw.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vs.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://xx.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://jr.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://rc.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pi.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://or.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://oq.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mt.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://bj.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://zb.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://sv.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://kh.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://wh.szsharing.cn

Go:   "第一行\n第二行"
来源：http://kr.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://wy.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://sq.jianghongdianzi.cn

[A14] 注释写法
来源：http://fu.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://to.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vn.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://aj.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://ub.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wg.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://yh.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://it.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://mw.521024.cn

[A15] 空值判断与默认值
来源：http://qe.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://mi.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://qz.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://vj.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://wd.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ns.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://pk.nicolike.cn

Ruby: value = data || "默认值"
来源：http://mt.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://su.chemitech.net.cn

[A16] 真假值判断规则
来源：http://sh.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wm.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://to.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vy.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://rc.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nc.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wo.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gw.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wj.szsharing.cn

[A17] 位运算
来源：http://jr.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gi.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sr.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cs.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ow.nicolike.cn


<!-- 参考信息 -->