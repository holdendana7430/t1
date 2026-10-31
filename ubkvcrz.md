代发 wailian999

[U97] JS：并发请求
来源：http://ky.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://rm.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qh.colortex.cn

[U99] JS：事件监听
来源：http://tp.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://xg.nszjky.cn

[U100] JS：DOM 查询
来源：http://kl.521024.cn

document.querySelector(".item")
来源：http://ff.hahajie.cn

[U101] JS：classList 操作
来源：http://bp.shtwfgs.cn

el.classList.toggle("active")
来源：http://sy.shxzskj.cn

[U102] JS：本地存储
来源：http://td.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://or.nicolike.cn

[U103] JS：定时器
来源：http://yh.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ss.hnjuh.cn

[U104] JS：防抖
来源：http://zk.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ba.yuexingan06.cn

[U105] JS：节流
来源：http://yb.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qv.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://tp.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://et.521024.cn

[U107] JS：数字千分位
来源：http://xz.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nb.newstarts.cn

[U108] JS：随机整数
来源：http://yy.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fq.hnjuh.cn

[U109] JS：数组分组
来源：http://bx.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://mw.shtwfgs.cn

[U110] JS：数组分块
来源：http://mi.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lf.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://th.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://sm.newstarts.cn

[U112] JS：字符串补位
来源：http://er.szxytkj.cn

"7".padStart(3, "0")
来源：http://td.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://nv.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://ht.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://hb.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sv.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ut.jianghongdianzi.cn

crypto.randomUUID()
来源：http://uq.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://az.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://fu.panjiajie.cn

[U117] JS：单元测试
来源：http://nf.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://ye.huanxung.cn

[U118] JS：开发服务器
来源：http://nm.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://rf.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://vd.huixiangedu.cn

npx vite build
来源：http://di.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://dx.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://fx.gzmigu.cn

================================================================================
来源：http://wq.newstarts.cn

统计汇总
来源：http://kl.521024.cn

================================================================================
来源：http://ch.asd995.cn

按语言统计（条）：
来源：http://ck.521024.cn

Python ......... 252
来源：http://zw.yuntaijiaju.cn

PHP ............ 252
来源：http://nh.9csxet.cn

JavaScript ..... 252
来源：http://ls.521024.cn

TypeScript ..... 212
来源：http://fo.shtwfgs.cn

Java ........... 212
来源：http://bh.bookmarksfly.cn

Go ............. 212
来源：http://at.szxytkj.cn

Ruby ........... 212
来源：http://hc.chemitech.net.cn

C# ............. 212
来源：http://la.bjjhwx.cn

C .............. 30
来源：http://jd.hahajie.cn

C++ ............ 30
来源：http://my.shtwfgs.cn

SQL ............ 90
来源：http://ff.huixinmuqiang.cn

Bash ........... 80
来源：http://ql.jctech888.com.cn

Kotlin ......... 15
来源：http://xz.colortex.cn

Swift .......... 15
来源：http://zq.szsharing.cn

Lua ............ 10
来源：http://et.hnjuh.cn

Perl ........... 10
来源：http://ca.521024.cn

Scala .......... 10
来源：http://ev.9csxet.cn

------------------------------------
来源：http://dh.panjiajie.cn

合计 ........... 2106 条
来源：http://yg.haigaiapp.cn

按章节统计：
来源：http://pg.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uy.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qi.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gz.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gk.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ne.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xo.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vr.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ko.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ln.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gz.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://te.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vm.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cx.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zj.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qx.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hy.shtwfgs.cn

Q SQL 专题                              90
来源：http://td.huanxung.cn

R Bash 专题                             80
来源：http://jy.yuexingan06.cn

S C / C++ 专题                          60
来源：http://ee.huixiangedu.cn

T 其他语言补充                          60
来源：http://ig.521024.cn

U 高频实用片段                         120
来源：http://ho.nicolike.cn

------------------------------------
来源：http://sm.521024.cn

合计                                  2106 条
来源：http://lq.colortex.cn

--------------------------------------------------------------------------------
来源：http://nt.bjjhwx.cn

使用提醒
来源：http://tn.newstarts.cn

--------------------------------------------------------------------------------
来源：http://fl.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://va.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sc.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pf.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://la.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pn.hnjuh.cn

—— 文件结束 ——
来源：http://lr.shtwfgs.cn

================================================================================
来源：http://uz.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://or.colortex.cn

Common Programming Examples Cheat Book
来源：http://pw.newstarts.cn

================================================================================
来源：http://fd.panjiajie.cn

【收录内容】
来源：http://xx.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gl.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aq.jctech888.com.cn

SQL · Bash · C · C++
来源：http://wc.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ja.shxzskj.cn

【使用说明】
来源：http://uq.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eu.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mj.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hw.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rb.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fy.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uz.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iw.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kw.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pq.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ks.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eo.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zn.huixinmuqiang.cn

【文件统计】
来源：http://pg.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ys.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://tq.9csxet.cn

目  录
来源：http://yl.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://hv.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gy.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wi.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fe.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ie.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tv.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fj.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ej.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uu.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rk.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oy.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wv.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uz.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xq.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ch.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yl.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xd.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fd.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zi.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sb.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hw.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mm.panjiajie.cn

================================================================================
来源：http://wc.colortex.cn

A. 基础语法与类型
来源：http://gb.muxihuayi.cn

================================================================================
来源：http://ke.huixinmuqiang.cn

[A01] Hello World
来源：http://iu.jctech888.com.cn

Py:   print("Hello, World!")
来源：http://go.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://xn.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://hk.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nk.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://un.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://bz.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://la.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xe.gzmigu.cn

[A02] 变量声明与赋值
来源：http://va.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bf.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vh.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wk.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ua.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://pb.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://uf.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://jt.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ll.huixinmuqiang.cn

[A03] 常量定义
来源：http://fq.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vv.asd995.cn

PHP:  const PI = 3.14159;
来源：http://fw.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://or.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://sk.colortex.cn

Java: static final double PI = 3.14159;
来源：http://pk.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://sy.asd995.cn

Ruby: PI = 3.14159
来源：http://ni.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://yq.shtwfgs.cn

[A04] 判断变量类型
来源：http://az.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bd.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://se.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://il.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://uz.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ao.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hw.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tu.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://ws.9csxet.cn

[A05] 整数除法与取模
来源：http://cz.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uu.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://an.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ox.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ez.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://uh.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://nd.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://xt.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://go.muxihuayi.cn

[A06] 字符串转数字
来源：http://yv.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://pz.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xe.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eb.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zj.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rp.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bg.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zp.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fx.hnjuh.cn

[A07] 数字转字符串
来源：http://xw.chemitech.net.cn

Py:   str(42)
来源：http://dr.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://of.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://ix.panjiajie.cn

TS:   String(42)
来源：http://qs.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rf.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://xp.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://js.shxzukj.cn

C#:   42.ToString()
来源：http://ns.huanxung.cn

[A08] 取整与四舍五入
来源：http://vv.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://px.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rk.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://se.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nj.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pm.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dw.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://np.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hv.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://tp.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ki.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ll.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tr.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://me.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zx.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ub.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lp.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nl.nszjky.cn

[A10] 生成随机数
来源：http://pg.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://sr.huanxung.cn

PHP:  random_int(1, 100);
来源：http://yp.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ue.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ku.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://xh.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ff.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://nw.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://mu.szsharing.cn

[A11] 条件表达式（三元）
来源：http://vy.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://fb.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nb.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rt.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nq.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://vj.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qq.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ho.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://db.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://wu.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pp.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://br.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://vu.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://tj.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://df.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rg.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://qy.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://hg.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vi.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://ul.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://jp.szsharing.cn

JS:   "第一行\n第二行"
来源：http://bo.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://vb.nszjky.cn

Java: "第一行\n第二行"
来源：http://jl.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ws.521024.cn

Ruby: "第一行\n第二行"
来源：http://hw.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://sc.huixinmuqiang.cn

[A14] 注释写法
来源：http://qy.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jd.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oi.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://mr.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://mj.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xk.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://pf.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tx.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://iz.shxzskj.cn

[A15] 空值判断与默认值
来源：http://ou.szsharing.cn

Py:   value = data or "默认值"
来源：http://qy.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://tp.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://wg.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://ub.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cn.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://un.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://rm.521024.cn

C#:   var value = data ?? "默认值";
来源：http://th.asd995.cn

[A16] 真假值判断规则
来源：http://mh.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ln.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sh.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ae.shxzukj.cn

TS:   if (!x) {}
来源：http://hw.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jn.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qj.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zn.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xa.gzmigu.cn

[A17] 位运算
来源：http://oj.shtwfgs.cn


<!-- 参考信息 -->