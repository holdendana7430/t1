代发 wailian999

[U93] JS：模板字符串
来源：http://ga.9csxet.cn

`共 ${n} 条`
来源：http://ad.shxzskj.cn

[U94] JS：箭头函数
来源：http://sh.9csxet.cn

const double = x => x * 2;
来源：http://aw.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://bu.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://xv.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://pj.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ez.huanxung.cn

[U97] JS：并发请求
来源：http://gs.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://co.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://lr.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ud.nszjky.cn

[U99] JS：事件监听
来源：http://bp.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://jg.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://ij.panjiajie.cn

document.querySelector(".item")
来源：http://si.hnjuh.cn

[U101] JS：classList 操作
来源：http://ha.hnjuh.cn

el.classList.toggle("active")
来源：http://gg.lnxyls.cn

[U102] JS：本地存储
来源：http://qg.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ra.asd995.cn

[U103] JS：定时器
来源：http://rs.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lc.szxytkj.cn

[U104] JS：防抖
来源：http://un.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yk.shtwfgs.cn

[U105] JS：节流
来源：http://na.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oe.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://ax.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ov.chemitech.net.cn

[U107] JS：数字千分位
来源：http://qz.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://us.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://fv.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uq.jctech888.com.cn

[U109] JS：数组分组
来源：http://xj.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://af.colortex.cn

[U110] JS：数组分块
来源：http://fc.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hd.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://rf.nicolike.cn

new Map(Object.entries(obj))
来源：http://ta.nszjky.cn

[U112] JS：字符串补位
来源：http://vk.szsharing.cn

"7".padStart(3, "0")
来源：http://el.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://pi.hnjuh.cn

s.replaceAll("a", "b")
来源：http://cy.szsharing.cn

[U114] JS：JSON 深比较
来源：http://yw.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://is.huanxung.cn

[U115] JS：生成 UUID
来源：http://ks.bjjhwx.cn

crypto.randomUUID()
来源：http://bl.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://it.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://ub.muxihuayi.cn

[U117] JS：单元测试
来源：http://sh.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://ht.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://zm.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://ll.gzmigu.cn

[U119] JS：生产构建
来源：http://sh.yuntaijiaju.cn

npx vite build
来源：http://ob.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://wt.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://vo.jctech888.com.cn

================================================================================
来源：http://vk.nszjky.cn

统计汇总
来源：http://ll.wgjwhj.cn

================================================================================
来源：http://tk.panjiajie.cn

按语言统计（条）：
来源：http://kl.yuexingan06.cn

Python ......... 252
来源：http://fn.bookmarksfly.cn

PHP ............ 252
来源：http://cp.shxzukj.cn

JavaScript ..... 252
来源：http://df.szsharing.cn

TypeScript ..... 212
来源：http://oa.chemitech.net.cn

Java ........... 212
来源：http://is.shxzukj.cn

Go ............. 212
来源：http://cu.bookmarksfly.cn

Ruby ........... 212
来源：http://ae.nszjky.cn

C# ............. 212
来源：http://jl.panjiajie.cn

C .............. 30
来源：http://rg.yuntaijiaju.cn

C++ ............ 30
来源：http://by.nicolike.cn

SQL ............ 90
来源：http://pg.huixiangedu.cn

Bash ........... 80
来源：http://ns.huixiangedu.cn

Kotlin ......... 15
来源：http://sg.muxihuayi.cn

Swift .......... 15
来源：http://rw.panjiajie.cn

Lua ............ 10
来源：http://by.lnxyls.cn

Perl ........... 10
来源：http://ie.szsharing.cn

Scala .......... 10
来源：http://uu.szsharing.cn

------------------------------------
来源：http://tt.szxytkj.cn

合计 ........... 2106 条
来源：http://he.521024.cn

按章节统计：
来源：http://ng.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sw.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ap.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gs.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ym.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qv.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vw.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ao.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tp.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qr.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tu.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zp.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xi.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cq.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uu.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://up.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hd.bookmarksfly.cn

Q SQL 专题                              90
来源：http://fy.jctech888.com.cn

R Bash 专题                             80
来源：http://yn.huanxung.cn

S C / C++ 专题                          60
来源：http://rt.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://yr.lnxyls.cn

U 高频实用片段                         120
来源：http://gv.hnjuh.cn

------------------------------------
来源：http://sg.shxzukj.cn

合计                                  2106 条
来源：http://ju.521024.cn

--------------------------------------------------------------------------------
来源：http://zj.muxihuayi.cn

使用提醒
来源：http://xo.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://uf.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ag.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dd.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kx.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://te.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kg.panjiajie.cn

—— 文件结束 ——
来源：http://ek.gzmigu.cn

================================================================================
来源：http://sc.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://ru.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://mr.521024.cn

================================================================================
来源：http://zh.asd995.cn

【收录内容】
来源：http://du.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wv.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vq.gzmigu.cn

SQL · Bash · C · C++
来源：http://xr.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://at.wgjwhj.cn

【使用说明】
来源：http://yp.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dg.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eg.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ul.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jm.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://za.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dw.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fv.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jb.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gc.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zz.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wa.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://db.521024.cn

【文件统计】
来源：http://ky.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zv.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ek.9csxet.cn

目  录
来源：http://up.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://oz.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oo.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ve.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hq.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jl.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hh.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kq.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vy.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qw.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eq.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ky.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ly.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hn.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ti.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hq.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wo.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ir.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fn.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jd.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qe.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pw.colortex.cn

================================================================================
来源：http://nb.szxytkj.cn

A. 基础语法与类型
来源：http://dn.colortex.cn

================================================================================
来源：http://bh.szsharing.cn

[A01] Hello World
来源：http://yc.szsharing.cn

Py:   print("Hello, World!")
来源：http://ph.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://fd.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://ao.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zx.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://iz.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://vf.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://zt.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jl.hahajie.cn

[A02] 变量声明与赋值
来源：http://oe.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ou.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cn.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fy.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qn.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://be.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://oo.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://yo.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://li.521024.cn

[A03] 常量定义
来源：http://ct.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eo.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://lk.nszjky.cn

JS:   const PI = 3.14159;
来源：http://gi.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://ig.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://vj.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://rn.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://zt.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://bo.newstarts.cn

[A04] 判断变量类型
来源：http://cg.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vu.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tj.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fp.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://lz.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rx.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qj.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gm.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://yy.muxihuayi.cn

[A05] 整数除法与取模
来源：http://qb.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yf.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fk.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nr.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hg.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://mw.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://pl.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://sx.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://vj.haigaiapp.cn

[A06] 字符串转数字
来源：http://kh.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://gf.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wh.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qi.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iu.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kk.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fg.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nx.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mf.nicolike.cn

[A07] 数字转字符串
来源：http://dq.bjjhwx.cn

Py:   str(42)
来源：http://mm.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://af.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://jx.asd995.cn

TS:   String(42)
来源：http://xv.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zz.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://lx.gzmigu.cn

Ruby: 42.to_s
来源：http://ta.szsharing.cn

C#:   42.ToString()
来源：http://ii.hahajie.cn

[A08] 取整与四舍五入
来源：http://qv.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://it.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qd.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mt.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kd.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mw.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://za.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://el.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://em.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://gt.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tx.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qg.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gk.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ue.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zy.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yk.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tr.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tz.shxzukj.cn

[A10] 生成随机数
来源：http://vq.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ba.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://sh.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gw.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vj.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://iw.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dh.colortex.cn

Ruby: rand(1..100)
来源：http://ie.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://yz.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://jq.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://yk.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sl.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vf.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ts.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://cp.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rn.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mv.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wb.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://fb.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://of.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://av.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://mi.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://nz.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ka.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gu.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://kp.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://vx.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nb.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://gg.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://ra.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://nd.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://xt.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://iz.huanxung.cn

Go:   "第一行\n第二行"
来源：http://bx.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://ob.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://nq.yuexingan06.cn

[A14] 注释写法
来源：http://tu.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lf.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ak.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://gk.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://sw.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cm.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://mv.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ry.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://ky.szxytkj.cn

[A15] 空值判断与默认值
来源：http://fr.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://bo.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://uv.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://mh.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://nq.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bb.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://gd.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://he.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://fh.panjiajie.cn

[A16] 真假值判断规则
来源：http://ly.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mt.hnjuh.cn


<!-- 参考信息 -->