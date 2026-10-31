代发 wailian999

[U95] JS：Promise 包装
来源：http://vc.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://nl.9csxet.cn

[U96] JS：async/await 与异常
来源：http://hk.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oc.gzmigu.cn

[U97] JS：并发请求
来源：http://si.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kk.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://qr.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vi.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://uj.nszjky.cn

el.addEventListener("click", e => {})
来源：http://sw.colortex.cn

[U100] JS：DOM 查询
来源：http://rk.panjiajie.cn

document.querySelector(".item")
来源：http://bq.chemitech.net.cn

[U101] JS：classList 操作
来源：http://qr.yuexingan06.cn

el.classList.toggle("active")
来源：http://xc.chemitech.net.cn

[U102] JS：本地存储
来源：http://xd.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sg.szxytkj.cn

[U103] JS：定时器
来源：http://ty.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tv.shxzukj.cn

[U104] JS：防抖
来源：http://st.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.haigaiapp.cn

[U105] JS：节流
来源：http://nu.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fa.nszjky.cn

[U106] JS：日期格式化
来源：http://xb.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oh.gzmigu.cn

[U107] JS：数字千分位
来源：http://ew.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.asd995.cn

[U108] JS：随机整数
来源：http://da.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gj.huanxung.cn

[U109] JS：数组分组
来源：http://qx.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://sg.shtwfgs.cn

[U110] JS：数组分块
来源：http://ot.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ic.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://lj.shxzskj.cn

new Map(Object.entries(obj))
来源：http://df.jctech888.com.cn

[U112] JS：字符串补位
来源：http://nw.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://oz.szsharing.cn

[U113] JS：正则替换全部
来源：http://gr.nszjky.cn

s.replaceAll("a", "b")
来源：http://pb.nicolike.cn

[U114] JS：JSON 深比较
来源：http://av.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yh.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://cu.colortex.cn

crypto.randomUUID()
来源：http://hm.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://yd.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://us.shxzskj.cn

[U117] JS：单元测试
来源：http://hj.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://pg.521024.cn

[U118] JS：开发服务器
来源：http://sn.nszjky.cn

npm i -D vite;  npx vite
来源：http://dx.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://nl.521024.cn

npx vite build
来源：http://lb.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://eb.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://oz.wgjwhj.cn

统计汇总
来源：http://pq.szxytkj.cn

================================================================================
来源：http://cg.asd995.cn

按语言统计（条）：
来源：http://ye.huanxung.cn

Python ......... 252
来源：http://ac.chemitech.net.cn

PHP ............ 252
来源：http://mo.521024.cn

JavaScript ..... 252
来源：http://la.colortex.cn

TypeScript ..... 212
来源：http://xd.521024.cn

Java ........... 212
来源：http://mg.hnjuh.cn

Go ............. 212
来源：http://rm.haigaiapp.cn

Ruby ........... 212
来源：http://fg.huixiangedu.cn

C# ............. 212
来源：http://tv.gzmigu.cn

C .............. 30
来源：http://se.huanxung.cn

C++ ............ 30
来源：http://cp.szsharing.cn

SQL ............ 90
来源：http://dl.shxzukj.cn

Bash ........... 80
来源：http://ey.chemitech.net.cn

Kotlin ......... 15
来源：http://dj.hahajie.cn

Swift .......... 15
来源：http://gl.colortex.cn

Lua ............ 10
来源：http://me.jctech888.com.cn

Perl ........... 10
来源：http://iv.jianghongdianzi.cn

Scala .......... 10
来源：http://xe.yuntaijiaju.cn

------------------------------------
来源：http://jb.521024.cn

合计 ........... 2106 条
来源：http://sj.hahajie.cn

按章节统计：
来源：http://iu.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cx.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ql.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sx.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yu.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lg.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lx.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lc.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gc.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wf.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ti.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://no.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kr.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pf.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yb.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qm.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fh.lnxyls.cn

Q SQL 专题                              90
来源：http://au.asd995.cn

R Bash 专题                             80
来源：http://hn.panjiajie.cn

S C / C++ 专题                          60
来源：http://kt.wgjwhj.cn

T 其他语言补充                          60
来源：http://vk.huixiangedu.cn

U 高频实用片段                         120
来源：http://bd.9csxet.cn

------------------------------------
来源：http://tn.haigaiapp.cn

合计                                  2106 条
来源：http://ai.newstarts.cn

--------------------------------------------------------------------------------
来源：http://cu.jianghongdianzi.cn

使用提醒
来源：http://zi.521024.cn

--------------------------------------------------------------------------------
来源：http://dh.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jw.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uw.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mo.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qg.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dr.gzmigu.cn

—— 文件结束 ——
来源：http://fy.haigaiapp.cn

================================================================================
来源：http://oc.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://xm.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://wo.521024.cn

================================================================================
来源：http://qf.huixiangedu.cn

【收录内容】
来源：http://rx.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ye.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nb.chemitech.net.cn

SQL · Bash · C · C++
来源：http://mq.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xh.gzmigu.cn

【使用说明】
来源：http://un.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pm.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://st.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ca.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tl.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hf.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vz.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tg.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bq.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ud.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wi.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dk.bookmarksfly.cn

【文件统计】
来源：http://di.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gm.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://sn.hnjuh.cn

目  录
来源：http://ry.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ol.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rv.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gu.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ds.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fk.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vc.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vh.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ue.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hd.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rr.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tn.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wp.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ob.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vf.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ta.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bt.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cm.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cc.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://he.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ip.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fw.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jq.huixinmuqiang.cn

================================================================================
来源：http://ua.9csxet.cn

A. 基础语法与类型
来源：http://lu.nicolike.cn

================================================================================
来源：http://ly.gzmigu.cn

[A01] Hello World
来源：http://fj.shxzukj.cn

Py:   print("Hello, World!")
来源：http://de.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://rv.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://ri.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oj.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://no.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://eb.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://rf.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wn.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://ls.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fj.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ni.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cc.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://og.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://ki.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://xs.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://sr.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ga.chemitech.net.cn

[A03] 常量定义
来源：http://nh.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://te.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://wv.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://qp.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://no.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://rm.nicolike.cn

Go:   const PI = 3.14159
来源：http://qm.panjiajie.cn

Ruby: PI = 3.14159
来源：http://nk.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://oy.nicolike.cn

[A04] 判断变量类型
来源：http://cb.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://re.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mv.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ls.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://lx.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zl.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dn.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xt.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://yo.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://qm.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gn.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ci.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qo.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nx.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://uo.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://ti.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://nu.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://bo.bookmarksfly.cn

[A06] 字符串转数字
来源：http://rz.521024.cn

Py:   int("42"); float("3.14")
来源：http://xt.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xb.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xo.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://md.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jz.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tz.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ch.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hl.gzmigu.cn

[A07] 数字转字符串
来源：http://bz.asd995.cn

Py:   str(42)
来源：http://lf.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://bk.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://qi.9csxet.cn

TS:   String(42)
来源：http://cs.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ab.colortex.cn

Go:   strconv.Itoa(42)
来源：http://ke.huixiangedu.cn

Ruby: 42.to_s
来源：http://zi.shtwfgs.cn

C#:   42.ToString()
来源：http://oa.hnjuh.cn

[A08] 取整与四舍五入
来源：http://xb.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uh.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mm.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wq.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gc.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pg.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ii.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gd.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ui.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://cq.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nm.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://li.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dl.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gk.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zj.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xr.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iy.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yy.szxytkj.cn

[A10] 生成随机数
来源：http://sb.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://bq.szsharing.cn

PHP:  random_int(1, 100);
来源：http://cd.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jz.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rz.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://qa.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lq.haigaiapp.cn

Ruby: rand(1..100)
来源：http://hh.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://vo.nszjky.cn

[A11] 条件表达式（三元）
来源：http://ea.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://cn.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pc.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nz.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gk.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://tu.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wv.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lq.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bz.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://bw.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gy.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ss.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://hy.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://cf.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://bq.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kp.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://vi.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://ut.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://km.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://na.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://rp.newstarts.cn

JS:   "第一行\n第二行"
来源：http://us.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://zd.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://ft.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://rs.521024.cn

Ruby: "第一行\n第二行"
来源：http://gk.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://jo.shxzskj.cn

[A14] 注释写法
来源：http://jk.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yp.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yp.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ba.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://xk.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://if.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://rk.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vg.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://tb.lnxyls.cn

[A15] 空值判断与默认值
来源：http://ep.szxytkj.cn

Py:   value = data or "默认值"
来源：http://xh.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://vw.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://jc.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://el.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uf.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://wf.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://bm.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://ms.newstarts.cn

[A16] 真假值判断规则
来源：http://wk.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yb.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qa.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xm.bookmarksfly.cn

TS:   if (!x) {}
来源：http://ab.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qw.huixinmuqiang.cn


<!-- 参考信息 -->