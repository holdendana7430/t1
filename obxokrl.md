代发 wailian999

[U95] JS：Promise 包装
来源：http://to.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://zr.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://oa.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qy.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://nt.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yb.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://lq.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zq.szxytkj.cn

[U99] JS：事件监听
来源：http://hz.asd995.cn

el.addEventListener("click", e => {})
来源：http://fq.panjiajie.cn

[U100] JS：DOM 查询
来源：http://rj.521024.cn

document.querySelector(".item")
来源：http://te.nicolike.cn

[U101] JS：classList 操作
来源：http://mc.chemitech.net.cn

el.classList.toggle("active")
来源：http://bk.huixiangedu.cn

[U102] JS：本地存储
来源：http://yo.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hi.muxihuayi.cn

[U103] JS：定时器
来源：http://er.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zf.chemitech.net.cn

[U104] JS：防抖
来源：http://cu.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ec.huanxung.cn

[U105] JS：节流
来源：http://ab.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://my.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://gv.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dh.szxytkj.cn

[U107] JS：数字千分位
来源：http://bi.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vh.yuexingan06.cn

[U108] JS：随机整数
来源：http://be.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qw.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://qt.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://uc.shxzukj.cn

[U110] JS：数组分块
来源：http://go.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kh.huanxung.cn

[U111] JS：对象转 Map
来源：http://ko.huanxung.cn

new Map(Object.entries(obj))
来源：http://ko.chemitech.net.cn

[U112] JS：字符串补位
来源：http://jn.hahajie.cn

"7".padStart(3, "0")
来源：http://rg.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://qm.gzmigu.cn

s.replaceAll("a", "b")
来源：http://br.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://zw.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jb.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://qf.wgjwhj.cn

crypto.randomUUID()
来源：http://av.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://te.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://fh.yuexingan06.cn

[U117] JS：单元测试
来源：http://zv.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://ce.yuexingan06.cn

[U118] JS：开发服务器
来源：http://sp.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://lc.bjjhwx.cn

[U119] JS：生产构建
来源：http://eo.wgjwhj.cn

npx vite build
来源：http://tc.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://kw.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://zk.521024.cn

================================================================================
来源：http://ho.shxzukj.cn

统计汇总
来源：http://fv.huixiangedu.cn

================================================================================
来源：http://cg.jianghongdianzi.cn

按语言统计（条）：
来源：http://mt.yuexingan06.cn

Python ......... 252
来源：http://os.yuntaijiaju.cn

PHP ............ 252
来源：http://zj.shxzukj.cn

JavaScript ..... 252
来源：http://gk.yuexingan06.cn

TypeScript ..... 212
来源：http://iw.haigaiapp.cn

Java ........... 212
来源：http://gv.yuexingan06.cn

Go ............. 212
来源：http://jo.chemitech.net.cn

Ruby ........... 212
来源：http://wi.panjiajie.cn

C# ............. 212
来源：http://mf.colortex.cn

C .............. 30
来源：http://ho.hnjuh.cn

C++ ............ 30
来源：http://ca.521024.cn

SQL ............ 90
来源：http://si.huixiangedu.cn

Bash ........... 80
来源：http://eu.nicolike.cn

Kotlin ......... 15
来源：http://br.521024.cn

Swift .......... 15
来源：http://uk.yuexingan06.cn

Lua ............ 10
来源：http://de.shxzukj.cn

Perl ........... 10
来源：http://jd.muxihuayi.cn

Scala .......... 10
来源：http://th.chemitech.net.cn

------------------------------------
来源：http://my.haigaiapp.cn

合计 ........... 2106 条
来源：http://lu.9csxet.cn

按章节统计：
来源：http://ho.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kn.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nv.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://us.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sq.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vq.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mn.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nb.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qh.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xu.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yn.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qv.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gx.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lh.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gq.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ta.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://as.shtwfgs.cn

Q SQL 专题                              90
来源：http://vb.huixinmuqiang.cn

R Bash 专题                             80
来源：http://ot.shxzskj.cn

S C / C++ 专题                          60
来源：http://dr.hnjuh.cn

T 其他语言补充                          60
来源：http://oa.bjjhwx.cn

U 高频实用片段                         120
来源：http://bn.nicolike.cn

------------------------------------
来源：http://ph.lnxyls.cn

合计                                  2106 条
来源：http://hm.newstarts.cn

--------------------------------------------------------------------------------
来源：http://dp.huixinmuqiang.cn

使用提醒
来源：http://jj.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://bb.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sj.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vj.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cm.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ri.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sj.huanxung.cn

—— 文件结束 ——
来源：http://vx.nicolike.cn

================================================================================
来源：http://eq.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://pq.nicolike.cn

Common Programming Examples Cheat Book
来源：http://xv.shxzukj.cn

================================================================================
来源：http://vu.nicolike.cn

【收录内容】
来源：http://uo.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://to.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rs.bjjhwx.cn

SQL · Bash · C · C++
来源：http://pw.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://om.szxytkj.cn

【使用说明】
来源：http://cf.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fn.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://io.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bx.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gn.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pw.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ng.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qz.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vw.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nc.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ua.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ro.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sj.haigaiapp.cn

【文件统计】
来源：http://be.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ac.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://sw.jianghongdianzi.cn

目  录
来源：http://ps.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://nk.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gw.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rr.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xx.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cl.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oz.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tl.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qu.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ai.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rf.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fn.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eq.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gm.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yo.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bz.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://al.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ob.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gh.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bh.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sd.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fr.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lh.521024.cn

================================================================================
来源：http://ap.9csxet.cn

A. 基础语法与类型
来源：http://wf.szsharing.cn

================================================================================
来源：http://im.szxytkj.cn

[A01] Hello World
来源：http://di.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://tm.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://nq.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://ys.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ws.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://kv.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://od.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://kh.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wi.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://pc.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ud.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hp.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ae.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gz.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://gg.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://fm.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://kt.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lb.colortex.cn

[A03] 常量定义
来源：http://yr.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lg.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://ky.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://fz.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://ao.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://qc.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://kf.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://xu.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://cp.huixiangedu.cn

[A04] 判断变量类型
来源：http://wy.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tr.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mt.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xd.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://jw.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lc.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rj.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gh.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://qu.521024.cn

[A05] 整数除法与取模
来源：http://sf.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zq.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fx.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nz.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sx.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://fw.521024.cn

Go:   7 / 2; 7 % 2
来源：http://mu.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://jk.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://kn.gzmigu.cn

[A06] 字符串转数字
来源：http://bn.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://if.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zt.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pl.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dn.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rj.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ut.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ry.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bh.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://gc.lnxyls.cn

Py:   str(42)
来源：http://au.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://in.newstarts.cn

JS:   String(42); (42).toString()
来源：http://bo.jctech888.com.cn

TS:   String(42)
来源：http://ri.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kh.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://ye.yuexingan06.cn

Ruby: 42.to_s
来源：http://sd.wgjwhj.cn

C#:   42.ToString()
来源：http://tm.nicolike.cn

[A08] 取整与四舍五入
来源：http://qs.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ln.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ty.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qd.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ii.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pu.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://so.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wt.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kw.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://qp.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://df.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ih.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tz.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ty.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hj.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qs.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wz.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dl.gzmigu.cn

[A10] 生成随机数
来源：http://xt.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://uq.huanxung.cn

PHP:  random_int(1, 100);
来源：http://gy.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jr.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uq.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://ya.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vo.shxzskj.cn

Ruby: rand(1..100)
来源：http://lp.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://rg.newstarts.cn

[A11] 条件表达式（三元）
来源：http://pn.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://jr.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mp.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dl.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uo.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://ej.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wr.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dw.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ft.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://xv.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pq.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jl.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://uy.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://ft.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ol.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xo.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://mn.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://al.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://td.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://er.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://ih.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://wh.colortex.cn

TS:   "第一行\n第二行"
来源：http://sf.huanxung.cn

Java: "第一行\n第二行"
来源：http://qn.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://cj.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://xe.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://av.9csxet.cn

[A14] 注释写法
来源：http://dt.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mu.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fu.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://fd.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://wj.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bc.521024.cn

Go:   // 单行；/* 多行 */
来源：http://lm.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mo.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://yq.asd995.cn

[A15] 空值判断与默认值
来源：http://yb.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://ft.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://hg.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://fb.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ml.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bw.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://bt.nicolike.cn

Ruby: value = data || "默认值"
来源：http://bw.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://gz.shtwfgs.cn

[A16] 真假值判断规则
来源：http://ju.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ob.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://al.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://al.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://sm.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://va.jianghongdianzi.cn


<!-- 参考信息 -->