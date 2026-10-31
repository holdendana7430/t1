代发 wailian999

[U87] JS：解构默认值
来源：http://vn.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://as.nicolike.cn

[U88] JS：对象展开合并
来源：http://sn.szxytkj.cn

{ ...a, ...b }
来源：http://dj.bookmarksfly.cn

[U89] JS：数组去重
来源：http://db.9csxet.cn

[...new Set(arr)]
来源：http://oq.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://wg.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://iq.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://kd.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pp.asd995.cn

[U92] JS：深拷贝
来源：http://as.nszjky.cn

structuredClone(obj)
来源：http://mz.shxzskj.cn

[U93] JS：模板字符串
来源：http://at.wgjwhj.cn

`共 ${n} 条`
来源：http://ld.szxytkj.cn

[U94] JS：箭头函数
来源：http://pu.hahajie.cn

const double = x => x * 2;
来源：http://zg.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://wl.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://ue.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://me.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ji.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://tg.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ba.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rc.shtwfgs.cn

[U99] JS：事件监听
来源：http://mi.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://ci.colortex.cn

[U100] JS：DOM 查询
来源：http://fy.colortex.cn

document.querySelector(".item")
来源：http://pl.chemitech.net.cn

[U101] JS：classList 操作
来源：http://th.bjjhwx.cn

el.classList.toggle("active")
来源：http://jt.muxihuayi.cn

[U102] JS：本地存储
来源：http://kq.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zm.shtwfgs.cn

[U103] JS：定时器
来源：http://uv.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ba.9csxet.cn

[U104] JS：防抖
来源：http://sg.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ra.chemitech.net.cn

[U105] JS：节流
来源：http://js.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yw.521024.cn

[U106] JS：日期格式化
来源：http://is.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://he.9csxet.cn

[U107] JS：数字千分位
来源：http://ax.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://de.gzmigu.cn

[U108] JS：随机整数
来源：http://cw.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://is.shxzukj.cn

[U109] JS：数组分组
来源：http://ga.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://wt.shtwfgs.cn

[U110] JS：数组分块
来源：http://dk.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tg.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://jb.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://wb.chemitech.net.cn

[U112] JS：字符串补位
来源：http://ex.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://pr.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://qd.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ah.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://oq.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://jh.yuexingan06.cn

crypto.randomUUID()
来源：http://jg.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://or.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://iv.colortex.cn

[U117] JS：单元测试
来源：http://hn.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://cs.shtwfgs.cn

[U118] JS：开发服务器
来源：http://xw.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://nd.colortex.cn

[U119] JS：生产构建
来源：http://wm.nicolike.cn

npx vite build
来源：http://wz.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://lz.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://px.panjiajie.cn

================================================================================
来源：http://ar.gzmigu.cn

统计汇总
来源：http://jq.asd995.cn

================================================================================
来源：http://qp.hnjuh.cn

按语言统计（条）：
来源：http://lm.lnxyls.cn

Python ......... 252
来源：http://lh.huixiangedu.cn

PHP ............ 252
来源：http://ky.yuntaijiaju.cn

JavaScript ..... 252
来源：http://nw.jianghongdianzi.cn

TypeScript ..... 212
来源：http://ws.colortex.cn

Java ........... 212
来源：http://kk.hahajie.cn

Go ............. 212
来源：http://jl.szxytkj.cn

Ruby ........... 212
来源：http://jz.wgjwhj.cn

C# ............. 212
来源：http://vx.szxytkj.cn

C .............. 30
来源：http://wh.huixiangedu.cn

C++ ............ 30
来源：http://nr.szxytkj.cn

SQL ............ 90
来源：http://gj.colortex.cn

Bash ........... 80
来源：http://lm.bjjhwx.cn

Kotlin ......... 15
来源：http://gn.newstarts.cn

Swift .......... 15
来源：http://va.huixiangedu.cn

Lua ............ 10
来源：http://wk.haigaiapp.cn

Perl ........... 10
来源：http://nu.panjiajie.cn

Scala .......... 10
来源：http://ce.yuntaijiaju.cn

------------------------------------
来源：http://gl.yuexingan06.cn

合计 ........... 2106 条
来源：http://sq.shtwfgs.cn

按章节统计：
来源：http://xy.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lz.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ah.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hr.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eu.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://io.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nh.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dz.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://it.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://au.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tk.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wu.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iq.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ku.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bv.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qm.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pd.hnjuh.cn

Q SQL 专题                              90
来源：http://fi.shtwfgs.cn

R Bash 专题                             80
来源：http://gc.huixiangedu.cn

S C / C++ 专题                          60
来源：http://ww.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://co.hahajie.cn

U 高频实用片段                         120
来源：http://bc.yuexingan06.cn

------------------------------------
来源：http://ri.9csxet.cn

合计                                  2106 条
来源：http://ah.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://xq.hahajie.cn

使用提醒
来源：http://qg.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://nh.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xh.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://at.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nc.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fp.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rs.9csxet.cn

—— 文件结束 ——
来源：http://tk.gzmigu.cn

================================================================================
来源：http://ex.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://la.521024.cn

Common Programming Examples Cheat Book
来源：http://tc.szxytkj.cn

================================================================================
来源：http://na.jianghongdianzi.cn

【收录内容】
来源：http://vx.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yd.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ye.szsharing.cn

SQL · Bash · C · C++
来源：http://ef.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pm.521024.cn

【使用说明】
来源：http://uw.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ob.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ns.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bk.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ax.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://je.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gb.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sa.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://io.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ll.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tu.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ap.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yc.haigaiapp.cn

【文件统计】
来源：http://ye.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lc.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ld.szsharing.cn

目  录
来源：http://vz.asd995.cn

--------------------------------------------------------------------------------
来源：http://de.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ki.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gh.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dd.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sa.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ma.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jn.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ug.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vv.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zl.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wy.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wl.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ma.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cm.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ju.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pr.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://te.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ks.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wu.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bx.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ah.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gw.nszjky.cn

================================================================================
来源：http://bv.huixinmuqiang.cn

A. 基础语法与类型
来源：http://dt.521024.cn

================================================================================
来源：http://pt.bjjhwx.cn

[A01] Hello World
来源：http://ek.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://ay.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://zr.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://ba.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nf.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://ez.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://mq.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://nr.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://us.gzmigu.cn

[A02] 变量声明与赋值
来源：http://vz.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hl.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ko.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yd.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fa.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://ai.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://oy.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://wp.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wu.hahajie.cn

[A03] 常量定义
来源：http://kn.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ym.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://hb.newstarts.cn

JS:   const PI = 3.14159;
来源：http://qn.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://cm.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://dp.panjiajie.cn

Go:   const PI = 3.14159
来源：http://fg.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://qi.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://el.panjiajie.cn

[A04] 判断变量类型
来源：http://cr.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rb.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fv.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mw.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://wq.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nh.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://im.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://up.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://lr.lnxyls.cn

[A05] 整数除法与取模
来源：http://ih.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dt.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jv.muxihuayi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xe.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zd.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://jl.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://fs.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://pu.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://fp.wgjwhj.cn

[A06] 字符串转数字
来源：http://ip.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://lp.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xz.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bh.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bh.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://js.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sg.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ne.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gi.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://tp.jctech888.com.cn

Py:   str(42)
来源：http://of.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://hl.nszjky.cn

JS:   String(42); (42).toString()
来源：http://rs.newstarts.cn

TS:   String(42)
来源：http://de.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hg.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://mo.shxzskj.cn

Ruby: 42.to_s
来源：http://dc.wgjwhj.cn

C#:   42.ToString()
来源：http://wa.gzmigu.cn

[A08] 取整与四舍五入
来源：http://rl.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ht.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ss.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jf.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ck.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mo.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tb.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://po.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zc.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://fc.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zx.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lm.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tq.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rj.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vg.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ww.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xp.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ac.haigaiapp.cn

[A10] 生成随机数
来源：http://zp.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://vo.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://zn.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bn.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dt.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://zp.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eg.hnjuh.cn

Ruby: rand(1..100)
来源：http://lb.521024.cn

C#:   new Random().Next(1, 101)
来源：http://lk.521024.cn

[A11] 条件表达式（三元）
来源：http://wo.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://tp.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kl.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gg.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qo.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://hg.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ib.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fd.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gr.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://pd.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qa.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xg.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://zq.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://eo.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ah.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mw.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://yd.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://zm.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ic.hahajie.cn

Py:   "第一行\n第二行"
来源：http://fu.colortex.cn

PHP:  "第一行\n第二行"
来源：http://hp.nszjky.cn

JS:   "第一行\n第二行"
来源：http://pi.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://xs.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://ym.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://df.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://zn.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://nh.yuntaijiaju.cn

[A14] 注释写法
来源：http://vn.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pq.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://md.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://es.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://te.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lz.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://if.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://om.szsharing.cn


<!-- 参考信息 -->