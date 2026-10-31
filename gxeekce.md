代发 wailian999

[U91] JS：对象键值遍历
来源：http://nf.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ad.9csxet.cn

[U92] JS：深拷贝
来源：http://yi.huanxung.cn

structuredClone(obj)
来源：http://rr.szxytkj.cn

[U93] JS：模板字符串
来源：http://hl.panjiajie.cn

`共 ${n} 条`
来源：http://kq.muxihuayi.cn

[U94] JS：箭头函数
来源：http://in.yuexingan06.cn

const double = x => x * 2;
来源：http://dn.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ji.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://jj.521024.cn

[U96] JS：async/await 与异常
来源：http://ps.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ao.huixiangedu.cn

[U97] JS：并发请求
来源：http://wg.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dn.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ux.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ki.huixiangedu.cn

[U99] JS：事件监听
来源：http://hq.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://xs.colortex.cn

[U100] JS：DOM 查询
来源：http://mi.hnjuh.cn

document.querySelector(".item")
来源：http://do.lnxyls.cn

[U101] JS：classList 操作
来源：http://ty.huixiangedu.cn

el.classList.toggle("active")
来源：http://ie.nszjky.cn

[U102] JS：本地存储
来源：http://dw.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qs.nszjky.cn

[U103] JS：定时器
来源：http://ie.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zg.panjiajie.cn

[U104] JS：防抖
来源：http://rd.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.shtwfgs.cn

[U105] JS：节流
来源：http://su.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yi.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://tj.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yb.huanxung.cn

[U107] JS：数字千分位
来源：http://la.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jb.9csxet.cn

[U108] JS：随机整数
来源：http://se.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pi.colortex.cn

[U109] JS：数组分组
来源：http://yi.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://wx.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://ra.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pr.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ix.hahajie.cn

new Map(Object.entries(obj))
来源：http://fc.nicolike.cn

[U112] JS：字符串补位
来源：http://rd.bjjhwx.cn

"7".padStart(3, "0")
来源：http://op.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://uq.gzmigu.cn

s.replaceAll("a", "b")
来源：http://fo.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://yl.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mo.panjiajie.cn

[U115] JS：生成 UUID
来源：http://cf.shtwfgs.cn

crypto.randomUUID()
来源：http://df.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://ha.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://sg.shtwfgs.cn

[U117] JS：单元测试
来源：http://xk.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://uy.yuexingan06.cn

[U118] JS：开发服务器
来源：http://ez.huanxung.cn

npm i -D vite;  npx vite
来源：http://hq.nicolike.cn

[U119] JS：生产构建
来源：http://xh.asd995.cn

npx vite build
来源：http://dv.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://rx.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://te.shxzskj.cn

================================================================================
来源：http://od.muxihuayi.cn

统计汇总
来源：http://jw.chemitech.net.cn

================================================================================
来源：http://uq.wgjwhj.cn

按语言统计（条）：
来源：http://ex.gzmigu.cn

Python ......... 252
来源：http://zs.colortex.cn

PHP ............ 252
来源：http://wy.huanxung.cn

JavaScript ..... 252
来源：http://uv.shxzukj.cn

TypeScript ..... 212
来源：http://uw.wgjwhj.cn

Java ........... 212
来源：http://dt.huixiangedu.cn

Go ............. 212
来源：http://lc.yuntaijiaju.cn

Ruby ........... 212
来源：http://vl.nszjky.cn

C# ............. 212
来源：http://ww.asd995.cn

C .............. 30
来源：http://gz.jctech888.com.cn

C++ ............ 30
来源：http://bx.nicolike.cn

SQL ............ 90
来源：http://gi.wgjwhj.cn

Bash ........... 80
来源：http://aw.bookmarksfly.cn

Kotlin ......... 15
来源：http://ss.jctech888.com.cn

Swift .......... 15
来源：http://wi.hahajie.cn

Lua ............ 10
来源：http://hs.shxzskj.cn

Perl ........... 10
来源：http://ys.muxihuayi.cn

Scala .......... 10
来源：http://zd.panjiajie.cn

------------------------------------
来源：http://kg.muxihuayi.cn

合计 ........... 2106 条
来源：http://jg.panjiajie.cn

按章节统计：
来源：http://ow.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://li.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ty.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qz.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sl.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fp.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://od.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ll.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ud.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cm.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pl.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jy.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://em.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nl.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ic.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pv.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ny.shtwfgs.cn

Q SQL 专题                              90
来源：http://sf.9csxet.cn

R Bash 专题                             80
来源：http://rn.9csxet.cn

S C / C++ 专题                          60
来源：http://ym.shxzskj.cn

T 其他语言补充                          60
来源：http://fw.yuexingan06.cn

U 高频实用片段                         120
来源：http://uy.huixinmuqiang.cn

------------------------------------
来源：http://hb.asd995.cn

合计                                  2106 条
来源：http://nf.newstarts.cn

--------------------------------------------------------------------------------
来源：http://uw.bookmarksfly.cn

使用提醒
来源：http://uj.nszjky.cn

--------------------------------------------------------------------------------
来源：http://qp.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://re.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oo.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mq.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vy.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fp.panjiajie.cn

—— 文件结束 ——
来源：http://ny.chemitech.net.cn

================================================================================
来源：http://hu.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://lg.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://cb.bjjhwx.cn

================================================================================
来源：http://hv.lnxyls.cn

【收录内容】
来源：http://ne.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jg.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ek.nszjky.cn

SQL · Bash · C · C++
来源：http://ad.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ib.haigaiapp.cn

【使用说明】
来源：http://wz.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://np.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oh.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wk.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fj.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ow.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uk.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gu.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yc.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zj.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qw.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cd.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jianghongdianzi.cn

【文件统计】
来源：http://za.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://js.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://tt.shxzukj.cn

目  录
来源：http://or.newstarts.cn

--------------------------------------------------------------------------------
来源：http://bo.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://at.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jk.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ho.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ht.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mx.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xe.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nl.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xd.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xk.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yz.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zb.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gy.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mn.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zm.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://db.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cb.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vt.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ki.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zv.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wq.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iu.asd995.cn

================================================================================
来源：http://zf.panjiajie.cn

A. 基础语法与类型
来源：http://yp.jianghongdianzi.cn

================================================================================
来源：http://vq.shxzukj.cn

[A01] Hello World
来源：http://wf.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://sa.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://vv.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://lf.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zz.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://ea.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ec.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://mo.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bw.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://ni.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ct.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tb.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dh.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gm.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://bj.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://jy.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://xu.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yl.colortex.cn

[A03] 常量定义
来源：http://tu.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ag.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://oe.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://ph.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://dz.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://ts.szsharing.cn

Go:   const PI = 3.14159
来源：http://ul.shxzukj.cn

Ruby: PI = 3.14159
来源：http://jt.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://jr.nszjky.cn

[A04] 判断变量类型
来源：http://te.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yq.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lu.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://si.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://os.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yz.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ez.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yx.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://nc.haigaiapp.cn

[A05] 整数除法与取模
来源：http://de.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ua.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ys.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://al.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rh.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://ao.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://oz.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://wf.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://aj.colortex.cn

[A06] 字符串转数字
来源：http://ul.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://yo.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kz.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pf.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sw.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ua.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gg.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://up.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sa.chemitech.net.cn

[A07] 数字转字符串
来源：http://iw.jctech888.com.cn

Py:   str(42)
来源：http://ak.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://yl.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://op.wgjwhj.cn

TS:   String(42)
来源：http://po.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hb.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://po.newstarts.cn

Ruby: 42.to_s
来源：http://yz.gzmigu.cn

C#:   42.ToString()
来源：http://hv.521024.cn

[A08] 取整与四舍五入
来源：http://tm.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wl.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fz.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gp.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gf.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cx.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gv.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zd.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sy.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://lq.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ti.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qa.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fd.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ox.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://os.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mw.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rd.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qi.chemitech.net.cn

[A10] 生成随机数
来源：http://xl.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://xa.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ue.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ft.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bz.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ls.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gp.haigaiapp.cn

Ruby: rand(1..100)
来源：http://kd.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://ki.asd995.cn

[A11] 条件表达式（三元）
来源：http://iq.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://mo.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ot.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jl.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qj.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://fk.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jd.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yr.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eu.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://bj.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ga.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jd.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://fb.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://qd.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://mn.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lf.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://gq.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://py.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jy.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://vt.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://vg.521024.cn

JS:   "第一行\n第二行"
来源：http://is.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://ig.huanxung.cn

Java: "第一行\n第二行"
来源：http://qb.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ph.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://vq.521024.cn

C#:   "第一行\n第二行"
来源：http://kx.shxzukj.cn

[A14] 注释写法
来源：http://vy.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yz.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pn.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://ry.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://kp.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://je.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://rj.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yn.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://il.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://aq.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://jc.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://bv.521024.cn

JS:   const value = data ?? "默认值";
来源：http://dv.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://sq.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ee.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://tg.muxihuayi.cn


<!-- 参考信息 -->