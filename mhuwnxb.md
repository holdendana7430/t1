代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://fj.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kw.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://sp.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xk.jianghongdianzi.cn

[U85] JS：可选链
来源：http://pc.colortex.cn

a?.b?.c
来源：http://kp.newstarts.cn

[U86] JS：空值合并
来源：http://xa.shtwfgs.cn

a ?? b
来源：http://dl.wgjwhj.cn

[U87] JS：解构默认值
来源：http://vx.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://vk.asd995.cn

[U88] JS：对象展开合并
来源：http://zp.newstarts.cn

{ ...a, ...b }
来源：http://ue.muxihuayi.cn

[U89] JS：数组去重
来源：http://um.muxihuayi.cn

[...new Set(arr)]
来源：http://bw.521024.cn

[U90] JS：数字数组排序
来源：http://nm.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://cx.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://kj.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nd.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ta.chemitech.net.cn

structuredClone(obj)
来源：http://ci.gzmigu.cn

[U93] JS：模板字符串
来源：http://uc.bjjhwx.cn

`共 ${n} 条`
来源：http://tc.521024.cn

[U94] JS：箭头函数
来源：http://cm.shxzskj.cn

const double = x => x * 2;
来源：http://tr.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ft.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://se.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://vf.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lt.shtwfgs.cn

[U97] JS：并发请求
来源：http://bd.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dh.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://if.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rb.huanxung.cn

[U99] JS：事件监听
来源：http://ox.asd995.cn

el.addEventListener("click", e => {})
来源：http://nu.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://qd.colortex.cn

document.querySelector(".item")
来源：http://pe.shxzskj.cn

[U101] JS：classList 操作
来源：http://qy.newstarts.cn

el.classList.toggle("active")
来源：http://ip.bjjhwx.cn

[U102] JS：本地存储
来源：http://rt.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zc.haigaiapp.cn

[U103] JS：定时器
来源：http://wp.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zp.521024.cn

[U104] JS：防抖
来源：http://wh.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.hahajie.cn

[U105] JS：节流
来源：http://dj.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mx.shxzukj.cn

[U106] JS：日期格式化
来源：http://og.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rq.shtwfgs.cn

[U107] JS：数字千分位
来源：http://gz.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xu.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://oo.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qw.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://zq.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://rw.lnxyls.cn

[U110] JS：数组分块
来源：http://rm.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ms.asd995.cn

[U111] JS：对象转 Map
来源：http://ud.hahajie.cn

new Map(Object.entries(obj))
来源：http://yd.panjiajie.cn

[U112] JS：字符串补位
来源：http://lr.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ge.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://fu.szxytkj.cn

s.replaceAll("a", "b")
来源：http://rx.nicolike.cn

[U114] JS：JSON 深比较
来源：http://pw.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ed.shxzukj.cn

[U115] JS：生成 UUID
来源：http://re.jctech888.com.cn

crypto.randomUUID()
来源：http://ew.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://rr.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ms.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ls.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://uj.hahajie.cn

[U118] JS：开发服务器
来源：http://dp.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://vc.szsharing.cn

[U119] JS：生产构建
来源：http://ju.bjjhwx.cn

npx vite build
来源：http://gh.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://zu.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://gq.szxytkj.cn

统计汇总
来源：http://wy.shxzskj.cn

================================================================================
来源：http://zv.shxzukj.cn

按语言统计（条）：
来源：http://wz.haigaiapp.cn

Python ......... 252
来源：http://ha.szsharing.cn

PHP ............ 252
来源：http://dp.gzmigu.cn

JavaScript ..... 252
来源：http://bw.yuexingan06.cn

TypeScript ..... 212
来源：http://vb.chemitech.net.cn

Java ........... 212
来源：http://fr.lnxyls.cn

Go ............. 212
来源：http://rk.szxytkj.cn

Ruby ........... 212
来源：http://vn.panjiajie.cn

C# ............. 212
来源：http://ar.asd995.cn

C .............. 30
来源：http://im.panjiajie.cn

C++ ............ 30
来源：http://jd.521024.cn

SQL ............ 90
来源：http://hc.hahajie.cn

Bash ........... 80
来源：http://gi.hnjuh.cn

Kotlin ......... 15
来源：http://tn.shtwfgs.cn

Swift .......... 15
来源：http://mt.huixinmuqiang.cn

Lua ............ 10
来源：http://va.hahajie.cn

Perl ........... 10
来源：http://ga.bookmarksfly.cn

Scala .......... 10
来源：http://ur.yuntaijiaju.cn

------------------------------------
来源：http://at.szsharing.cn

合计 ........... 2106 条
来源：http://yp.panjiajie.cn

按章节统计：
来源：http://hg.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lf.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pq.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cu.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ay.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rl.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wj.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cq.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uk.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wk.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xv.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ch.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rz.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wd.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yw.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bl.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ds.hahajie.cn

Q SQL 专题                              90
来源：http://lb.yuexingan06.cn

R Bash 专题                             80
来源：http://dl.bjjhwx.cn

S C / C++ 专题                          60
来源：http://dw.shxzskj.cn

T 其他语言补充                          60
来源：http://ln.huixiangedu.cn

U 高频实用片段                         120
来源：http://dg.521024.cn

------------------------------------
来源：http://tv.szsharing.cn

合计                                  2106 条
来源：http://sz.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://yk.shxzukj.cn

使用提醒
来源：http://kn.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://cg.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fa.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ku.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hd.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://no.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qf.huixiangedu.cn

—— 文件结束 ——
来源：http://fy.jctech888.com.cn

================================================================================
来源：http://sf.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://bh.huanxung.cn

Common Programming Examples Cheat Book
来源：http://hp.gzmigu.cn

================================================================================
来源：http://qh.hahajie.cn

【收录内容】
来源：http://xl.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cz.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://td.nicolike.cn

SQL · Bash · C · C++
来源：http://hf.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zp.chemitech.net.cn

【使用说明】
来源：http://vm.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fl.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ef.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cq.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xl.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ak.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ht.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tu.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hb.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cz.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qe.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ze.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fp.hnjuh.cn

【文件统计】
来源：http://jl.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ie.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://mv.bookmarksfly.cn

目  录
来源：http://sw.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://qu.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ck.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://na.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rr.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fi.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://za.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ry.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pv.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jb.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vd.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qu.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zx.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ho.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sq.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kv.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pu.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aj.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sa.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hd.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tw.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://il.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uo.521024.cn

================================================================================
来源：http://mq.huixinmuqiang.cn

A. 基础语法与类型
来源：http://sg.521024.cn

================================================================================
来源：http://ru.bookmarksfly.cn

[A01] Hello World
来源：http://rd.szxytkj.cn

Py:   print("Hello, World!")
来源：http://zl.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://ga.colortex.cn

JS:   console.log("Hello, World!");
来源：http://jf.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nl.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://sz.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://lq.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://bb.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nw.gzmigu.cn

[A02] 变量声明与赋值
来源：http://zq.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yc.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nb.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ix.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oi.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://lf.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://ex.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://sl.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://co.bookmarksfly.cn

[A03] 常量定义
来源：http://vh.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wf.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://bd.nszjky.cn

JS:   const PI = 3.14159;
来源：http://dg.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://la.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://qv.szsharing.cn

Go:   const PI = 3.14159
来源：http://py.521024.cn

Ruby: PI = 3.14159
来源：http://ca.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://gh.huixiangedu.cn

[A04] 判断变量类型
来源：http://sh.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hj.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://id.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ne.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://gc.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pe.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eg.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ft.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://ta.nicolike.cn

[A05] 整数除法与取模
来源：http://dm.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uy.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://li.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gn.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jv.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://tg.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://mm.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ql.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://fe.huanxung.cn

[A06] 字符串转数字
来源：http://kb.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://bw.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://me.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bp.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cf.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rl.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qc.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://th.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cc.szxytkj.cn

[A07] 数字转字符串
来源：http://yq.newstarts.cn

Py:   str(42)
来源：http://xh.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://xo.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://pa.shxzukj.cn

TS:   String(42)
来源：http://cp.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vw.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://sr.newstarts.cn

Ruby: 42.to_s
来源：http://zu.jctech888.com.cn

C#:   42.ToString()
来源：http://gs.asd995.cn

[A08] 取整与四舍五入
来源：http://dh.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://st.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fx.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sn.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dm.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ny.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rs.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bq.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://so.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://rf.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lo.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://em.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xc.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://au.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uh.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qh.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qt.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wo.asd995.cn

[A10] 生成随机数
来源：http://dk.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://ho.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://pr.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bg.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qy.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://rh.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jv.panjiajie.cn

Ruby: rand(1..100)
来源：http://jj.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://ao.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ei.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://za.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xz.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kq.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vg.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://fo.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pv.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ws.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nn.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://go.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pw.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kc.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://nn.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://dg.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://bx.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://si.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://lg.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://gn.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ka.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://wr.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://qf.nicolike.cn

JS:   "第一行\n第二行"
来源：http://ah.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://yz.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ls.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://hy.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://yv.hahajie.cn

C#:   "第一行\n第二行"
来源：http://su.gzmigu.cn


<!-- 参考信息 -->