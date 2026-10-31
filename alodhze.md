代发 wailian999

[U87] JS：解构默认值
来源：http://gt.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://yj.newstarts.cn

[U88] JS：对象展开合并
来源：http://bx.yuntaijiaju.cn

{ ...a, ...b }
来源：http://bv.newstarts.cn

[U89] JS：数组去重
来源：http://me.muxihuayi.cn

[...new Set(arr)]
来源：http://eh.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://cc.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://et.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ez.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gq.521024.cn

[U92] JS：深拷贝
来源：http://jw.nicolike.cn

structuredClone(obj)
来源：http://cb.9csxet.cn

[U93] JS：模板字符串
来源：http://ic.yuexingan06.cn

`共 ${n} 条`
来源：http://ly.shxzskj.cn

[U94] JS：箭头函数
来源：http://vc.panjiajie.cn

const double = x => x * 2;
来源：http://ge.colortex.cn

[U95] JS：Promise 包装
来源：http://ko.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://aj.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://qb.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ek.nicolike.cn

[U97] JS：并发请求
来源：http://ta.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ia.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://mx.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sx.chemitech.net.cn

[U99] JS：事件监听
来源：http://se.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://xo.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://em.szxytkj.cn

document.querySelector(".item")
来源：http://tm.hnjuh.cn

[U101] JS：classList 操作
来源：http://ka.newstarts.cn

el.classList.toggle("active")
来源：http://ah.chemitech.net.cn

[U102] JS：本地存储
来源：http://ri.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ai.szxytkj.cn

[U103] JS：定时器
来源：http://or.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ml.szsharing.cn

[U104] JS：防抖
来源：http://mc.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bk.shxzskj.cn

[U105] JS：节流
来源：http://zg.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wn.huixiangedu.cn

[U106] JS：日期格式化
来源：http://rp.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dn.colortex.cn

[U107] JS：数字千分位
来源：http://ix.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hl.shxzskj.cn

[U108] JS：随机整数
来源：http://tv.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lx.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://bh.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://uf.panjiajie.cn

[U110] JS：数组分块
来源：http://pw.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://st.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://za.szxytkj.cn

new Map(Object.entries(obj))
来源：http://oe.nszjky.cn

[U112] JS：字符串补位
来源：http://ds.newstarts.cn

"7".padStart(3, "0")
来源：http://gf.newstarts.cn

[U113] JS：正则替换全部
来源：http://co.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://ui.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://rz.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qa.asd995.cn

[U115] JS：生成 UUID
来源：http://cc.haigaiapp.cn

crypto.randomUUID()
来源：http://ee.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://nv.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://uu.9csxet.cn

[U117] JS：单元测试
来源：http://mq.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://zl.shtwfgs.cn

[U118] JS：开发服务器
来源：http://pr.bookmarksfly.cn

npm i -D vite;  npx vite
来源：http://hb.9csxet.cn

[U119] JS：生产构建
来源：http://yz.shxzukj.cn

npx vite build
来源：http://gq.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://hk.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://mw.haigaiapp.cn

================================================================================
来源：http://ju.lnxyls.cn

统计汇总
来源：http://ky.muxihuayi.cn

================================================================================
来源：http://cq.szsharing.cn

按语言统计（条）：
来源：http://wu.huixiangedu.cn

Python ......... 252
来源：http://rj.yuntaijiaju.cn

PHP ............ 252
来源：http://hc.bookmarksfly.cn

JavaScript ..... 252
来源：http://nb.jianghongdianzi.cn

TypeScript ..... 212
来源：http://je.szxytkj.cn

Java ........... 212
来源：http://pr.newstarts.cn

Go ............. 212
来源：http://hi.shxzskj.cn

Ruby ........... 212
来源：http://ww.hahajie.cn

C# ............. 212
来源：http://dw.lnxyls.cn

C .............. 30
来源：http://df.huanxung.cn

C++ ............ 30
来源：http://bv.muxihuayi.cn

SQL ............ 90
来源：http://or.asd995.cn

Bash ........... 80
来源：http://wn.wgjwhj.cn

Kotlin ......... 15
来源：http://pn.panjiajie.cn

Swift .......... 15
来源：http://vi.wgjwhj.cn

Lua ............ 10
来源：http://yv.newstarts.cn

Perl ........... 10
来源：http://bc.jianghongdianzi.cn

Scala .......... 10
来源：http://cr.shxzskj.cn

------------------------------------
来源：http://nn.bjjhwx.cn

合计 ........... 2106 条
来源：http://ba.muxihuayi.cn

按章节统计：
来源：http://ug.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ii.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ca.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hq.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fe.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cd.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://si.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xl.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cd.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://av.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uy.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fb.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://li.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kr.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cf.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qp.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rp.panjiajie.cn

Q SQL 专题                              90
来源：http://wk.gzmigu.cn

R Bash 专题                             80
来源：http://rq.nszjky.cn

S C / C++ 专题                          60
来源：http://gp.nicolike.cn

T 其他语言补充                          60
来源：http://cw.bjjhwx.cn

U 高频实用片段                         120
来源：http://ux.szsharing.cn

------------------------------------
来源：http://gb.shxzukj.cn

合计                                  2106 条
来源：http://ia.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://hs.shxzukj.cn

使用提醒
来源：http://ic.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://zt.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ax.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ma.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://em.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qd.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zn.newstarts.cn

—— 文件结束 ——
来源：http://zz.shxzskj.cn

================================================================================
来源：http://el.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://yv.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://hx.colortex.cn

================================================================================
来源：http://xh.huanxung.cn

【收录内容】
来源：http://hu.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ih.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wl.shxzukj.cn

SQL · Bash · C · C++
来源：http://in.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hi.yuexingan06.cn

【使用说明】
来源：http://gg.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cu.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hy.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ht.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gf.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vn.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iv.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ln.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pq.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tk.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bm.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ec.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dh.shxzukj.cn

【文件统计】
来源：http://pe.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jg.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://hu.bookmarksfly.cn

目  录
来源：http://ed.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://vt.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dr.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gl.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mu.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://td.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wn.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pf.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://se.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://df.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zo.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sc.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vu.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zi.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mq.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wr.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tx.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lr.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ib.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rj.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nz.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fa.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ph.shtwfgs.cn

================================================================================
来源：http://ph.jctech888.com.cn

A. 基础语法与类型
来源：http://un.jctech888.com.cn

================================================================================
来源：http://in.panjiajie.cn

[A01] Hello World
来源：http://mb.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://lw.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://ta.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://su.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gk.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://en.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ba.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://hy.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://db.521024.cn

[A02] 变量声明与赋值
来源：http://hj.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cl.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lq.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cj.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sp.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://mn.521024.cn

Go:   name := "Alex"; age := 20
来源：http://md.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://ct.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cg.haigaiapp.cn

[A03] 常量定义
来源：http://rq.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uq.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://ox.newstarts.cn

JS:   const PI = 3.14159;
来源：http://wx.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://cm.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://rw.lnxyls.cn

Go:   const PI = 3.14159
来源：http://nu.colortex.cn

Ruby: PI = 3.14159
来源：http://ta.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://kl.szsharing.cn

[A04] 判断变量类型
来源：http://pd.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zo.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bf.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lw.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://jb.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sz.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ay.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ui.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://od.huanxung.cn

[A05] 整数除法与取模
来源：http://bi.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gq.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wx.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://he.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dp.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://iu.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://ak.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://yh.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://ja.bookmarksfly.cn

[A06] 字符串转数字
来源：http://qx.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://je.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nt.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bv.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mc.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ni.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lw.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://na.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://st.huanxung.cn

[A07] 数字转字符串
来源：http://cn.szsharing.cn

Py:   str(42)
来源：http://hs.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://dh.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://ys.lnxyls.cn

TS:   String(42)
来源：http://qi.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zu.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://tx.muxihuayi.cn

Ruby: 42.to_s
来源：http://qe.lnxyls.cn

C#:   42.ToString()
来源：http://hx.lnxyls.cn

[A08] 取整与四舍五入
来源：http://eo.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zm.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wi.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://me.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mk.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wc.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ps.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nq.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qj.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://um.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mv.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ng.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oi.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vg.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://br.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yr.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tl.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uy.hahajie.cn

[A10] 生成随机数
来源：http://qf.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://rm.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://pa.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hy.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fj.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://me.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qr.shxzskj.cn

Ruby: rand(1..100)
来源：http://ht.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://um.huanxung.cn

[A11] 条件表达式（三元）
来源：http://mc.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://sq.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fu.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nd.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gj.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://je.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ov.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://um.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bh.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://iu.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zr.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://km.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://nf.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://vs.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://nw.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ol.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://wz.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://iz.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rm.newstarts.cn

Py:   "第一行\n第二行"
来源：http://mj.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://ct.521024.cn

JS:   "第一行\n第二行"
来源：http://fa.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://da.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://zm.colortex.cn

Go:   "第一行\n第二行"
来源：http://vw.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://rp.9csxet.cn

C#:   "第一行\n第二行"
来源：http://hf.jctech888.com.cn

[A14] 注释写法
来源：http://uo.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fy.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://un.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://do.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://et.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qc.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://gi.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nj.521024.cn


<!-- 参考信息 -->