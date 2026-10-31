代发 wailian999

[U87] JS：解构默认值
来源：http://fj.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://kg.hahajie.cn

[U88] JS：对象展开合并
来源：http://oy.hahajie.cn

{ ...a, ...b }
来源：http://kj.jctech888.com.cn

[U89] JS：数组去重
来源：http://na.shtwfgs.cn

[...new Set(arr)]
来源：http://ou.newstarts.cn

[U90] JS：数字数组排序
来源：http://ie.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://iq.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://jo.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://me.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://tg.colortex.cn

structuredClone(obj)
来源：http://tl.shtwfgs.cn

[U93] JS：模板字符串
来源：http://hv.muxihuayi.cn

`共 ${n} 条`
来源：http://vp.shtwfgs.cn

[U94] JS：箭头函数
来源：http://yj.huanxung.cn

const double = x => x * 2;
来源：http://xc.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ed.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://fc.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://zd.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vr.colortex.cn

[U97] JS：并发请求
来源：http://om.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://ae.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xr.panjiajie.cn

[U99] JS：事件监听
来源：http://ry.huanxung.cn

el.addEventListener("click", e => {})
来源：http://fw.asd995.cn

[U100] JS：DOM 查询
来源：http://fr.huixinmuqiang.cn

document.querySelector(".item")
来源：http://qd.huixiangedu.cn

[U101] JS：classList 操作
来源：http://fc.haigaiapp.cn

el.classList.toggle("active")
来源：http://ij.shtwfgs.cn

[U102] JS：本地存储
来源：http://dv.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hn.colortex.cn

[U103] JS：定时器
来源：http://co.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kz.lnxyls.cn

[U104] JS：防抖
来源：http://be.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cd.lnxyls.cn

[U105] JS：节流
来源：http://lc.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wa.lnxyls.cn

[U106] JS：日期格式化
来源：http://wd.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mj.haigaiapp.cn

[U107] JS：数字千分位
来源：http://ql.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xm.gzmigu.cn

[U108] JS：随机整数
来源：http://yw.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://be.szxytkj.cn

[U109] JS：数组分组
来源：http://kb.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ud.haigaiapp.cn

[U110] JS：数组分块
来源：http://ac.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xe.asd995.cn

[U111] JS：对象转 Map
来源：http://ci.lnxyls.cn

new Map(Object.entries(obj))
来源：http://vz.huanxung.cn

[U112] JS：字符串补位
来源：http://oz.haigaiapp.cn

"7".padStart(3, "0")
来源：http://vm.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ac.521024.cn

s.replaceAll("a", "b")
来源：http://po.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://aq.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dn.shxzskj.cn

[U115] JS：生成 UUID
来源：http://tk.lnxyls.cn

crypto.randomUUID()
来源：http://lv.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://am.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://or.bjjhwx.cn

[U117] JS：单元测试
来源：http://rh.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://oy.panjiajie.cn

[U118] JS：开发服务器
来源：http://xd.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://vl.lnxyls.cn

[U119] JS：生产构建
来源：http://gr.bjjhwx.cn

npx vite build
来源：http://aw.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://xf.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://pc.haigaiapp.cn

================================================================================
来源：http://ch.szsharing.cn

统计汇总
来源：http://ad.shtwfgs.cn

================================================================================
来源：http://en.bookmarksfly.cn

按语言统计（条）：
来源：http://pf.hnjuh.cn

Python ......... 252
来源：http://vm.9csxet.cn

PHP ............ 252
来源：http://kl.jctech888.com.cn

JavaScript ..... 252
来源：http://sa.nszjky.cn

TypeScript ..... 212
来源：http://od.newstarts.cn

Java ........... 212
来源：http://rn.colortex.cn

Go ............. 212
来源：http://kj.asd995.cn

Ruby ........... 212
来源：http://vk.521024.cn

C# ............. 212
来源：http://ot.muxihuayi.cn

C .............. 30
来源：http://sr.muxihuayi.cn

C++ ............ 30
来源：http://wg.shtwfgs.cn

SQL ............ 90
来源：http://ks.521024.cn

Bash ........... 80
来源：http://ie.muxihuayi.cn

Kotlin ......... 15
来源：http://yz.szxytkj.cn

Swift .......... 15
来源：http://am.chemitech.net.cn

Lua ............ 10
来源：http://sx.nszjky.cn

Perl ........... 10
来源：http://il.lnxyls.cn

Scala .......... 10
来源：http://jh.newstarts.cn

------------------------------------
来源：http://nb.nszjky.cn

合计 ........... 2106 条
来源：http://ty.colortex.cn

按章节统计：
来源：http://hk.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ym.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hw.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sa.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qx.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sy.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mi.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ej.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zy.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wf.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qn.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uw.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ff.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qu.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fb.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://du.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pz.huixiangedu.cn

Q SQL 专题                              90
来源：http://sh.wgjwhj.cn

R Bash 专题                             80
来源：http://oy.nszjky.cn

S C / C++ 专题                          60
来源：http://hf.jctech888.com.cn

T 其他语言补充                          60
来源：http://px.panjiajie.cn

U 高频实用片段                         120
来源：http://tc.bookmarksfly.cn

------------------------------------
来源：http://fa.huixinmuqiang.cn

合计                                  2106 条
来源：http://dt.colortex.cn

--------------------------------------------------------------------------------
来源：http://ld.bjjhwx.cn

使用提醒
来源：http://bx.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://km.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://le.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jm.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uv.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qh.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fg.shtwfgs.cn

—— 文件结束 ——
来源：http://yg.szxytkj.cn

================================================================================
来源：http://vz.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://bf.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://cd.newstarts.cn

================================================================================
来源：http://wt.wgjwhj.cn

【收录内容】
来源：http://sm.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iy.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://se.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://yz.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pr.jianghongdianzi.cn

【使用说明】
来源：http://ps.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vp.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vj.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nj.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ol.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cr.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jq.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yl.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hd.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lt.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bn.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ik.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hh.muxihuayi.cn

【文件统计】
来源：http://xh.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cw.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hk.lnxyls.cn

目  录
来源：http://rj.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zd.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oc.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jq.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jm.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cy.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gk.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wh.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ol.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gb.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pl.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aw.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fb.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pi.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ny.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://br.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zk.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xo.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gk.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ot.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rc.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ai.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hq.newstarts.cn

================================================================================
来源：http://tv.muxihuayi.cn

A. 基础语法与类型
来源：http://zt.shxzukj.cn

================================================================================
来源：http://ga.9csxet.cn

[A01] Hello World
来源：http://cj.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ap.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://bl.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://ln.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cd.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://ag.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://bz.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://bz.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fo.huanxung.cn

[A02] 变量声明与赋值
来源：http://oz.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zd.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zn.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kc.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ho.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://vj.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ho.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://ka.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tt.jctech888.com.cn

[A03] 常量定义
来源：http://xi.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ns.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://rk.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://hj.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://sq.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://qj.hnjuh.cn

Go:   const PI = 3.14159
来源：http://ei.asd995.cn

Ruby: PI = 3.14159
来源：http://on.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://pl.hnjuh.cn

[A04] 判断变量类型
来源：http://ia.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ha.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mr.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xm.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://jj.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ix.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gh.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ba.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://wv.szsharing.cn

[A05] 整数除法与取模
来源：http://qr.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hd.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fg.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oy.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nl.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://ok.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://ls.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://tb.521024.cn

C#:   7 / 2; 7 % 2
来源：http://wk.colortex.cn

[A06] 字符串转数字
来源：http://ey.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://dg.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wa.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yl.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ly.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ir.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fd.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ms.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hx.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://jj.asd995.cn

Py:   str(42)
来源：http://cf.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://ql.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://pp.asd995.cn

TS:   String(42)
来源：http://iw.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zs.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://lh.bjjhwx.cn

Ruby: 42.to_s
来源：http://ft.wgjwhj.cn

C#:   42.ToString()
来源：http://og.asd995.cn

[A08] 取整与四舍五入
来源：http://ri.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://to.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wp.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cm.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qv.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bh.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ug.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://au.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cj.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://yr.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cs.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bi.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jz.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qu.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ft.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qf.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mo.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://st.9csxet.cn

[A10] 生成随机数
来源：http://ke.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ny.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://th.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zd.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ur.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://wr.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qa.hahajie.cn

Ruby: rand(1..100)
来源：http://cz.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://dq.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://zv.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://lk.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kk.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qk.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mi.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wt.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nk.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dm.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ht.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://na.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kf.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ai.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://lp.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ot.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ky.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://em.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://jd.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://zb.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ol.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://cy.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://he.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://ec.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://rg.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://bt.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://ug.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://lf.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://zc.haigaiapp.cn

[A14] 注释写法
来源：http://td.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gy.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://id.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://rw.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://sl.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kb.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://af.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://me.jianghongdianzi.cn


<!-- 参考信息 -->