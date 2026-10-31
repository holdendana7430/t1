代发 wailian999

[U91] JS：对象键值遍历
来源：http://wo.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qi.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://hj.shxzukj.cn

structuredClone(obj)
来源：http://od.shxzskj.cn

[U93] JS：模板字符串
来源：http://oj.shxzskj.cn

`共 ${n} 条`
来源：http://yg.hnjuh.cn

[U94] JS：箭头函数
来源：http://xj.newstarts.cn

const double = x => x * 2;
来源：http://zn.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://xd.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://oa.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://an.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dv.szxytkj.cn

[U97] JS：并发请求
来源：http://hz.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fr.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://bo.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kd.521024.cn

[U99] JS：事件监听
来源：http://pk.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://qa.panjiajie.cn

[U100] JS：DOM 查询
来源：http://tv.bookmarksfly.cn

document.querySelector(".item")
来源：http://en.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://cv.panjiajie.cn

el.classList.toggle("active")
来源：http://oz.nicolike.cn

[U102] JS：本地存储
来源：http://uz.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ij.asd995.cn

[U103] JS：定时器
来源：http://sb.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wq.jctech888.com.cn

[U104] JS：防抖
来源：http://dn.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://no.jctech888.com.cn

[U105] JS：节流
来源：http://fj.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jp.hnjuh.cn

[U106] JS：日期格式化
来源：http://te.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tr.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://jd.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sw.yuexingan06.cn

[U108] JS：随机整数
来源：http://vn.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://av.szxytkj.cn

[U109] JS：数组分组
来源：http://dd.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://rf.hahajie.cn

[U110] JS：数组分块
来源：http://eb.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rh.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://db.asd995.cn

new Map(Object.entries(obj))
来源：http://ij.nszjky.cn

[U112] JS：字符串补位
来源：http://el.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://la.szsharing.cn

[U113] JS：正则替换全部
来源：http://zp.hahajie.cn

s.replaceAll("a", "b")
来源：http://xi.huanxung.cn

[U114] JS：JSON 深比较
来源：http://eh.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://bt.szsharing.cn

crypto.randomUUID()
来源：http://ha.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://gv.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://ka.panjiajie.cn

[U117] JS：单元测试
来源：http://vt.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://gq.yuexingan06.cn

[U118] JS：开发服务器
来源：http://yw.asd995.cn

npm i -D vite;  npx vite
来源：http://iq.nicolike.cn

[U119] JS：生产构建
来源：http://xp.bookmarksfly.cn

npx vite build
来源：http://lj.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://wk.521024.cn

import.meta.env.VITE_API_URL
来源：http://hi.jianghongdianzi.cn

================================================================================
来源：http://bl.nszjky.cn

统计汇总
来源：http://sr.jctech888.com.cn

================================================================================
来源：http://xh.huixinmuqiang.cn

按语言统计（条）：
来源：http://mi.shtwfgs.cn

Python ......... 252
来源：http://av.muxihuayi.cn

PHP ............ 252
来源：http://vz.jianghongdianzi.cn

JavaScript ..... 252
来源：http://pc.gzmigu.cn

TypeScript ..... 212
来源：http://ir.yuexingan06.cn

Java ........... 212
来源：http://ko.521024.cn

Go ............. 212
来源：http://cu.gzmigu.cn

Ruby ........... 212
来源：http://xn.shxzskj.cn

C# ............. 212
来源：http://xh.hnjuh.cn

C .............. 30
来源：http://yj.huanxung.cn

C++ ............ 30
来源：http://pp.shxzukj.cn

SQL ............ 90
来源：http://vc.yuntaijiaju.cn

Bash ........... 80
来源：http://fp.yuntaijiaju.cn

Kotlin ......... 15
来源：http://vd.jianghongdianzi.cn

Swift .......... 15
来源：http://mw.huixinmuqiang.cn

Lua ............ 10
来源：http://bg.9csxet.cn

Perl ........... 10
来源：http://nu.gzmigu.cn

Scala .......... 10
来源：http://rf.panjiajie.cn

------------------------------------
来源：http://dh.colortex.cn

合计 ........... 2106 条
来源：http://dq.gzmigu.cn

按章节统计：
来源：http://ei.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bk.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zj.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fy.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ce.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bl.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vh.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rb.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lk.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ls.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://is.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qr.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sb.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wp.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ka.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jc.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bq.muxihuayi.cn

Q SQL 专题                              90
来源：http://jx.nicolike.cn

R Bash 专题                             80
来源：http://sy.chemitech.net.cn

S C / C++ 专题                          60
来源：http://an.szxytkj.cn

T 其他语言补充                          60
来源：http://zd.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://hd.jctech888.com.cn

------------------------------------
来源：http://fu.asd995.cn

合计                                  2106 条
来源：http://kj.nicolike.cn

--------------------------------------------------------------------------------
来源：http://wq.bookmarksfly.cn

使用提醒
来源：http://dd.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://id.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sc.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jr.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cq.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dk.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ox.yuntaijiaju.cn

—— 文件结束 ——
来源：http://vq.gzmigu.cn

================================================================================
来源：http://go.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://mf.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://dw.chemitech.net.cn

================================================================================
来源：http://ah.shtwfgs.cn

【收录内容】
来源：http://rt.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yw.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jw.hahajie.cn

SQL · Bash · C · C++
来源：http://ww.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wi.shxzskj.cn

【使用说明】
来源：http://dd.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dg.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dv.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ht.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dl.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bm.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dm.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ax.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dr.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://am.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zb.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ee.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fa.nszjky.cn

【文件统计】
来源：http://eo.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sr.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ws.jianghongdianzi.cn

目  录
来源：http://tr.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dx.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sq.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fq.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wm.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cl.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dm.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://we.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sk.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pn.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ct.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wx.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bs.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uk.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qr.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fv.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ig.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yo.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gy.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oa.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fh.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aa.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ix.9csxet.cn

================================================================================
来源：http://tx.nicolike.cn

A. 基础语法与类型
来源：http://fp.huixinmuqiang.cn

================================================================================
来源：http://ig.huixiangedu.cn

[A01] Hello World
来源：http://om.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ns.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://cx.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://fs.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://it.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://qx.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://ek.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://eo.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jd.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ds.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nm.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ij.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xm.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iz.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://ht.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://jj.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://sr.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ds.newstarts.cn

[A03] 常量定义
来源：http://qs.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xx.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://hz.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://jd.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://yu.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://kn.nicolike.cn

Go:   const PI = 3.14159
来源：http://za.lnxyls.cn

Ruby: PI = 3.14159
来源：http://wh.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://gg.hahajie.cn

[A04] 判断变量类型
来源：http://mz.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mm.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://be.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cn.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://ji.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tl.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fs.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pg.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://io.nicolike.cn

[A05] 整数除法与取模
来源：http://en.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gy.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fh.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mq.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ws.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://gn.521024.cn

Go:   7 / 2; 7 % 2
来源：http://co.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://bk.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://jh.lnxyls.cn

[A06] 字符串转数字
来源：http://jv.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ya.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ys.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jx.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qc.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vq.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rp.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nh.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cb.huanxung.cn

[A07] 数字转字符串
来源：http://wu.huixinmuqiang.cn

Py:   str(42)
来源：http://pb.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://co.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://gg.huixiangedu.cn

TS:   String(42)
来源：http://to.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dz.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://tp.haigaiapp.cn

Ruby: 42.to_s
来源：http://kx.hnjuh.cn

C#:   42.ToString()
来源：http://tl.shxzukj.cn

[A08] 取整与四舍五入
来源：http://va.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qy.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://an.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tz.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tg.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cs.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oq.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fc.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jy.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ju.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kz.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ui.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pf.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dx.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mm.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lv.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ov.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pf.hnjuh.cn

[A10] 生成随机数
来源：http://zx.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://vr.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://nq.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wz.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mj.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://mi.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oj.shtwfgs.cn

Ruby: rand(1..100)
来源：http://qr.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://wr.asd995.cn

[A11] 条件表达式（三元）
来源：http://ku.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://fl.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cb.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tu.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hx.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://cr.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tu.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vr.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rd.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://gm.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dy.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gb.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://um.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://nn.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://nh.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ze.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://dk.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://ny.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bq.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://ey.asd995.cn

PHP:  "第一行\n第二行"
来源：http://jd.521024.cn

JS:   "第一行\n第二行"
来源：http://uj.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://ki.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://hx.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://yy.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://co.521024.cn

C#:   "第一行\n第二行"
来源：http://ws.jianghongdianzi.cn

[A14] 注释写法
来源：http://sg.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ey.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sg.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://rj.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ma.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tn.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://hu.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sk.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://oq.521024.cn

[A15] 空值判断与默认值
来源：http://bn.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://dx.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://so.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://tx.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://wy.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nj.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://yd.yuntaijiaju.cn


<!-- 参考信息 -->