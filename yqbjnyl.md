代发 wailian999

[U97] JS：并发请求
来源：http://ma.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kc.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://pr.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pf.szxytkj.cn

[U99] JS：事件监听
来源：http://sx.hahajie.cn

el.addEventListener("click", e => {})
来源：http://yt.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://ag.muxihuayi.cn

document.querySelector(".item")
来源：http://gp.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://dl.panjiajie.cn

el.classList.toggle("active")
来源：http://og.huanxung.cn

[U102] JS：本地存储
来源：http://hv.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rx.nszjky.cn

[U103] JS：定时器
来源：http://yr.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nk.lnxyls.cn

[U104] JS：防抖
来源：http://ug.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gj.colortex.cn

[U105] JS：节流
来源：http://xg.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nz.9csxet.cn

[U106] JS：日期格式化
来源：http://zp.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lo.hnjuh.cn

[U107] JS：数字千分位
来源：http://ga.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ux.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://sr.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pt.huanxung.cn

[U109] JS：数组分组
来源：http://kp.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://tz.yuexingan06.cn

[U110] JS：数组分块
来源：http://eu.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kg.9csxet.cn

[U111] JS：对象转 Map
来源：http://uw.lnxyls.cn

new Map(Object.entries(obj))
来源：http://it.chemitech.net.cn

[U112] JS：字符串补位
来源：http://vb.shxzukj.cn

"7".padStart(3, "0")
来源：http://kv.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://kd.huanxung.cn

s.replaceAll("a", "b")
来源：http://mk.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://qg.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mt.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://vu.nicolike.cn

crypto.randomUUID()
来源：http://pz.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://ft.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://og.szxytkj.cn

[U117] JS：单元测试
来源：http://kf.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://bw.jctech888.com.cn

[U118] JS：开发服务器
来源：http://yn.521024.cn

npm i -D vite;  npx vite
来源：http://vf.jctech888.com.cn

[U119] JS：生产构建
来源：http://ym.9csxet.cn

npx vite build
来源：http://sf.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://pc.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://sd.hahajie.cn

================================================================================
来源：http://cg.shtwfgs.cn

统计汇总
来源：http://vq.gzmigu.cn

================================================================================
来源：http://ps.bookmarksfly.cn

按语言统计（条）：
来源：http://cu.bookmarksfly.cn

Python ......... 252
来源：http://lg.chemitech.net.cn

PHP ............ 252
来源：http://lq.huixiangedu.cn

JavaScript ..... 252
来源：http://so.yuntaijiaju.cn

TypeScript ..... 212
来源：http://qh.yuexingan06.cn

Java ........... 212
来源：http://fx.lnxyls.cn

Go ............. 212
来源：http://tm.huixiangedu.cn

Ruby ........... 212
来源：http://zt.jctech888.com.cn

C# ............. 212
来源：http://an.nicolike.cn

C .............. 30
来源：http://eu.jianghongdianzi.cn

C++ ............ 30
来源：http://wz.asd995.cn

SQL ............ 90
来源：http://rc.shxzskj.cn

Bash ........... 80
来源：http://mx.huixiangedu.cn

Kotlin ......... 15
来源：http://gx.9csxet.cn

Swift .......... 15
来源：http://dq.hahajie.cn

Lua ............ 10
来源：http://ro.szsharing.cn

Perl ........... 10
来源：http://gq.nszjky.cn

Scala .......... 10
来源：http://ch.yuntaijiaju.cn

------------------------------------
来源：http://my.wgjwhj.cn

合计 ........... 2106 条
来源：http://ca.hnjuh.cn

按章节统计：
来源：http://cx.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nh.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://em.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ss.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://du.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ko.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mc.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tj.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fz.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kd.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qg.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mw.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wg.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qz.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oa.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gq.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dg.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://fy.lnxyls.cn

R Bash 专题                             80
来源：http://bh.wgjwhj.cn

S C / C++ 专题                          60
来源：http://sm.bookmarksfly.cn

T 其他语言补充                          60
来源：http://lu.bjjhwx.cn

U 高频实用片段                         120
来源：http://oc.shxzukj.cn

------------------------------------
来源：http://dx.wgjwhj.cn

合计                                  2106 条
来源：http://fl.szsharing.cn

--------------------------------------------------------------------------------
来源：http://wm.yuntaijiaju.cn

使用提醒
来源：http://iq.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://uh.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bj.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ag.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zm.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tm.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hh.bookmarksfly.cn

—— 文件结束 ——
来源：http://gj.haigaiapp.cn

================================================================================
来源：http://eu.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://ir.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://nm.newstarts.cn

================================================================================
来源：http://re.muxihuayi.cn

【收录内容】
来源：http://lg.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yf.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eq.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://uf.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://di.9csxet.cn

【使用说明】
来源：http://nj.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ng.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ip.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lc.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vi.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wn.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ht.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fr.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gx.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tf.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zh.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://us.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xv.shtwfgs.cn

【文件统计】
来源：http://qr.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ot.bookmarksfly.cn

目  录
来源：http://ao.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://pg.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xe.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gs.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xz.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ys.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mi.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zm.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vu.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nr.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zs.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aj.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ij.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yz.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ad.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bj.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xu.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xc.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nl.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ib.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jt.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pa.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zr.haigaiapp.cn

================================================================================
来源：http://yn.gzmigu.cn

A. 基础语法与类型
来源：http://sr.muxihuayi.cn

================================================================================
来源：http://qb.521024.cn

[A01] Hello World
来源：http://ip.521024.cn

Py:   print("Hello, World!")
来源：http://gs.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ex.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://kw.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qg.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://ib.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://jj.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://yn.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vi.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://nn.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yp.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qs.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hg.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yi.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://sj.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://xa.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://ub.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bc.huixinmuqiang.cn

[A03] 常量定义
来源：http://oe.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gl.521024.cn

PHP:  const PI = 3.14159;
来源：http://th.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://eo.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://fq.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://kj.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://rx.9csxet.cn

Ruby: PI = 3.14159
来源：http://ki.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://sa.shtwfgs.cn

[A04] 判断变量类型
来源：http://md.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qp.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kx.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hg.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://px.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xh.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://np.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wu.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://pi.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://rm.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ap.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hv.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vs.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tz.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://ay.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://qs.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://df.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://vi.bookmarksfly.cn

[A06] 字符串转数字
来源：http://xi.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://bb.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yo.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lj.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cw.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://np.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rd.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pq.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ep.panjiajie.cn

[A07] 数字转字符串
来源：http://en.hnjuh.cn

Py:   str(42)
来源：http://tr.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://os.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://jy.bookmarksfly.cn

TS:   String(42)
来源：http://cm.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xk.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://lu.huixiangedu.cn

Ruby: 42.to_s
来源：http://od.panjiajie.cn

C#:   42.ToString()
来源：http://mz.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://bo.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qy.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hs.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jq.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nx.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iz.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://di.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ro.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://id.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://tr.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ci.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kk.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zu.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vj.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ts.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fj.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mq.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ig.huixinmuqiang.cn

[A10] 生成随机数
来源：http://ua.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://yj.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://qi.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bb.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kf.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://jd.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ht.haigaiapp.cn

Ruby: rand(1..100)
来源：http://te.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://qp.szsharing.cn

[A11] 条件表达式（三元）
来源：http://rw.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://oo.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xn.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qq.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://px.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://pi.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ar.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://df.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ws.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://mk.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tf.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://is.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://tb.521024.cn

TS:   `Hello, ${name}!`
来源：http://ps.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://wq.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ma.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://bf.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://aa.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yp.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://lp.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://fw.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://dw.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://jh.521024.cn

Java: "第一行\n第二行"
来源：http://yd.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://bu.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://oi.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://kt.muxihuayi.cn

[A14] 注释写法
来源：http://pe.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wn.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://do.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ca.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://hi.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ng.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://oe.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mb.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://am.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://cd.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://ej.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://io.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://lx.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://kx.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qt.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://bz.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://gk.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://hq.szxytkj.cn

[A16] 真假值判断规则
来源：http://pw.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xo.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xl.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://te.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://et.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mo.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://in.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ld.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hx.huixiangedu.cn

[A17] 位运算
来源：http://aj.szsharing.cn


<!-- 参考信息 -->