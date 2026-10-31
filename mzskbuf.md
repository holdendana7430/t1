代发 wailian999

[U85] JS：可选链
来源：http://ns.szxytkj.cn

a?.b?.c
来源：http://kc.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://rv.shxzukj.cn

a ?? b
来源：http://ot.nszjky.cn

[U87] JS：解构默认值
来源：http://ci.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://km.9csxet.cn

[U88] JS：对象展开合并
来源：http://it.huixiangedu.cn

{ ...a, ...b }
来源：http://im.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://om.nszjky.cn

[...new Set(arr)]
来源：http://gj.nicolike.cn

[U90] JS：数字数组排序
来源：http://pc.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://ek.colortex.cn

[U91] JS：对象键值遍历
来源：http://ej.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://su.nicolike.cn

[U92] JS：深拷贝
来源：http://ax.haigaiapp.cn

structuredClone(obj)
来源：http://wq.bjjhwx.cn

[U93] JS：模板字符串
来源：http://dr.bjjhwx.cn

`共 ${n} 条`
来源：http://yw.hnjuh.cn

[U94] JS：箭头函数
来源：http://wv.muxihuayi.cn

const double = x => x * 2;
来源：http://cq.newstarts.cn

[U95] JS：Promise 包装
来源：http://wy.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ln.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://qw.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://je.nicolike.cn

[U97] JS：并发请求
来源：http://ad.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ce.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://ba.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gl.9csxet.cn

[U99] JS：事件监听
来源：http://st.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://rp.shxzukj.cn

[U100] JS：DOM 查询
来源：http://vo.asd995.cn

document.querySelector(".item")
来源：http://kb.gzmigu.cn

[U101] JS：classList 操作
来源：http://ip.gzmigu.cn

el.classList.toggle("active")
来源：http://fq.nicolike.cn

[U102] JS：本地存储
来源：http://mx.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pw.shtwfgs.cn

[U103] JS：定时器
来源：http://hd.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fm.jianghongdianzi.cn

[U104] JS：防抖
来源：http://ge.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mn.nicolike.cn

[U105] JS：节流
来源：http://dh.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cg.szsharing.cn

[U106] JS：日期格式化
来源：http://yw.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ju.nszjky.cn

[U107] JS：数字千分位
来源：http://wt.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fy.asd995.cn

[U108] JS：随机整数
来源：http://fr.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nh.bookmarksfly.cn

[U109] JS：数组分组
来源：http://mk.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://ku.yuexingan06.cn

[U110] JS：数组分块
来源：http://kp.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sm.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://tp.shxzukj.cn

new Map(Object.entries(obj))
来源：http://gw.szxytkj.cn

[U112] JS：字符串补位
来源：http://pc.lnxyls.cn

"7".padStart(3, "0")
来源：http://xc.huanxung.cn

[U113] JS：正则替换全部
来源：http://js.shxzskj.cn

s.replaceAll("a", "b")
来源：http://ko.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://em.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ds.nszjky.cn

[U115] JS：生成 UUID
来源：http://tj.muxihuayi.cn

crypto.randomUUID()
来源：http://cr.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://kj.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://bl.chemitech.net.cn

[U117] JS：单元测试
来源：http://ze.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://cm.colortex.cn

[U118] JS：开发服务器
来源：http://ic.gzmigu.cn

npm i -D vite;  npx vite
来源：http://gn.nszjky.cn

[U119] JS：生产构建
来源：http://tp.haigaiapp.cn

npx vite build
来源：http://vr.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://lo.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://jj.colortex.cn

================================================================================
来源：http://gr.nszjky.cn

统计汇总
来源：http://st.asd995.cn

================================================================================
来源：http://dt.yuntaijiaju.cn

按语言统计（条）：
来源：http://lt.bookmarksfly.cn

Python ......... 252
来源：http://qt.huixinmuqiang.cn

PHP ............ 252
来源：http://se.shtwfgs.cn

JavaScript ..... 252
来源：http://oc.521024.cn

TypeScript ..... 212
来源：http://pr.szsharing.cn

Java ........... 212
来源：http://ws.shxzskj.cn

Go ............. 212
来源：http://su.shxzukj.cn

Ruby ........... 212
来源：http://fa.szsharing.cn

C# ............. 212
来源：http://wy.haigaiapp.cn

C .............. 30
来源：http://il.yuexingan06.cn

C++ ............ 30
来源：http://at.nicolike.cn

SQL ............ 90
来源：http://sr.gzmigu.cn

Bash ........... 80
来源：http://xa.wgjwhj.cn

Kotlin ......... 15
来源：http://xe.colortex.cn

Swift .......... 15
来源：http://vw.colortex.cn

Lua ............ 10
来源：http://tj.bookmarksfly.cn

Perl ........... 10
来源：http://vp.yuntaijiaju.cn

Scala .......... 10
来源：http://re.bookmarksfly.cn

------------------------------------
来源：http://ne.jctech888.com.cn

合计 ........... 2106 条
来源：http://du.nicolike.cn

按章节统计：
来源：http://bl.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zx.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rn.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aw.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wr.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kk.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://js.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jw.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sh.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qb.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wo.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xb.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xi.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kc.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://su.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://by.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rw.wgjwhj.cn

Q SQL 专题                              90
来源：http://pc.haigaiapp.cn

R Bash 专题                             80
来源：http://cn.nicolike.cn

S C / C++ 专题                          60
来源：http://op.szsharing.cn

T 其他语言补充                          60
来源：http://wi.asd995.cn

U 高频实用片段                         120
来源：http://yn.nicolike.cn

------------------------------------
来源：http://vu.nicolike.cn

合计                                  2106 条
来源：http://qm.9csxet.cn

--------------------------------------------------------------------------------
来源：http://nu.szsharing.cn

使用提醒
来源：http://eh.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://hm.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uf.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yo.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fb.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wp.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kd.9csxet.cn

—— 文件结束 ——
来源：http://jx.colortex.cn

================================================================================
来源：http://bp.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://bq.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://dx.huanxung.cn

================================================================================
来源：http://qa.9csxet.cn

【收录内容】
来源：http://di.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zp.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pt.hnjuh.cn

SQL · Bash · C · C++
来源：http://vb.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wj.szsharing.cn

【使用说明】
来源：http://cu.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nb.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ai.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lz.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yr.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kr.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rh.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ua.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mw.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iu.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cl.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qt.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gs.yuexingan06.cn

【文件统计】
来源：http://pt.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gg.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ta.9csxet.cn

目  录
来源：http://sl.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ae.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ur.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uz.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ff.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mi.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://du.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xm.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://au.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://do.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lm.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fw.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pp.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ty.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hs.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pr.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://io.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://up.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vx.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hu.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tl.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qs.bookmarksfly.cn

================================================================================
来源：http://wt.shtwfgs.cn

A. 基础语法与类型
来源：http://iy.shxzskj.cn

================================================================================
来源：http://am.shxzskj.cn

[A01] Hello World
来源：http://nb.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://wo.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://ad.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://qn.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nn.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://lk.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ew.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://kn.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ie.lnxyls.cn

[A02] 变量声明与赋值
来源：http://rr.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fj.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cm.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sp.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vo.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://cv.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://hh.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://zx.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rp.yuexingan06.cn

[A03] 常量定义
来源：http://jf.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yb.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://mf.szsharing.cn

JS:   const PI = 3.14159;
来源：http://ce.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://vp.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://jr.shxzukj.cn

Go:   const PI = 3.14159
来源：http://qp.newstarts.cn

Ruby: PI = 3.14159
来源：http://bc.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://tq.gzmigu.cn

[A04] 判断变量类型
来源：http://pi.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ay.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pk.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cr.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://vp.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qm.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://su.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yq.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://jr.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://zq.jctech888.com.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vp.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ia.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ku.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tj.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://nd.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://fy.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://xu.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://po.yuexingan06.cn

[A06] 字符串转数字
来源：http://hk.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://xi.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://us.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uh.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iq.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ei.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ni.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rg.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://la.hahajie.cn

[A07] 数字转字符串
来源：http://uv.szxytkj.cn

Py:   str(42)
来源：http://pp.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://we.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://ew.huixinmuqiang.cn

TS:   String(42)
来源：http://fb.bjjhwx.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zu.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://te.gzmigu.cn

Ruby: 42.to_s
来源：http://pr.nicolike.cn

C#:   42.ToString()
来源：http://yj.asd995.cn

[A08] 取整与四舍五入
来源：http://ri.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ir.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://be.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vg.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ym.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://po.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oz.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://it.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yh.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ow.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ea.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sd.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://im.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ba.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tn.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ex.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://an.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kl.colortex.cn

[A10] 生成随机数
来源：http://ir.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://rl.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://uo.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://om.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ec.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://pw.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dl.huixiangedu.cn

Ruby: rand(1..100)
来源：http://gq.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://iv.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://sx.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://af.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vi.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dn.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xd.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://fb.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nm.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zi.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zd.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://mw.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fr.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oa.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://tf.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://hh.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://hw.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yi.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://bj.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://mk.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://et.9csxet.cn

Py:   "第一行\n第二行"
来源：http://eh.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://wp.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://nq.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://ie.panjiajie.cn

Java: "第一行\n第二行"
来源：http://kg.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://rj.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://qp.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://sq.jctech888.com.cn

[A14] 注释写法
来源：http://uc.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tx.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bj.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://iq.jianghongdianzi.cn


<!-- 参考信息 -->