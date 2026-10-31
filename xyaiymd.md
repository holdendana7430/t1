代发 wailian999

[U97] JS：并发请求
来源：http://pb.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dm.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ni.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://is.szxytkj.cn

[U99] JS：事件监听
来源：http://ie.newstarts.cn

el.addEventListener("click", e => {})
来源：http://cw.asd995.cn

[U100] JS：DOM 查询
来源：http://ti.hnjuh.cn

document.querySelector(".item")
来源：http://uh.bjjhwx.cn

[U101] JS：classList 操作
来源：http://ce.bookmarksfly.cn

el.classList.toggle("active")
来源：http://te.chemitech.net.cn

[U102] JS：本地存储
来源：http://he.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wk.panjiajie.cn

[U103] JS：定时器
来源：http://cj.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ng.huixinmuqiang.cn

[U104] JS：防抖
来源：http://dp.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tw.huixinmuqiang.cn

[U105] JS：节流
来源：http://fp.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ea.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ud.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vv.colortex.cn

[U107] JS：数字千分位
来源：http://bh.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cx.shxzskj.cn

[U108] JS：随机整数
来源：http://by.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://we.shxzskj.cn

[U109] JS：数组分组
来源：http://rt.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://cr.chemitech.net.cn

[U110] JS：数组分块
来源：http://qo.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yi.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://lk.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://wk.wgjwhj.cn

[U112] JS：字符串补位
来源：http://bb.hnjuh.cn

"7".padStart(3, "0")
来源：http://ll.asd995.cn

[U113] JS：正则替换全部
来源：http://rq.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://fw.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://pn.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bw.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://sn.nicolike.cn

crypto.randomUUID()
来源：http://wd.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://kr.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://zy.chemitech.net.cn

[U117] JS：单元测试
来源：http://te.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://cv.huixiangedu.cn

[U118] JS：开发服务器
来源：http://sw.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://py.gzmigu.cn

[U119] JS：生产构建
来源：http://hm.huixinmuqiang.cn

npx vite build
来源：http://pb.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ty.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://ou.hnjuh.cn

================================================================================
来源：http://zy.panjiajie.cn

统计汇总
来源：http://rd.colortex.cn

================================================================================
来源：http://wd.bookmarksfly.cn

按语言统计（条）：
来源：http://if.szsharing.cn

Python ......... 252
来源：http://hh.colortex.cn

PHP ............ 252
来源：http://vd.wgjwhj.cn

JavaScript ..... 252
来源：http://wx.bjjhwx.cn

TypeScript ..... 212
来源：http://jq.bjjhwx.cn

Java ........... 212
来源：http://li.muxihuayi.cn

Go ............. 212
来源：http://yd.huanxung.cn

Ruby ........... 212
来源：http://ik.nszjky.cn

C# ............. 212
来源：http://wg.jctech888.com.cn

C .............. 30
来源：http://pc.chemitech.net.cn

C++ ............ 30
来源：http://dc.nszjky.cn

SQL ............ 90
来源：http://sy.shxzukj.cn

Bash ........... 80
来源：http://si.chemitech.net.cn

Kotlin ......... 15
来源：http://di.huanxung.cn

Swift .......... 15
来源：http://ny.hnjuh.cn

Lua ............ 10
来源：http://qq.huixinmuqiang.cn

Perl ........... 10
来源：http://to.9csxet.cn

Scala .......... 10
来源：http://wy.szxytkj.cn

------------------------------------
来源：http://hv.gzmigu.cn

合计 ........... 2106 条
来源：http://xv.gzmigu.cn

按章节统计：
来源：http://mj.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sh.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gf.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zb.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gi.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ft.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ez.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hx.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xp.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bq.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ho.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://db.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rk.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iq.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rz.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oh.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lx.colortex.cn

Q SQL 专题                              90
来源：http://zz.szxytkj.cn

R Bash 专题                             80
来源：http://st.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://oe.nicolike.cn

T 其他语言补充                          60
来源：http://ei.huixiangedu.cn

U 高频实用片段                         120
来源：http://kf.panjiajie.cn

------------------------------------
来源：http://rq.wgjwhj.cn

合计                                  2106 条
来源：http://di.9csxet.cn

--------------------------------------------------------------------------------
来源：http://uo.huixinmuqiang.cn

使用提醒
来源：http://st.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://hd.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kn.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gz.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qr.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dl.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mj.gzmigu.cn

—— 文件结束 ——
来源：http://mi.colortex.cn

================================================================================
来源：http://mn.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ok.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://gi.shxzukj.cn

================================================================================
来源：http://ky.lnxyls.cn

【收录内容】
来源：http://vn.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vp.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pf.asd995.cn

SQL · Bash · C · C++
来源：http://ok.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tu.bookmarksfly.cn

【使用说明】
来源：http://no.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cr.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qs.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://or.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ta.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nw.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ca.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lz.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jx.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nh.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qd.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pw.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dz.yuntaijiaju.cn

【文件统计】
来源：http://iv.lnxyls.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ce.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://rk.szsharing.cn

目  录
来源：http://bt.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ca.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://al.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mn.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xf.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cn.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hg.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ko.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rx.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ue.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://go.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pz.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hj.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ai.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ft.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://us.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rz.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://af.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ih.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kh.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mj.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bv.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yh.shxzukj.cn

================================================================================
来源：http://or.huixinmuqiang.cn

A. 基础语法与类型
来源：http://pk.huixinmuqiang.cn

================================================================================
来源：http://dx.lnxyls.cn

[A01] Hello World
来源：http://fe.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://ir.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://kg.yuntaijiaju.cn

JS:   console.log("Hello, World!");
来源：http://lj.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ei.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://vi.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://xh.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://so.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nf.hahajie.cn

[A02] 变量声明与赋值
来源：http://qy.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wc.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rh.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xr.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gz.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://kh.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://ps.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://pm.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wm.muxihuayi.cn

[A03] 常量定义
来源：http://yo.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jv.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://da.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ju.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://rs.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://yv.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://df.nszjky.cn

Ruby: PI = 3.14159
来源：http://pu.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://sy.bookmarksfly.cn

[A04] 判断变量类型
来源：http://ar.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ol.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vh.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dz.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://hf.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ye.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vl.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iu.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://ya.asd995.cn

[A05] 整数除法与取模
来源：http://ld.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nk.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fx.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rz.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tv.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://uj.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://pg.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hz.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://hy.asd995.cn

[A06] 字符串转数字
来源：http://he.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://hm.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gy.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://om.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yy.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vn.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ft.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ir.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iz.shxzskj.cn

[A07] 数字转字符串
来源：http://tc.szsharing.cn

Py:   str(42)
来源：http://du.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://fs.newstarts.cn

JS:   String(42); (42).toString()
来源：http://tm.521024.cn

TS:   String(42)
来源：http://rd.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lf.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://zi.huanxung.cn

Ruby: 42.to_s
来源：http://mm.nszjky.cn

C#:   42.ToString()
来源：http://il.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://hs.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jr.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vq.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mt.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jp.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jg.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sy.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pv.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gi.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://cj.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lu.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wd.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oi.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://od.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dx.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sk.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://py.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sf.nicolike.cn

[A10] 生成随机数
来源：http://fq.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://bh.9csxet.cn

PHP:  random_int(1, 100);
来源：http://yx.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ga.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fx.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://sa.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oe.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://fl.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://go.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://as.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://uv.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wz.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ew.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ze.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://jj.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://at.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kb.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kr.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://nv.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xp.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wc.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://wn.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://rg.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://bp.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fg.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://fa.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://bd.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wa.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://dg.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://xp.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://df.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://po.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ck.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bt.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://mf.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://cg.panjiajie.cn

[A14] 注释写法
来源：http://tw.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fk.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zk.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://uj.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://qx.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fg.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://vt.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ws.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://xo.9csxet.cn

[A15] 空值判断与默认值
来源：http://fg.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://zn.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://rt.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://vx.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ya.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vq.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://qe.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://hw.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://oa.jctech888.com.cn

[A16] 真假值判断规则
来源：http://bi.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lp.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wd.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wq.newstarts.cn

TS:   if (!x) {}
来源：http://ec.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bi.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gq.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vm.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nx.huixiangedu.cn

[A17] 位运算
来源：http://er.wgjwhj.cn


<!-- 参考信息 -->