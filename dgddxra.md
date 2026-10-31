代发 wailian999

[U89] JS：数组去重
来源：http://zn.nicolike.cn

[...new Set(arr)]
来源：http://tr.hahajie.cn

[U90] JS：数字数组排序
来源：http://rz.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://rm.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://va.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tj.nszjky.cn

[U92] JS：深拷贝
来源：http://md.chemitech.net.cn

structuredClone(obj)
来源：http://bc.nicolike.cn

[U93] JS：模板字符串
来源：http://ra.shxzukj.cn

`共 ${n} 条`
来源：http://ow.yuexingan06.cn

[U94] JS：箭头函数
来源：http://wj.bookmarksfly.cn

const double = x => x * 2;
来源：http://bt.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ay.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://sq.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://cd.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zs.wgjwhj.cn

[U97] JS：并发请求
来源：http://vo.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rf.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://hx.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nd.colortex.cn

[U99] JS：事件监听
来源：http://kv.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://qe.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://zn.521024.cn

document.querySelector(".item")
来源：http://fp.yuexingan06.cn

[U101] JS：classList 操作
来源：http://rf.huixiangedu.cn

el.classList.toggle("active")
来源：http://uq.bookmarksfly.cn

[U102] JS：本地存储
来源：http://wc.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://li.asd995.cn

[U103] JS：定时器
来源：http://el.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kh.huixiangedu.cn

[U104] JS：防抖
来源：http://fe.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.haigaiapp.cn

[U105] JS：节流
来源：http://yk.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jx.panjiajie.cn

[U106] JS：日期格式化
来源：http://px.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pj.asd995.cn

[U107] JS：数字千分位
来源：http://us.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hk.9csxet.cn

[U108] JS：随机整数
来源：http://lx.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rx.9csxet.cn

[U109] JS：数组分组
来源：http://qp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://tv.wgjwhj.cn

[U110] JS：数组分块
来源：http://aw.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vs.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://jc.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://pp.lnxyls.cn

[U112] JS：字符串补位
来源：http://aa.newstarts.cn

"7".padStart(3, "0")
来源：http://wb.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ea.nicolike.cn

s.replaceAll("a", "b")
来源：http://bh.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://nz.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lt.huanxung.cn

[U115] JS：生成 UUID
来源：http://ua.shtwfgs.cn

crypto.randomUUID()
来源：http://fl.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://wp.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://gs.wgjwhj.cn

[U117] JS：单元测试
来源：http://to.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://bm.colortex.cn

[U118] JS：开发服务器
来源：http://ww.gzmigu.cn

npm i -D vite;  npx vite
来源：http://tz.hahajie.cn

[U119] JS：生产构建
来源：http://lf.muxihuayi.cn

npx vite build
来源：http://gc.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://hp.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://pa.huixinmuqiang.cn

================================================================================
来源：http://hs.nszjky.cn

统计汇总
来源：http://cu.muxihuayi.cn

================================================================================
来源：http://qq.shxzskj.cn

按语言统计（条）：
来源：http://kh.yuexingan06.cn

Python ......... 252
来源：http://li.jctech888.com.cn

PHP ............ 252
来源：http://ta.521024.cn

JavaScript ..... 252
来源：http://ee.shtwfgs.cn

TypeScript ..... 212
来源：http://wf.muxihuayi.cn

Java ........... 212
来源：http://bu.wgjwhj.cn

Go ............. 212
来源：http://uh.chemitech.net.cn

Ruby ........... 212
来源：http://su.panjiajie.cn

C# ............. 212
来源：http://an.gzmigu.cn

C .............. 30
来源：http://di.jianghongdianzi.cn

C++ ............ 30
来源：http://ll.newstarts.cn

SQL ............ 90
来源：http://px.newstarts.cn

Bash ........... 80
来源：http://sm.jctech888.com.cn

Kotlin ......... 15
来源：http://vv.9csxet.cn

Swift .......... 15
来源：http://qx.jianghongdianzi.cn

Lua ............ 10
来源：http://wk.haigaiapp.cn

Perl ........... 10
来源：http://zy.huixinmuqiang.cn

Scala .......... 10
来源：http://iw.jianghongdianzi.cn

------------------------------------
来源：http://ne.shxzukj.cn

合计 ........... 2106 条
来源：http://pe.huixinmuqiang.cn

按章节统计：
来源：http://lm.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lt.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fi.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://se.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lm.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wf.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lh.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sz.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bi.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vb.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hb.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ca.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mx.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://od.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xf.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://az.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eu.newstarts.cn

Q SQL 专题                              90
来源：http://fh.bjjhwx.cn

R Bash 专题                             80
来源：http://yn.lnxyls.cn

S C / C++ 专题                          60
来源：http://rj.huixiangedu.cn

T 其他语言补充                          60
来源：http://bl.9csxet.cn

U 高频实用片段                         120
来源：http://ql.szxytkj.cn

------------------------------------
来源：http://dj.jctech888.com.cn

合计                                  2106 条
来源：http://bh.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ng.huixinmuqiang.cn

使用提醒
来源：http://gw.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://th.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oo.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zt.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cy.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sh.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fs.asd995.cn

—— 文件结束 ——
来源：http://pe.jctech888.com.cn

================================================================================
来源：http://fb.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://qt.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://hq.haigaiapp.cn

================================================================================
来源：http://dn.colortex.cn

【收录内容】
来源：http://cs.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://la.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ff.huanxung.cn

SQL · Bash · C · C++
来源：http://ce.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ji.wgjwhj.cn

【使用说明】
来源：http://tv.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://im.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dz.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ys.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rr.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hr.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hj.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xb.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yr.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lo.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jo.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://is.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rf.jianghongdianzi.cn

【文件统计】
来源：http://ry.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qi.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://el.chemitech.net.cn

目  录
来源：http://vm.newstarts.cn

--------------------------------------------------------------------------------
来源：http://aa.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ym.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lk.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://de.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pl.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kw.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wb.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jp.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ml.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tx.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://md.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xz.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jt.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xk.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dh.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rg.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dd.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hm.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eb.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pf.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kj.yuntaijiaju.cn

================================================================================
来源：http://vj.szsharing.cn

A. 基础语法与类型
来源：http://in.jctech888.com.cn

================================================================================
来源：http://yr.yuntaijiaju.cn

[A01] Hello World
来源：http://sa.panjiajie.cn

Py:   print("Hello, World!")
来源：http://gq.asd995.cn

PHP:  echo "Hello, World!";
来源：http://iv.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://rm.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kg.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://ok.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://ze.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://oi.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gk.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://kn.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bd.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mg.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sh.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ef.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://lq.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://vy.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://bv.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hb.bjjhwx.cn

[A03] 常量定义
来源：http://sl.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ns.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://dx.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://zv.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://lj.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://hp.9csxet.cn

Go:   const PI = 3.14159
来源：http://nb.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://fk.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://hi.wgjwhj.cn

[A04] 判断变量类型
来源：http://ik.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zb.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kj.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bj.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://cd.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vp.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qs.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ou.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://sz.huixiangedu.cn

[A05] 整数除法与取模
来源：http://vh.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qy.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vu.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qi.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ps.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://sy.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://gt.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://ea.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ml.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://eq.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://yw.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nj.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://og.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cg.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hd.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://my.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kr.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wq.yuexingan06.cn

[A07] 数字转字符串
来源：http://ss.jctech888.com.cn

Py:   str(42)
来源：http://nv.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://gj.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://fw.wgjwhj.cn

TS:   String(42)
来源：http://hm.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sp.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://bf.asd995.cn

Ruby: 42.to_s
来源：http://te.szsharing.cn

C#:   42.ToString()
来源：http://oe.hahajie.cn

[A08] 取整与四舍五入
来源：http://rs.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sw.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kp.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ej.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sz.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bg.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://or.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eh.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wn.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://ed.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://in.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kp.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pq.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qk.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ej.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rx.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sb.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qn.szsharing.cn

[A10] 生成随机数
来源：http://rf.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://rq.nszjky.cn

PHP:  random_int(1, 100);
来源：http://in.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jz.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cg.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://cq.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sx.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://be.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://rs.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://tq.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://dn.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cf.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ha.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://im.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ai.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uv.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://id.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://np.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://gs.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ks.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nt.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://mk.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://iz.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://vo.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xh.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://yf.521024.cn

C#:   $"Hello, {name}!"
来源：http://xn.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xs.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://fe.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://cx.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://yh.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://fg.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ls.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://qr.521024.cn

Ruby: "第一行\n第二行"
来源：http://zd.szsharing.cn

C#:   "第一行\n第二行"
来源：http://gg.jctech888.com.cn

[A14] 注释写法
来源：http://wj.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wi.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gb.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://yx.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://re.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yq.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://ty.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mc.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://sr.521024.cn

[A15] 空值判断与默认值
来源：http://zt.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://wq.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://ew.hahajie.cn


<!-- 参考信息 -->