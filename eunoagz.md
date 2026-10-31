代发 wailian999

[U99] JS：事件监听
来源：http://yk.colortex.cn

el.addEventListener("click", e => {})
来源：http://fj.nicolike.cn

[U100] JS：DOM 查询
来源：http://zw.huanxung.cn

document.querySelector(".item")
来源：http://hl.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://oe.hahajie.cn

el.classList.toggle("active")
来源：http://cq.colortex.cn

[U102] JS：本地存储
来源：http://gx.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hr.newstarts.cn

[U103] JS：定时器
来源：http://gk.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cv.szsharing.cn

[U104] JS：防抖
来源：http://nl.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wa.muxihuayi.cn

[U105] JS：节流
来源：http://hw.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yr.newstarts.cn

[U106] JS：日期格式化
来源：http://xj.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ex.hahajie.cn

[U107] JS：数字千分位
来源：http://fm.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vw.szsharing.cn

[U108] JS：随机整数
来源：http://rk.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ut.gzmigu.cn

[U109] JS：数组分组
来源：http://hr.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://pp.szxytkj.cn

[U110] JS：数组分块
来源：http://yi.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ln.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://dr.hahajie.cn

new Map(Object.entries(obj))
来源：http://ve.newstarts.cn

[U112] JS：字符串补位
来源：http://ca.hahajie.cn

"7".padStart(3, "0")
来源：http://fo.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://qy.huanxung.cn

s.replaceAll("a", "b")
来源：http://no.huanxung.cn

[U114] JS：JSON 深比较
来源：http://wy.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://do.521024.cn

crypto.randomUUID()
来源：http://jf.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://xh.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://sg.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://kl.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://lv.colortex.cn

[U118] JS：开发服务器
来源：http://qf.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://oz.shxzukj.cn

[U119] JS：生产构建
来源：http://xi.wgjwhj.cn

npx vite build
来源：http://je.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://xe.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://yo.shxzukj.cn

================================================================================
来源：http://iv.shxzskj.cn

统计汇总
来源：http://cz.yuntaijiaju.cn

================================================================================
来源：http://fo.haigaiapp.cn

按语言统计（条）：
来源：http://rs.newstarts.cn

Python ......... 252
来源：http://om.gzmigu.cn

PHP ............ 252
来源：http://ik.hnjuh.cn

JavaScript ..... 252
来源：http://rn.haigaiapp.cn

TypeScript ..... 212
来源：http://bt.newstarts.cn

Java ........... 212
来源：http://hk.521024.cn

Go ............. 212
来源：http://ck.colortex.cn

Ruby ........... 212
来源：http://ri.szsharing.cn

C# ............. 212
来源：http://fh.szsharing.cn

C .............. 30
来源：http://xy.shxzskj.cn

C++ ............ 30
来源：http://fm.521024.cn

SQL ............ 90
来源：http://wp.newstarts.cn

Bash ........... 80
来源：http://en.shxzukj.cn

Kotlin ......... 15
来源：http://nh.lnxyls.cn

Swift .......... 15
来源：http://nk.chemitech.net.cn

Lua ............ 10
来源：http://ps.shxzukj.cn

Perl ........... 10
来源：http://tc.lnxyls.cn

Scala .......... 10
来源：http://kq.yuntaijiaju.cn

------------------------------------
来源：http://pj.bookmarksfly.cn

合计 ........... 2106 条
来源：http://fy.hnjuh.cn

按章节统计：
来源：http://la.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kl.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tl.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zj.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://te.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hx.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://le.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fz.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rw.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sf.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mi.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vv.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eh.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uy.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rq.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vy.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fs.szsharing.cn

Q SQL 专题                              90
来源：http://gd.muxihuayi.cn

R Bash 专题                             80
来源：http://wl.huanxung.cn

S C / C++ 专题                          60
来源：http://zs.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://jn.panjiajie.cn

U 高频实用片段                         120
来源：http://uw.szsharing.cn

------------------------------------
来源：http://op.chemitech.net.cn

合计                                  2106 条
来源：http://jt.9csxet.cn

--------------------------------------------------------------------------------
来源：http://wg.chemitech.net.cn

使用提醒
来源：http://ak.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ld.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rk.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fq.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sk.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qo.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ce.521024.cn

—— 文件结束 ——
来源：http://md.panjiajie.cn

================================================================================
来源：http://vs.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://um.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://ly.lnxyls.cn

================================================================================
来源：http://ei.szsharing.cn

【收录内容】
来源：http://wu.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sb.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qh.panjiajie.cn

SQL · Bash · C · C++
来源：http://ax.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pw.bookmarksfly.cn

【使用说明】
来源：http://pe.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kk.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tl.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lw.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sz.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jh.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sa.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wq.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ri.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fd.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ec.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ki.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fe.bjjhwx.cn

【文件统计】
来源：http://xx.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ly.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://gh.szsharing.cn

目  录
来源：http://td.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://al.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hm.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nw.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oz.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://is.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ho.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dk.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yf.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mi.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lt.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fm.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://as.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fc.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vs.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cd.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jg.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sp.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oy.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qd.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vu.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wo.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mc.szxytkj.cn

================================================================================
来源：http://kj.hnjuh.cn

A. 基础语法与类型
来源：http://fc.shtwfgs.cn

================================================================================
来源：http://xc.szxytkj.cn

[A01] Hello World
来源：http://me.nszjky.cn

Py:   print("Hello, World!")
来源：http://qj.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://xb.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://pw.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ja.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://yd.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://sf.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://jh.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rq.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://ke.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hl.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jb.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lv.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hj.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://ia.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://tq.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://pe.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rb.jctech888.com.cn

[A03] 常量定义
来源：http://qh.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xw.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://he.nszjky.cn

JS:   const PI = 3.14159;
来源：http://ca.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://jp.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://ct.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ti.9csxet.cn

Ruby: PI = 3.14159
来源：http://ix.colortex.cn

C#:   const double PI = 3.14159;
来源：http://rj.wgjwhj.cn

[A04] 判断变量类型
来源：http://sx.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://go.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ej.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wp.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://ha.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ho.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://on.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ax.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://vh.huanxung.cn

[A05] 整数除法与取模
来源：http://zo.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dj.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wj.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vl.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://we.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://el.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://hq.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://lj.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://ng.hahajie.cn

[A06] 字符串转数字
来源：http://pa.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://lg.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dk.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://td.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xf.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://su.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://li.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mg.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://da.nszjky.cn

[A07] 数字转字符串
来源：http://ad.panjiajie.cn

Py:   str(42)
来源：http://kc.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://fi.9csxet.cn

JS:   String(42); (42).toString()
来源：http://ub.bookmarksfly.cn

TS:   String(42)
来源：http://bs.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ti.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://oc.muxihuayi.cn

Ruby: 42.to_s
来源：http://vh.wgjwhj.cn

C#:   42.ToString()
来源：http://kw.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://pe.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zs.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cx.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mm.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hn.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ip.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zk.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uc.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wk.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://cc.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uo.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cl.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bu.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rn.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wv.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wl.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mj.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fx.yuexingan06.cn

[A10] 生成随机数
来源：http://oy.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://xh.nszjky.cn

PHP:  random_int(1, 100);
来源：http://xn.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://te.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pj.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://vd.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xm.colortex.cn

Ruby: rand(1..100)
来源：http://yx.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://hj.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://kb.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://sh.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ne.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ve.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rd.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://wc.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ob.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pm.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gi.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://tx.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eu.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://er.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://bi.colortex.cn

TS:   `Hello, ${name}!`
来源：http://wk.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://sn.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://um.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://tm.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://rq.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sy.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ns.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://iy.9csxet.cn

JS:   "第一行\n第二行"
来源：http://cm.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://xe.gzmigu.cn

Java: "第一行\n第二行"
来源：http://fy.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://cu.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://fd.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://cs.gzmigu.cn

[A14] 注释写法
来源：http://pu.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ci.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sz.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://yl.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ok.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bo.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://sa.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hm.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://xh.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://zy.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://cv.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://sg.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://zp.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://zs.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nh.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://rm.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://ff.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://vy.hahajie.cn

[A16] 真假值判断规则
来源：http://ey.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xp.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fa.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pc.lnxyls.cn

TS:   if (!x) {}
来源：http://na.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yw.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ln.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mi.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gp.huanxung.cn

[A17] 位运算
来源：http://am.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lh.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pu.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qr.panjiajie.cn


<!-- 参考信息 -->