代发 wailian999

[U95] JS：Promise 包装
来源：http://dp.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://tw.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://xi.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://on.bjjhwx.cn

[U97] JS：并发请求
来源：http://ih.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lx.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://ab.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tl.lnxyls.cn

[U99] JS：事件监听
来源：http://ja.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://gv.nszjky.cn

[U100] JS：DOM 查询
来源：http://jn.gzmigu.cn

document.querySelector(".item")
来源：http://xr.newstarts.cn

[U101] JS：classList 操作
来源：http://bc.newstarts.cn

el.classList.toggle("active")
来源：http://be.szsharing.cn

[U102] JS：本地存储
来源：http://bd.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ay.lnxyls.cn

[U103] JS：定时器
来源：http://zz.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://on.shxzukj.cn

[U104] JS：防抖
来源：http://nd.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mw.szsharing.cn

[U105] JS：节流
来源：http://du.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ou.huanxung.cn

[U106] JS：日期格式化
来源：http://sg.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zd.hnjuh.cn

[U107] JS：数字千分位
来源：http://vk.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gq.yuexingan06.cn

[U108] JS：随机整数
来源：http://oz.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yw.yuexingan06.cn

[U109] JS：数组分组
来源：http://yl.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://rv.huanxung.cn

[U110] JS：数组分块
来源：http://rg.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xe.nicolike.cn

[U111] JS：对象转 Map
来源：http://og.9csxet.cn

new Map(Object.entries(obj))
来源：http://lb.jctech888.com.cn

[U112] JS：字符串补位
来源：http://tb.shxzskj.cn

"7".padStart(3, "0")
来源：http://ch.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://pl.shxzskj.cn

s.replaceAll("a", "b")
来源：http://ht.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://pg.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ey.newstarts.cn

[U115] JS：生成 UUID
来源：http://ty.yuntaijiaju.cn

crypto.randomUUID()
来源：http://ow.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://dw.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://ws.shtwfgs.cn

[U117] JS：单元测试
来源：http://ha.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://kd.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://sy.huanxung.cn

npm i -D vite;  npx vite
来源：http://tr.chemitech.net.cn

[U119] JS：生产构建
来源：http://bv.colortex.cn

npx vite build
来源：http://nj.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://pz.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ax.jianghongdianzi.cn

================================================================================
来源：http://ws.nicolike.cn

统计汇总
来源：http://bt.jctech888.com.cn

================================================================================
来源：http://ad.jianghongdianzi.cn

按语言统计（条）：
来源：http://ll.colortex.cn

Python ......... 252
来源：http://fw.jctech888.com.cn

PHP ............ 252
来源：http://bv.gzmigu.cn

JavaScript ..... 252
来源：http://hv.shtwfgs.cn

TypeScript ..... 212
来源：http://ar.gzmigu.cn

Java ........... 212
来源：http://zw.lnxyls.cn

Go ............. 212
来源：http://oc.newstarts.cn

Ruby ........... 212
来源：http://mi.wgjwhj.cn

C# ............. 212
来源：http://il.nszjky.cn

C .............. 30
来源：http://tt.lnxyls.cn

C++ ............ 30
来源：http://iz.shxzukj.cn

SQL ............ 90
来源：http://qn.shtwfgs.cn

Bash ........... 80
来源：http://io.jctech888.com.cn

Kotlin ......... 15
来源：http://np.chemitech.net.cn

Swift .......... 15
来源：http://jx.bookmarksfly.cn

Lua ............ 10
来源：http://en.nicolike.cn

Perl ........... 10
来源：http://yj.hnjuh.cn

Scala .......... 10
来源：http://gq.newstarts.cn

------------------------------------
来源：http://qc.hahajie.cn

合计 ........... 2106 条
来源：http://pi.huanxung.cn

按章节统计：
来源：http://bd.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mw.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jb.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rn.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dq.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aw.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xo.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yr.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wn.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lu.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bj.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ee.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://im.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tf.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qx.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cf.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ip.bookmarksfly.cn

Q SQL 专题                              90
来源：http://xj.muxihuayi.cn

R Bash 专题                             80
来源：http://ke.szsharing.cn

S C / C++ 专题                          60
来源：http://ce.yuexingan06.cn

T 其他语言补充                          60
来源：http://vz.bookmarksfly.cn

U 高频实用片段                         120
来源：http://mt.szxytkj.cn

------------------------------------
来源：http://gz.hnjuh.cn

合计                                  2106 条
来源：http://lf.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ft.huanxung.cn

使用提醒
来源：http://du.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://oi.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://he.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tq.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xr.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mo.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xm.shxzukj.cn

—— 文件结束 ——
来源：http://it.szsharing.cn

================================================================================
来源：http://no.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://tx.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://gw.huixiangedu.cn

================================================================================
来源：http://tr.haigaiapp.cn

【收录内容】
来源：http://eb.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dc.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://na.9csxet.cn

SQL · Bash · C · C++
来源：http://gd.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jd.hahajie.cn

【使用说明】
来源：http://rw.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bf.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nt.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mo.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jh.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wy.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lh.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ye.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qc.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zm.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nr.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pa.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://va.newstarts.cn

【文件统计】
来源：http://pz.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ue.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xs.jianghongdianzi.cn

目  录
来源：http://az.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zc.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zm.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gn.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lf.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ro.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ro.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wq.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://th.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wp.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cv.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ll.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://us.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://au.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yk.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cx.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ro.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nd.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ve.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vf.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sy.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://um.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fm.yuntaijiaju.cn

================================================================================
来源：http://tg.muxihuayi.cn

A. 基础语法与类型
来源：http://fs.hnjuh.cn

================================================================================
来源：http://jl.bookmarksfly.cn

[A01] Hello World
来源：http://yx.shxzukj.cn

Py:   print("Hello, World!")
来源：http://nb.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://vr.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://hi.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pg.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://hs.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://gj.hahajie.cn

Ruby: puts "Hello, World!"
来源：http://st.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hb.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://ko.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lg.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dq.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vp.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ep.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://qp.521024.cn

Go:   name := "Alex"; age := 20
来源：http://bx.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://nn.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kc.chemitech.net.cn

[A03] 常量定义
来源：http://pw.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rf.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://nl.szsharing.cn

JS:   const PI = 3.14159;
来源：http://un.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://sq.colortex.cn

Java: static final double PI = 3.14159;
来源：http://mh.hnjuh.cn

Go:   const PI = 3.14159
来源：http://ss.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://cf.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://pf.521024.cn

[A04] 判断变量类型
来源：http://zd.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fr.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rg.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wp.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://is.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bf.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qg.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jy.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://pd.hahajie.cn

[A05] 整数除法与取模
来源：http://gj.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ld.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ab.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sb.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ic.521024.cn

Java: 7 / 2; 7 % 2
来源：http://sc.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://xo.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://ww.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://wk.shxzukj.cn

[A06] 字符串转数字
来源：http://pr.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://ta.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nq.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ki.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mm.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hj.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qe.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jx.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iw.huanxung.cn

[A07] 数字转字符串
来源：http://fu.hahajie.cn

Py:   str(42)
来源：http://xa.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://ry.colortex.cn

JS:   String(42); (42).toString()
来源：http://qq.jctech888.com.cn

TS:   String(42)
来源：http://tw.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tx.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://pg.shxzskj.cn

Ruby: 42.to_s
来源：http://we.szsharing.cn

C#:   42.ToString()
来源：http://mj.9csxet.cn

[A08] 取整与四舍五入
来源：http://tn.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://to.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kb.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eu.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cy.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gc.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nx.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jr.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dc.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://eh.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jb.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hl.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tj.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pk.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ai.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://st.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qm.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ug.szxytkj.cn

[A10] 生成随机数
来源：http://vv.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://hz.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://yt.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jz.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kx.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://ga.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rj.newstarts.cn

Ruby: rand(1..100)
来源：http://pm.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://bt.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://br.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ze.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jn.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rn.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zx.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ie.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ts.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bt.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ld.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://jb.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bj.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uq.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://uf.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://wb.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://at.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://em.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://cj.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://hs.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ja.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://st.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://dn.nicolike.cn

JS:   "第一行\n第二行"
来源：http://mp.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://qf.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://gx.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ft.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://io.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ot.huixiangedu.cn

[A14] 注释写法
来源：http://mp.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://my.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://up.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://jl.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ks.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fm.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://ie.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kf.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://tt.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://qs.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://ks.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://xw.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://ot.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://vk.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sq.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ls.9csxet.cn

Ruby: value = data || "默认值"
来源：http://ek.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://bs.szxytkj.cn

[A16] 真假值判断规则
来源：http://nz.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cu.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://km.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kg.haigaiapp.cn

TS:   if (!x) {}
来源：http://wa.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wq.jianghongdianzi.cn


<!-- 参考信息 -->