代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://wu.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cy.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://aj.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ps.hahajie.cn

[U85] JS：可选链
来源：http://kr.panjiajie.cn

a?.b?.c
来源：http://ac.szxytkj.cn

[U86] JS：空值合并
来源：http://ma.lnxyls.cn

a ?? b
来源：http://no.hahajie.cn

[U87] JS：解构默认值
来源：http://th.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://wv.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://zb.nicolike.cn

{ ...a, ...b }
来源：http://ny.wgjwhj.cn

[U89] JS：数组去重
来源：http://kx.szxytkj.cn

[...new Set(arr)]
来源：http://xp.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://vc.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://gb.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ew.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sm.bjjhwx.cn

[U92] JS：深拷贝
来源：http://ou.huanxung.cn

structuredClone(obj)
来源：http://fh.chemitech.net.cn

[U93] JS：模板字符串
来源：http://ob.jctech888.com.cn

`共 ${n} 条`
来源：http://qp.gzmigu.cn

[U94] JS：箭头函数
来源：http://gp.521024.cn

const double = x => x * 2;
来源：http://qs.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://ld.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://be.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://bh.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ud.szsharing.cn

[U97] JS：并发请求
来源：http://yz.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ov.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://rl.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yq.shtwfgs.cn

[U99] JS：事件监听
来源：http://op.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://hn.huanxung.cn

[U100] JS：DOM 查询
来源：http://ye.panjiajie.cn

document.querySelector(".item")
来源：http://ms.szxytkj.cn

[U101] JS：classList 操作
来源：http://ls.panjiajie.cn

el.classList.toggle("active")
来源：http://sa.szxytkj.cn

[U102] JS：本地存储
来源：http://ib.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ps.colortex.cn

[U103] JS：定时器
来源：http://vu.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rq.hnjuh.cn

[U104] JS：防抖
来源：http://go.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uf.nszjky.cn

[U105] JS：节流
来源：http://yd.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rm.chemitech.net.cn

[U106] JS：日期格式化
来源：http://zu.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mv.szsharing.cn

[U107] JS：数字千分位
来源：http://da.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pt.colortex.cn

[U108] JS：随机整数
来源：http://zs.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kj.9csxet.cn

[U109] JS：数组分组
来源：http://cx.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://of.nicolike.cn

[U110] JS：数组分块
来源：http://tv.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ky.szxytkj.cn

[U111] JS：对象转 Map
来源：http://hp.shxzukj.cn

new Map(Object.entries(obj))
来源：http://xw.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://hv.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ex.huanxung.cn

[U113] JS：正则替换全部
来源：http://cz.huanxung.cn

s.replaceAll("a", "b")
来源：http://yf.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://ma.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bb.nszjky.cn

[U115] JS：生成 UUID
来源：http://jq.yuexingan06.cn

crypto.randomUUID()
来源：http://kp.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://vh.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://fp.nicolike.cn

[U117] JS：单元测试
来源：http://rw.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://iw.521024.cn

[U118] JS：开发服务器
来源：http://ce.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://lm.huanxung.cn

[U119] JS：生产构建
来源：http://uz.nszjky.cn

npx vite build
来源：http://ql.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://vc.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://dn.huanxung.cn

================================================================================
来源：http://bz.9csxet.cn

统计汇总
来源：http://cq.szxytkj.cn

================================================================================
来源：http://yg.huixiangedu.cn

按语言统计（条）：
来源：http://yk.bjjhwx.cn

Python ......... 252
来源：http://qi.wgjwhj.cn

PHP ............ 252
来源：http://bk.jianghongdianzi.cn

JavaScript ..... 252
来源：http://iw.gzmigu.cn

TypeScript ..... 212
来源：http://mi.yuntaijiaju.cn

Java ........... 212
来源：http://px.nszjky.cn

Go ............. 212
来源：http://rh.yuntaijiaju.cn

Ruby ........... 212
来源：http://mb.hnjuh.cn

C# ............. 212
来源：http://xy.521024.cn

C .............. 30
来源：http://ep.colortex.cn

C++ ............ 30
来源：http://fj.nszjky.cn

SQL ............ 90
来源：http://qo.nszjky.cn

Bash ........... 80
来源：http://do.huixiangedu.cn

Kotlin ......... 15
来源：http://qu.szxytkj.cn

Swift .......... 15
来源：http://hq.shtwfgs.cn

Lua ............ 10
来源：http://gl.yuexingan06.cn

Perl ........... 10
来源：http://qy.9csxet.cn

Scala .......... 10
来源：http://zf.asd995.cn

------------------------------------
来源：http://fg.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://vo.521024.cn

按章节统计：
来源：http://mz.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gt.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uy.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cm.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://of.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vf.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nl.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pe.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tk.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zb.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vz.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eg.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vw.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ta.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://np.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ww.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xz.yuexingan06.cn

Q SQL 专题                              90
来源：http://na.nszjky.cn

R Bash 专题                             80
来源：http://df.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://su.9csxet.cn

T 其他语言补充                          60
来源：http://oi.colortex.cn

U 高频实用片段                         120
来源：http://md.huanxung.cn

------------------------------------
来源：http://qz.wgjwhj.cn

合计                                  2106 条
来源：http://ag.nszjky.cn

--------------------------------------------------------------------------------
来源：http://hv.panjiajie.cn

使用提醒
来源：http://em.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://zm.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gb.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zk.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qi.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tx.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://go.huixiangedu.cn

—— 文件结束 ——
来源：http://lf.chemitech.net.cn

================================================================================
来源：http://bu.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://pq.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://jr.nicolike.cn

================================================================================
来源：http://fz.hahajie.cn

【收录内容】
来源：http://vb.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rc.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://us.huanxung.cn

SQL · Bash · C · C++
来源：http://om.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vd.jctech888.com.cn

【使用说明】
来源：http://si.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bk.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ak.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ti.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ao.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fc.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pg.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://aq.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mu.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vp.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ug.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://as.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xd.panjiajie.cn

【文件统计】
来源：http://ws.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dt.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://zl.szsharing.cn

目  录
来源：http://ta.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://tj.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://os.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://up.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kv.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bj.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gp.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sr.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kw.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zl.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jf.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uc.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gz.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gh.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vz.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rj.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ui.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dc.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jf.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fn.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zx.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mq.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dw.colortex.cn

================================================================================
来源：http://aq.jianghongdianzi.cn

A. 基础语法与类型
来源：http://qf.jctech888.com.cn

================================================================================
来源：http://zh.muxihuayi.cn

[A01] Hello World
来源：http://xu.9csxet.cn

Py:   print("Hello, World!")
来源：http://gr.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://pu.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://ud.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gl.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://xm.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://cs.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://su.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://co.gzmigu.cn

[A02] 变量声明与赋值
来源：http://zy.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bt.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lv.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wc.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mq.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://yz.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://bp.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://ie.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dk.szsharing.cn

[A03] 常量定义
来源：http://lo.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xn.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://wg.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ou.521024.cn

TS:   const PI: number = 3.14159;
来源：http://pn.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ni.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://co.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://pm.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://yg.9csxet.cn

[A04] 判断变量类型
来源：http://bn.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rx.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://to.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cv.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://ge.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tm.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qa.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://em.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://mf.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://yf.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wa.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hg.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://he.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yk.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://vo.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://qj.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ef.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://qg.muxihuayi.cn

[A06] 字符串转数字
来源：http://qk.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://og.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qz.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tw.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fa.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://md.wgjwhj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gc.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tn.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mx.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://pc.chemitech.net.cn

Py:   str(42)
来源：http://rg.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://yx.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://dr.521024.cn

TS:   String(42)
来源：http://gw.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mp.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://km.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://ts.jctech888.com.cn

C#:   42.ToString()
来源：http://ey.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ta.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://os.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gr.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mz.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://as.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ul.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cz.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bk.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vb.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://yp.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fl.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tc.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vl.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ae.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qd.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ly.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ed.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bx.nszjky.cn

[A10] 生成随机数
来源：http://cs.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://mc.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://ou.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vm.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ir.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://go.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pv.hahajie.cn

Ruby: rand(1..100)
来源：http://hf.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://kc.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://lg.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://nb.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ho.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nj.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lh.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://hv.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://my.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ph.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ea.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://da.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://os.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qy.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://we.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://qn.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ks.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://av.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://tu.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://qo.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qk.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://bq.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://oj.9csxet.cn

JS:   "第一行\n第二行"
来源：http://kz.colortex.cn

TS:   "第一行\n第二行"
来源：http://hw.nicolike.cn

Java: "第一行\n第二行"
来源：http://fn.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://bl.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://vs.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://cj.shxzskj.cn


<!-- 参考信息 -->