代发 wailian999

[U93] JS：模板字符串
来源：http://cn.haigaiapp.cn

`共 ${n} 条`
来源：http://hy.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://wp.bookmarksfly.cn

const double = x => x * 2;
来源：http://ta.shxzukj.cn

[U95] JS：Promise 包装
来源：http://jv.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://sq.521024.cn

[U96] JS：async/await 与异常
来源：http://dy.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://as.9csxet.cn

[U97] JS：并发请求
来源：http://yd.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ab.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wi.asd995.cn

[U99] JS：事件监听
来源：http://hf.hahajie.cn

el.addEventListener("click", e => {})
来源：http://mf.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://wr.szsharing.cn

document.querySelector(".item")
来源：http://qd.muxihuayi.cn

[U101] JS：classList 操作
来源：http://jr.hahajie.cn

el.classList.toggle("active")
来源：http://es.9csxet.cn

[U102] JS：本地存储
来源：http://iq.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wn.9csxet.cn

[U103] JS：定时器
来源：http://uh.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xs.newstarts.cn

[U104] JS：防抖
来源：http://kh.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ky.newstarts.cn

[U105] JS：节流
来源：http://ub.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uk.521024.cn

[U106] JS：日期格式化
来源：http://qq.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yj.szsharing.cn

[U107] JS：数字千分位
来源：http://xo.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ym.haigaiapp.cn

[U108] JS：随机整数
来源：http://ke.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ji.huixiangedu.cn

[U109] JS：数组分组
来源：http://wf.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://iq.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://ld.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rb.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://dp.gzmigu.cn

new Map(Object.entries(obj))
来源：http://nw.newstarts.cn

[U112] JS：字符串补位
来源：http://sh.hnjuh.cn

"7".padStart(3, "0")
来源：http://wu.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://mb.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://my.asd995.cn

[U114] JS：JSON 深比较
来源：http://cl.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cm.szxytkj.cn

[U115] JS：生成 UUID
来源：http://go.shxzskj.cn

crypto.randomUUID()
来源：http://nw.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://ng.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://et.gzmigu.cn

[U117] JS：单元测试
来源：http://xn.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://gd.colortex.cn

[U118] JS：开发服务器
来源：http://pu.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://bk.szsharing.cn

[U119] JS：生产构建
来源：http://fx.chemitech.net.cn

npx vite build
来源：http://hn.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://wy.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ui.hahajie.cn

================================================================================
来源：http://jf.asd995.cn

统计汇总
来源：http://lg.colortex.cn

================================================================================
来源：http://ez.yuexingan06.cn

按语言统计（条）：
来源：http://ye.lnxyls.cn

Python ......... 252
来源：http://qn.jctech888.com.cn

PHP ............ 252
来源：http://gc.shxzukj.cn

JavaScript ..... 252
来源：http://og.shxzukj.cn

TypeScript ..... 212
来源：http://hk.wgjwhj.cn

Java ........... 212
来源：http://ge.wgjwhj.cn

Go ............. 212
来源：http://uq.shtwfgs.cn

Ruby ........... 212
来源：http://oy.asd995.cn

C# ............. 212
来源：http://ml.wgjwhj.cn

C .............. 30
来源：http://mx.newstarts.cn

C++ ............ 30
来源：http://mi.wgjwhj.cn

SQL ............ 90
来源：http://ye.jctech888.com.cn

Bash ........... 80
来源：http://js.huixinmuqiang.cn

Kotlin ......... 15
来源：http://wh.colortex.cn

Swift .......... 15
来源：http://pp.szsharing.cn

Lua ............ 10
来源：http://in.bookmarksfly.cn

Perl ........... 10
来源：http://cu.chemitech.net.cn

Scala .......... 10
来源：http://tk.haigaiapp.cn

------------------------------------
来源：http://bj.szxytkj.cn

合计 ........... 2106 条
来源：http://rm.asd995.cn

按章节统计：
来源：http://xs.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jb.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ds.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qh.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://de.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yp.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ao.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cp.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ud.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eo.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qu.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yf.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zn.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dq.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ep.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jl.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uq.shtwfgs.cn

Q SQL 专题                              90
来源：http://hk.wgjwhj.cn

R Bash 专题                             80
来源：http://cf.gzmigu.cn

S C / C++ 专题                          60
来源：http://ak.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://gz.huanxung.cn

U 高频实用片段                         120
来源：http://ii.muxihuayi.cn

------------------------------------
来源：http://rz.muxihuayi.cn

合计                                  2106 条
来源：http://ys.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://le.huixinmuqiang.cn

使用提醒
来源：http://mh.colortex.cn

--------------------------------------------------------------------------------
来源：http://qq.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://el.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://by.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ju.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kj.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sa.huixinmuqiang.cn

—— 文件结束 ——
来源：http://cg.muxihuayi.cn

================================================================================
来源：http://ms.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://vy.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://hl.gzmigu.cn

================================================================================
来源：http://cv.gzmigu.cn

【收录内容】
来源：http://fz.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ce.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://of.9csxet.cn

SQL · Bash · C · C++
来源：http://hu.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cj.bjjhwx.cn

【使用说明】
来源：http://pd.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dw.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ih.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gr.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yt.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://up.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ip.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://st.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ep.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ng.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pb.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fd.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mg.asd995.cn

【文件统计】
来源：http://qb.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qj.colortex.cn

--------------------------------------------------------------------------------
来源：http://us.lnxyls.cn

目  录
来源：http://va.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://fi.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vc.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://la.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yu.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hu.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tn.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ib.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://la.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wm.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fk.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tr.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pu.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dv.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cg.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jd.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tz.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dh.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oh.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ar.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gm.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dw.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lh.szsharing.cn

================================================================================
来源：http://wy.bjjhwx.cn

A. 基础语法与类型
来源：http://bc.yuexingan06.cn

================================================================================
来源：http://zk.gzmigu.cn

[A01] Hello World
来源：http://ub.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://oz.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://jj.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://xz.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wy.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://vr.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://mh.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://nn.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ky.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://tg.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xp.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://un.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uz.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ky.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://tq.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://eo.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://kl.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rm.hahajie.cn

[A03] 常量定义
来源：http://dm.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gd.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://as.nszjky.cn

JS:   const PI = 3.14159;
来源：http://tp.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://cs.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://uo.shxzukj.cn

Go:   const PI = 3.14159
来源：http://an.nszjky.cn

Ruby: PI = 3.14159
来源：http://ab.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://fh.szsharing.cn

[A04] 判断变量类型
来源：http://zt.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ka.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cx.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vx.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://du.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tm.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zc.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kk.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://wn.gzmigu.cn

[A05] 整数除法与取模
来源：http://kx.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fx.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uo.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yu.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sk.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://dv.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://oi.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://up.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://xr.lnxyls.cn

[A06] 字符串转数字
来源：http://nw.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://ee.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gi.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ie.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jb.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tw.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ad.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ec.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xk.shxzskj.cn

[A07] 数字转字符串
来源：http://jb.asd995.cn

Py:   str(42)
来源：http://ki.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://hk.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://wi.jianghongdianzi.cn

TS:   String(42)
来源：http://od.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ou.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://at.bookmarksfly.cn

Ruby: 42.to_s
来源：http://hy.shxzukj.cn

C#:   42.ToString()
来源：http://mu.szxytkj.cn

[A08] 取整与四舍五入
来源：http://nw.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nq.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xe.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lw.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ml.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fv.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lz.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pu.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kc.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://rg.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zg.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qf.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sa.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fi.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kd.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kb.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qb.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tc.haigaiapp.cn

[A10] 生成随机数
来源：http://bf.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://hp.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://sw.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://en.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mu.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://pb.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cf.hahajie.cn

Ruby: rand(1..100)
来源：http://hz.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://da.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://om.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://lo.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xy.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qi.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jj.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://vb.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cd.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qh.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sd.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://hr.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nk.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vq.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://rm.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://dv.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://gz.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ms.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://fs.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://jn.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ov.colortex.cn

Py:   "第一行\n第二行"
来源：http://db.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://ey.newstarts.cn

JS:   "第一行\n第二行"
来源：http://xv.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://lb.9csxet.cn

Java: "第一行\n第二行"
来源：http://kc.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://wh.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://tc.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://bi.huixiangedu.cn

[A14] 注释写法
来源：http://hk.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://we.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ry.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://fq.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://bt.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gs.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://zw.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qo.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://vp.newstarts.cn

[A15] 空值判断与默认值
来源：http://ge.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://wi.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://yl.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://dk.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://yh.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qn.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://je.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://nr.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://rg.asd995.cn

[A16] 真假值判断规则
来源：http://bk.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bd.colortex.cn


<!-- 参考信息 -->