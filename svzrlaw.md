代发 wailian999

[U87] JS：解构默认值
来源：http://gg.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://ef.shxzskj.cn

[U88] JS：对象展开合并
来源：http://gm.muxihuayi.cn

{ ...a, ...b }
来源：http://ux.shxzukj.cn

[U89] JS：数组去重
来源：http://bk.newstarts.cn

[...new Set(arr)]
来源：http://pf.szxytkj.cn

[U90] JS：数字数组排序
来源：http://yb.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://cw.huanxung.cn

[U91] JS：对象键值遍历
来源：http://cx.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lc.huixiangedu.cn

[U92] JS：深拷贝
来源：http://km.bookmarksfly.cn

structuredClone(obj)
来源：http://vf.asd995.cn

[U93] JS：模板字符串
来源：http://nl.shxzukj.cn

`共 ${n} 条`
来源：http://oy.hahajie.cn

[U94] JS：箭头函数
来源：http://zp.gzmigu.cn

const double = x => x * 2;
来源：http://yn.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://hh.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://of.hahajie.cn

[U96] JS：async/await 与异常
来源：http://ad.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oc.chemitech.net.cn

[U97] JS：并发请求
来源：http://sb.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://pk.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ps.521024.cn

[U99] JS：事件监听
来源：http://vq.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://ao.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://pw.nicolike.cn

document.querySelector(".item")
来源：http://sd.shxzskj.cn

[U101] JS：classList 操作
来源：http://se.colortex.cn

el.classList.toggle("active")
来源：http://bu.jctech888.com.cn

[U102] JS：本地存储
来源：http://jy.chemitech.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://po.shxzukj.cn

[U103] JS：定时器
来源：http://vt.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fw.gzmigu.cn

[U104] JS：防抖
来源：http://xj.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gm.bookmarksfly.cn

[U105] JS：节流
来源：http://sf.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wp.asd995.cn

[U106] JS：日期格式化
来源：http://uy.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mg.hahajie.cn

[U107] JS：数字千分位
来源：http://cq.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ep.lnxyls.cn

[U108] JS：随机整数
来源：http://uw.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cg.asd995.cn

[U109] JS：数组分组
来源：http://fu.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://lj.nicolike.cn

[U110] JS：数组分块
来源：http://ht.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cd.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://eq.panjiajie.cn

new Map(Object.entries(obj))
来源：http://yi.gzmigu.cn

[U112] JS：字符串补位
来源：http://uj.chemitech.net.cn

"7".padStart(3, "0")
来源：http://bp.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://hn.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://od.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://aj.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fo.szsharing.cn

[U115] JS：生成 UUID
来源：http://gq.shtwfgs.cn

crypto.randomUUID()
来源：http://kf.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://pe.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://fh.shtwfgs.cn

[U117] JS：单元测试
来源：http://fc.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://em.szxytkj.cn

[U118] JS：开发服务器
来源：http://tf.hnjuh.cn

npm i -D vite;  npx vite
来源：http://ux.huixiangedu.cn

[U119] JS：生产构建
来源：http://xl.chemitech.net.cn

npx vite build
来源：http://ld.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://fi.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://dg.szxytkj.cn

================================================================================
来源：http://yb.gzmigu.cn

统计汇总
来源：http://wp.haigaiapp.cn

================================================================================
来源：http://xd.haigaiapp.cn

按语言统计（条）：
来源：http://zz.gzmigu.cn

Python ......... 252
来源：http://vi.chemitech.net.cn

PHP ............ 252
来源：http://no.gzmigu.cn

JavaScript ..... 252
来源：http://es.bookmarksfly.cn

TypeScript ..... 212
来源：http://la.jianghongdianzi.cn

Java ........... 212
来源：http://gj.bookmarksfly.cn

Go ............. 212
来源：http://gc.szxytkj.cn

Ruby ........... 212
来源：http://qg.szxytkj.cn

C# ............. 212
来源：http://zl.huixinmuqiang.cn

C .............. 30
来源：http://jf.jctech888.com.cn

C++ ............ 30
来源：http://kk.bookmarksfly.cn

SQL ............ 90
来源：http://lp.yuexingan06.cn

Bash ........... 80
来源：http://hd.asd995.cn

Kotlin ......... 15
来源：http://hq.haigaiapp.cn

Swift .......... 15
来源：http://oj.huixiangedu.cn

Lua ............ 10
来源：http://fa.shtwfgs.cn

Perl ........... 10
来源：http://mk.yuexingan06.cn

Scala .......... 10
来源：http://hr.newstarts.cn

------------------------------------
来源：http://rh.hnjuh.cn

合计 ........... 2106 条
来源：http://vv.hnjuh.cn

按章节统计：
来源：http://cs.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fy.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yd.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fh.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://av.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://an.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jh.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hu.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zt.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cr.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hl.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://va.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hg.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yb.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://to.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eo.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cr.521024.cn

Q SQL 专题                              90
来源：http://hw.yuexingan06.cn

R Bash 专题                             80
来源：http://ns.wgjwhj.cn

S C / C++ 专题                          60
来源：http://cy.hnjuh.cn

T 其他语言补充                          60
来源：http://rv.hahajie.cn

U 高频实用片段                         120
来源：http://ys.9csxet.cn

------------------------------------
来源：http://na.chemitech.net.cn

合计                                  2106 条
来源：http://zu.nszjky.cn

--------------------------------------------------------------------------------
来源：http://pw.szsharing.cn

使用提醒
来源：http://kq.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://aa.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ct.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ss.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rm.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ug.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dk.bookmarksfly.cn

—— 文件结束 ——
来源：http://xl.wgjwhj.cn

================================================================================
来源：http://iw.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://oi.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://xf.yuntaijiaju.cn

================================================================================
来源：http://gc.shxzskj.cn

【收录内容】
来源：http://aw.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wg.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mx.panjiajie.cn

SQL · Bash · C · C++
来源：http://mq.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vf.hnjuh.cn

【使用说明】
来源：http://ek.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://so.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ab.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dt.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xs.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uy.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nq.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zo.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sg.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ku.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ot.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ae.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nj.hnjuh.cn

【文件统计】
来源：http://rk.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jp.colortex.cn

--------------------------------------------------------------------------------
来源：http://cb.colortex.cn

目  录
来源：http://kt.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://gd.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sr.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zi.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ls.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sf.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tv.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://by.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uu.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nu.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rk.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nv.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pl.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oi.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uj.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ub.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lo.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ng.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gu.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pw.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hs.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sz.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kc.newstarts.cn

================================================================================
来源：http://uy.haigaiapp.cn

A. 基础语法与类型
来源：http://jv.shxzukj.cn

================================================================================
来源：http://qb.hahajie.cn

[A01] Hello World
来源：http://gu.colortex.cn

Py:   print("Hello, World!")
来源：http://yy.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://un.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://nj.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ax.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://jy.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://md.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://sy.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bm.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://ap.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ni.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://al.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lz.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sy.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://hw.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://sq.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://gs.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fj.nicolike.cn

[A03] 常量定义
来源：http://ev.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bl.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://vm.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ky.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://fp.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://wu.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://xs.huanxung.cn

Ruby: PI = 3.14159
来源：http://bt.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://gw.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://fn.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gb.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ut.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jc.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://bn.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dn.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rh.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mr.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://ez.szsharing.cn

[A05] 整数除法与取模
来源：http://bc.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yq.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://md.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iq.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://no.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://hq.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://nw.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://od.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://dj.yuexingan06.cn

[A06] 字符串转数字
来源：http://fj.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://xo.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bn.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qu.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ba.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kr.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mi.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ju.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dq.yuexingan06.cn

[A07] 数字转字符串
来源：http://ot.521024.cn

Py:   str(42)
来源：http://ia.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://rf.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://li.chemitech.net.cn

TS:   String(42)
来源：http://aj.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rq.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://js.9csxet.cn

Ruby: 42.to_s
来源：http://yk.colortex.cn

C#:   42.ToString()
来源：http://yk.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://jb.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://my.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hu.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kf.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iy.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jp.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gq.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://er.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ck.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://no.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gx.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://no.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pq.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xj.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ql.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sf.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tu.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oo.panjiajie.cn

[A10] 生成随机数
来源：http://tn.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://qh.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://eq.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nx.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kk.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://ne.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ek.shtwfgs.cn

Ruby: rand(1..100)
来源：http://ti.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://lu.colortex.cn

[A11] 条件表达式（三元）
来源：http://xf.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://md.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nu.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bw.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wo.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://ou.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bh.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vo.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uw.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://ch.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mo.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jf.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://wr.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://nx.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://lv.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nx.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://sn.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://up.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sx.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://hd.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://lp.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://bf.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://vf.nszjky.cn

Java: "第一行\n第二行"
来源：http://me.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://fp.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://zv.hahajie.cn

C#:   "第一行\n第二行"
来源：http://xo.yuntaijiaju.cn

[A14] 注释写法
来源：http://fy.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qw.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ol.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://ev.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://vq.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oq.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://lm.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hn.szsharing.cn


<!-- 参考信息 -->