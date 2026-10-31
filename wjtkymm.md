代发 wailian999

[U91] JS：对象键值遍历
来源：http://fy.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hu.lnxyls.cn

[U92] JS：深拷贝
来源：http://da.gzmigu.cn

structuredClone(obj)
来源：http://td.shtwfgs.cn

[U93] JS：模板字符串
来源：http://np.huixinmuqiang.cn

`共 ${n} 条`
来源：http://mr.szsharing.cn

[U94] JS：箭头函数
来源：http://rk.hnjuh.cn

const double = x => x * 2;
来源：http://kc.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://fi.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://xb.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://jl.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ft.jctech888.com.cn

[U97] JS：并发请求
来源：http://tq.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qz.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://eq.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gw.huixiangedu.cn

[U99] JS：事件监听
来源：http://sh.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://dj.asd995.cn

[U100] JS：DOM 查询
来源：http://is.shxzskj.cn

document.querySelector(".item")
来源：http://un.asd995.cn

[U101] JS：classList 操作
来源：http://vb.chemitech.net.cn

el.classList.toggle("active")
来源：http://xd.hahajie.cn

[U102] JS：本地存储
来源：http://es.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jr.521024.cn

[U103] JS：定时器
来源：http://np.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ci.shxzukj.cn

[U104] JS：防抖
来源：http://ps.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.colortex.cn

[U105] JS：节流
来源：http://zz.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zp.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://za.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pz.bjjhwx.cn

[U107] JS：数字千分位
来源：http://og.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ct.nicolike.cn

[U108] JS：随机整数
来源：http://cr.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://su.hahajie.cn

[U109] JS：数组分组
来源：http://bm.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://yl.panjiajie.cn

[U110] JS：数组分块
来源：http://vp.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ei.szsharing.cn

[U111] JS：对象转 Map
来源：http://qw.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://on.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ze.jctech888.com.cn

"7".padStart(3, "0")
来源：http://th.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://vu.colortex.cn

s.replaceAll("a", "b")
来源：http://gn.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://cb.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rd.szsharing.cn

[U115] JS：生成 UUID
来源：http://sd.panjiajie.cn

crypto.randomUUID()
来源：http://xw.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://ap.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://de.huanxung.cn

[U117] JS：单元测试
来源：http://wh.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://al.yuexingan06.cn

[U118] JS：开发服务器
来源：http://yp.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://kd.muxihuayi.cn

[U119] JS：生产构建
来源：http://ax.shtwfgs.cn

npx vite build
来源：http://lb.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://nb.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://tn.szsharing.cn

================================================================================
来源：http://pr.yuntaijiaju.cn

统计汇总
来源：http://ir.bjjhwx.cn

================================================================================
来源：http://mt.lnxyls.cn

按语言统计（条）：
来源：http://nb.chemitech.net.cn

Python ......... 252
来源：http://ig.9csxet.cn

PHP ............ 252
来源：http://ic.shxzskj.cn

JavaScript ..... 252
来源：http://dc.9csxet.cn

TypeScript ..... 212
来源：http://qp.hahajie.cn

Java ........... 212
来源：http://ed.9csxet.cn

Go ............. 212
来源：http://wx.521024.cn

Ruby ........... 212
来源：http://fd.panjiajie.cn

C# ............. 212
来源：http://rq.jctech888.com.cn

C .............. 30
来源：http://np.bjjhwx.cn

C++ ............ 30
来源：http://pe.521024.cn

SQL ............ 90
来源：http://el.szsharing.cn

Bash ........... 80
来源：http://kn.huanxung.cn

Kotlin ......... 15
来源：http://to.bjjhwx.cn

Swift .......... 15
来源：http://en.521024.cn

Lua ............ 10
来源：http://tc.521024.cn

Perl ........... 10
来源：http://wc.shxzskj.cn

Scala .......... 10
来源：http://nq.gzmigu.cn

------------------------------------
来源：http://sq.shxzskj.cn

合计 ........... 2106 条
来源：http://ky.gzmigu.cn

按章节统计：
来源：http://kx.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ip.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qi.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xg.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ej.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ci.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bi.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tg.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cr.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uk.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ax.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cv.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oy.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qj.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uu.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nb.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://le.shxzskj.cn

Q SQL 专题                              90
来源：http://ms.jctech888.com.cn

R Bash 专题                             80
来源：http://eh.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://ue.bookmarksfly.cn

T 其他语言补充                          60
来源：http://mg.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://aa.9csxet.cn

------------------------------------
来源：http://qd.shxzskj.cn

合计                                  2106 条
来源：http://wz.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://gl.nicolike.cn

使用提醒
来源：http://hr.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://oa.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nm.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zk.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ez.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wi.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://io.521024.cn

—— 文件结束 ——
来源：http://dp.haigaiapp.cn

================================================================================
来源：http://ke.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://qp.colortex.cn

Common Programming Examples Cheat Book
来源：http://nv.muxihuayi.cn

================================================================================
来源：http://fl.szsharing.cn

【收录内容】
来源：http://ql.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kl.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wu.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://jp.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dw.haigaiapp.cn

【使用说明】
来源：http://gi.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qf.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dm.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dc.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yz.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nh.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ag.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rg.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qw.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rt.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kl.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ky.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ud.huixinmuqiang.cn

【文件统计】
来源：http://ea.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kh.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://nj.asd995.cn

目  录
来源：http://kv.newstarts.cn

--------------------------------------------------------------------------------
来源：http://pp.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oj.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pw.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dg.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jt.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wi.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sh.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://il.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ic.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ib.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cx.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ow.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ks.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://am.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://og.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qc.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mk.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gu.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cu.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fe.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cy.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wq.szxytkj.cn

================================================================================
来源：http://wi.521024.cn

A. 基础语法与类型
来源：http://kj.yuntaijiaju.cn

================================================================================
来源：http://qy.hahajie.cn

[A01] Hello World
来源：http://at.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://eu.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://cc.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://nl.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zm.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://lu.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://hj.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://tw.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gy.hahajie.cn

[A02] 变量声明与赋值
来源：http://fw.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xf.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ws.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dj.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cq.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://sw.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://vt.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://oq.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pb.lnxyls.cn

[A03] 常量定义
来源：http://lx.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cc.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://ds.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://md.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://cn.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://vu.521024.cn

Go:   const PI = 3.14159
来源：http://ry.szsharing.cn

Ruby: PI = 3.14159
来源：http://er.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://ur.shxzukj.cn

[A04] 判断变量类型
来源：http://we.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dg.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ea.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://on.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://bm.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://io.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fw.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://he.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://wk.szsharing.cn

[A05] 整数除法与取模
来源：http://xp.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ca.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://we.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ey.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ge.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ms.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://oa.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://dt.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://kc.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://fd.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://ya.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mr.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hr.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://le.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ln.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rh.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://no.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nc.521024.cn

[A07] 数字转字符串
来源：http://hc.bjjhwx.cn

Py:   str(42)
来源：http://ja.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://yg.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://fj.huixiangedu.cn

TS:   String(42)
来源：http://zr.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hq.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://qe.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://lw.szxytkj.cn

C#:   42.ToString()
来源：http://ls.szxytkj.cn

[A08] 取整与四舍五入
来源：http://vk.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kt.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qh.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ig.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tg.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ms.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qb.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bc.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bl.521024.cn

[A09] 绝对值与最大最小值
来源：http://ca.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fp.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oa.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sz.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nv.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ve.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pu.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xj.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ww.bookmarksfly.cn

[A10] 生成随机数
来源：http://io.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://az.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://px.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ca.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oy.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://yo.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lg.huanxung.cn

Ruby: rand(1..100)
来源：http://ks.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://si.nicolike.cn

[A11] 条件表达式（三元）
来源：http://xi.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://sq.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://li.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://we.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rk.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://qv.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ou.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pe.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ia.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://yk.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://we.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vx.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://qc.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://sk.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://sz.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pd.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://wy.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://hl.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rs.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://ec.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://at.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://bo.hahajie.cn

TS:   "第一行\n第二行"
来源：http://pk.hnjuh.cn

Java: "第一行\n第二行"
来源：http://li.hahajie.cn

Go:   "第一行\n第二行"
来源：http://du.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://lq.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://yv.huixinmuqiang.cn

[A14] 注释写法
来源：http://fn.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eq.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ly.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ko.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://rf.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vb.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://dz.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://no.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://ig.gzmigu.cn

[A15] 空值判断与默认值
来源：http://ou.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://ti.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://rx.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://aj.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://ew.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ni.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://mg.wgjwhj.cn


<!-- 参考信息 -->