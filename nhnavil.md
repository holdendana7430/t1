代发 wailian999

[U81] JS：初始化项目
来源：http://cy.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://om.colortex.cn

[U82] JS：package.json 脚本
来源：http://kn.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rb.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://kb.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pr.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://ay.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yv.yuntaijiaju.cn

[U85] JS：可选链
来源：http://ln.szxytkj.cn

a?.b?.c
来源：http://vo.haigaiapp.cn

[U86] JS：空值合并
来源：http://zl.newstarts.cn

a ?? b
来源：http://ob.hnjuh.cn

[U87] JS：解构默认值
来源：http://uf.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://dv.521024.cn

[U88] JS：对象展开合并
来源：http://yk.jianghongdianzi.cn

{ ...a, ...b }
来源：http://zy.muxihuayi.cn

[U89] JS：数组去重
来源：http://xt.huixiangedu.cn

[...new Set(arr)]
来源：http://pk.gzmigu.cn

[U90] JS：数字数组排序
来源：http://uk.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://vp.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://or.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uv.asd995.cn

[U92] JS：深拷贝
来源：http://hu.yuexingan06.cn

structuredClone(obj)
来源：http://ms.521024.cn

[U93] JS：模板字符串
来源：http://rb.jianghongdianzi.cn

`共 ${n} 条`
来源：http://um.szxytkj.cn

[U94] JS：箭头函数
来源：http://gy.jianghongdianzi.cn

const double = x => x * 2;
来源：http://pb.szxytkj.cn

[U95] JS：Promise 包装
来源：http://pw.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://ix.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://bw.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aw.haigaiapp.cn

[U97] JS：并发请求
来源：http://en.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yg.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://he.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bf.szsharing.cn

[U99] JS：事件监听
来源：http://ut.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://wl.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://qk.yuntaijiaju.cn

document.querySelector(".item")
来源：http://dc.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://ed.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://mo.muxihuayi.cn

[U102] JS：本地存储
来源：http://ld.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ik.9csxet.cn

[U103] JS：定时器
来源：http://rt.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rh.asd995.cn

[U104] JS：防抖
来源：http://we.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wg.gzmigu.cn

[U105] JS：节流
来源：http://ka.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bi.muxihuayi.cn

[U106] JS：日期格式化
来源：http://xs.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ap.muxihuayi.cn

[U107] JS：数字千分位
来源：http://yy.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dy.9csxet.cn

[U108] JS：随机整数
来源：http://sc.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tt.newstarts.cn

[U109] JS：数组分组
来源：http://ol.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://sa.szsharing.cn

[U110] JS：数组分块
来源：http://ck.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ed.huanxung.cn

[U111] JS：对象转 Map
来源：http://gj.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ra.jctech888.com.cn

[U112] JS：字符串补位
来源：http://ih.jctech888.com.cn

"7".padStart(3, "0")
来源：http://zw.nszjky.cn

[U113] JS：正则替换全部
来源：http://dv.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://yo.newstarts.cn

[U114] JS：JSON 深比较
来源：http://sx.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hk.asd995.cn

[U115] JS：生成 UUID
来源：http://ah.lnxyls.cn

crypto.randomUUID()
来源：http://op.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://hu.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://dx.bookmarksfly.cn

[U117] JS：单元测试
来源：http://ou.521024.cn

npm i -D vitest;  npx vitest
来源：http://tl.asd995.cn

[U118] JS：开发服务器
来源：http://yz.asd995.cn

npm i -D vite;  npx vite
来源：http://yk.bookmarksfly.cn

[U119] JS：生产构建
来源：http://rl.hnjuh.cn

npx vite build
来源：http://qh.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://of.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://st.huixiangedu.cn

================================================================================
来源：http://lo.hnjuh.cn

统计汇总
来源：http://ww.asd995.cn

================================================================================
来源：http://wz.shxzskj.cn

按语言统计（条）：
来源：http://fs.hahajie.cn

Python ......... 252
来源：http://bc.521024.cn

PHP ............ 252
来源：http://vd.asd995.cn

JavaScript ..... 252
来源：http://dy.wgjwhj.cn

TypeScript ..... 212
来源：http://tx.asd995.cn

Java ........... 212
来源：http://gh.chemitech.net.cn

Go ............. 212
来源：http://bf.bjjhwx.cn

Ruby ........... 212
来源：http://jc.yuexingan06.cn

C# ............. 212
来源：http://yf.yuntaijiaju.cn

C .............. 30
来源：http://dz.jianghongdianzi.cn

C++ ............ 30
来源：http://dp.jctech888.com.cn

SQL ............ 90
来源：http://dx.shxzukj.cn

Bash ........... 80
来源：http://la.yuntaijiaju.cn

Kotlin ......... 15
来源：http://wt.chemitech.net.cn

Swift .......... 15
来源：http://qn.bookmarksfly.cn

Lua ............ 10
来源：http://so.hahajie.cn

Perl ........... 10
来源：http://nr.jianghongdianzi.cn

Scala .......... 10
来源：http://ah.9csxet.cn

------------------------------------
来源：http://ll.colortex.cn

合计 ........... 2106 条
来源：http://fz.huixiangedu.cn

按章节统计：
来源：http://fw.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vk.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mf.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ec.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pu.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fp.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ri.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gl.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ik.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sf.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://we.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://me.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nx.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vg.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uv.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kq.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gy.szxytkj.cn

Q SQL 专题                              90
来源：http://vm.colortex.cn

R Bash 专题                             80
来源：http://rx.shxzskj.cn

S C / C++ 专题                          60
来源：http://ti.asd995.cn

T 其他语言补充                          60
来源：http://or.asd995.cn

U 高频实用片段                         120
来源：http://as.gzmigu.cn

------------------------------------
来源：http://ob.szxytkj.cn

合计                                  2106 条
来源：http://go.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ip.bookmarksfly.cn

使用提醒
来源：http://cm.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://fg.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nz.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eh.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xg.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jr.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cw.shxzukj.cn

—— 文件结束 ——
来源：http://to.panjiajie.cn

================================================================================
来源：http://cs.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://ut.hahajie.cn

Common Programming Examples Cheat Book
来源：http://mx.huixiangedu.cn

================================================================================
来源：http://dd.lnxyls.cn

【收录内容】
来源：http://ln.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://td.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://db.szxytkj.cn

SQL · Bash · C · C++
来源：http://qp.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vc.9csxet.cn

【使用说明】
来源：http://gs.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dl.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pd.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ie.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ls.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ez.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ar.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ed.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qv.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tj.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yz.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ud.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eh.gzmigu.cn

【文件统计】
来源：http://bv.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hn.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://su.wgjwhj.cn

目  录
来源：http://ql.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://qk.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ej.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ps.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jx.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bg.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qz.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ot.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wm.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hd.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gl.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bg.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rl.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hw.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ic.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hv.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lh.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://km.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hm.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oq.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ni.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mx.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bo.hahajie.cn

================================================================================
来源：http://cy.szxytkj.cn

A. 基础语法与类型
来源：http://gm.huanxung.cn

================================================================================
来源：http://bb.gzmigu.cn

[A01] Hello World
来源：http://pe.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ai.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://es.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://ui.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ly.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://pf.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://qz.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://dv.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gn.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://wl.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wv.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ry.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://it.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fc.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://dg.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ot.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://tq.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ul.gzmigu.cn

[A03] 常量定义
来源：http://xq.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uz.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://xz.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ep.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://sk.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://su.colortex.cn

Go:   const PI = 3.14159
来源：http://rj.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://ig.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://df.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://io.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sj.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vv.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sm.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://qn.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mm.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ln.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ri.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://nh.bjjhwx.cn

[A05] 整数除法与取模
来源：http://nv.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vf.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lz.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pa.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cl.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://oi.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://bs.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ju.521024.cn

C#:   7 / 2; 7 % 2
来源：http://we.chemitech.net.cn

[A06] 字符串转数字
来源：http://jy.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://eu.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vh.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yw.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iw.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rq.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://er.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hb.newstarts.cn

[A07] 数字转字符串
来源：http://wk.jianghongdianzi.cn

Py:   str(42)
来源：http://fu.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://bm.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://zn.nszjky.cn

TS:   String(42)
来源：http://ml.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kz.shtwfgs.cn

Go:   strconv.Itoa(42)
来源：http://bw.muxihuayi.cn

Ruby: 42.to_s
来源：http://zy.colortex.cn

C#:   42.ToString()
来源：http://jh.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://ok.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yq.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cf.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zh.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qn.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wv.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hr.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rz.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ib.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://al.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yk.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qx.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kk.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yr.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eu.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qw.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hg.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fb.jianghongdianzi.cn

[A10] 生成随机数
来源：http://sh.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://in.nszjky.cn

PHP:  random_int(1, 100);
来源：http://uw.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bt.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cu.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://ix.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nv.lnxyls.cn

Ruby: rand(1..100)
来源：http://sp.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://kx.9csxet.cn

[A11] 条件表达式（三元）
来源：http://oi.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qw.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fp.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rm.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ig.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://gq.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mc.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jv.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fl.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://cn.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mt.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gv.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ey.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://yo.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://wt.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kj.521024.cn

Ruby: "Hello, #{name}!"
来源：http://qz.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://zv.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ga.nicolike.cn

Py:   "第一行\n第二行"
来源：http://dd.asd995.cn

PHP:  "第一行\n第二行"
来源：http://xp.asd995.cn

JS:   "第一行\n第二行"
来源：http://yt.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://bd.szsharing.cn


<!-- 参考信息 -->