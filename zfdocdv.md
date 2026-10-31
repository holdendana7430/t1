代发 wailian999

[U81] JS：初始化项目
来源：http://fr.panjiajie.cn

npm init -y;  npm i express
来源：http://pf.hahajie.cn

[U82] JS：package.json 脚本
来源：http://ry.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yi.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://vw.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pq.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://zk.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://or.nicolike.cn

[U85] JS：可选链
来源：http://nl.9csxet.cn

a?.b?.c
来源：http://rb.panjiajie.cn

[U86] JS：空值合并
来源：http://fk.jctech888.com.cn

a ?? b
来源：http://ge.shxzskj.cn

[U87] JS：解构默认值
来源：http://km.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://vb.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://su.yuexingan06.cn

{ ...a, ...b }
来源：http://gd.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://zv.huanxung.cn

[...new Set(arr)]
来源：http://xx.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://zr.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://yl.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://sq.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ob.hnjuh.cn

[U92] JS：深拷贝
来源：http://ty.9csxet.cn

structuredClone(obj)
来源：http://za.szsharing.cn

[U93] JS：模板字符串
来源：http://gt.huanxung.cn

`共 ${n} 条`
来源：http://cw.jctech888.com.cn

[U94] JS：箭头函数
来源：http://vd.haigaiapp.cn

const double = x => x * 2;
来源：http://se.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ac.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://vs.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://wg.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ho.lnxyls.cn

[U97] JS：并发请求
来源：http://lj.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wb.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://ah.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zy.huixiangedu.cn

[U99] JS：事件监听
来源：http://ss.hahajie.cn

el.addEventListener("click", e => {})
来源：http://sb.9csxet.cn

[U100] JS：DOM 查询
来源：http://fn.asd995.cn

document.querySelector(".item")
来源：http://zs.hnjuh.cn

[U101] JS：classList 操作
来源：http://wj.panjiajie.cn

el.classList.toggle("active")
来源：http://km.muxihuayi.cn

[U102] JS：本地存储
来源：http://cu.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vs.9csxet.cn

[U103] JS：定时器
来源：http://vn.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bu.chemitech.net.cn

[U104] JS：防抖
来源：http://hi.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.szsharing.cn

[U105] JS：节流
来源：http://ct.yuexingan06.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zk.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://gm.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ro.nicolike.cn

[U107] JS：数字千分位
来源：http://os.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fo.shxzukj.cn

[U108] JS：随机整数
来源：http://cj.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vm.colortex.cn

[U109] JS：数组分组
来源：http://vz.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://al.panjiajie.cn

[U110] JS：数组分块
来源：http://mx.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ir.shxzukj.cn

[U111] JS：对象转 Map
来源：http://sr.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://pj.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://fr.asd995.cn

"7".padStart(3, "0")
来源：http://xh.szsharing.cn

[U113] JS：正则替换全部
来源：http://vi.lnxyls.cn

s.replaceAll("a", "b")
来源：http://pl.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://be.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xj.521024.cn

[U115] JS：生成 UUID
来源：http://kq.huanxung.cn

crypto.randomUUID()
来源：http://hb.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://sx.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://jl.shtwfgs.cn

[U117] JS：单元测试
来源：http://sl.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://mg.hnjuh.cn

[U118] JS：开发服务器
来源：http://ww.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ka.szsharing.cn

[U119] JS：生产构建
来源：http://te.panjiajie.cn

npx vite build
来源：http://gj.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ll.asd995.cn

import.meta.env.VITE_API_URL
来源：http://mz.chemitech.net.cn

================================================================================
来源：http://mv.muxihuayi.cn

统计汇总
来源：http://ov.nicolike.cn

================================================================================
来源：http://ls.521024.cn

按语言统计（条）：
来源：http://lz.gzmigu.cn

Python ......... 252
来源：http://hg.hahajie.cn

PHP ............ 252
来源：http://oz.9csxet.cn

JavaScript ..... 252
来源：http://jg.colortex.cn

TypeScript ..... 212
来源：http://ov.jianghongdianzi.cn

Java ........... 212
来源：http://gy.yuntaijiaju.cn

Go ............. 212
来源：http://lj.521024.cn

Ruby ........... 212
来源：http://mm.bjjhwx.cn

C# ............. 212
来源：http://pa.wgjwhj.cn

C .............. 30
来源：http://jw.haigaiapp.cn

C++ ............ 30
来源：http://yx.yuexingan06.cn

SQL ............ 90
来源：http://en.hahajie.cn

Bash ........... 80
来源：http://lx.jctech888.com.cn

Kotlin ......... 15
来源：http://no.szsharing.cn

Swift .......... 15
来源：http://gp.9csxet.cn

Lua ............ 10
来源：http://nn.muxihuayi.cn

Perl ........... 10
来源：http://ga.yuexingan06.cn

Scala .......... 10
来源：http://hy.521024.cn

------------------------------------
来源：http://tw.hahajie.cn

合计 ........... 2106 条
来源：http://zv.lnxyls.cn

按章节统计：
来源：http://pt.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ki.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mz.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lw.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://np.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fj.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pn.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jk.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uz.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sn.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rw.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fn.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hg.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lj.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rm.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dr.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vo.gzmigu.cn

Q SQL 专题                              90
来源：http://ry.huanxung.cn

R Bash 专题                             80
来源：http://mn.521024.cn

S C / C++ 专题                          60
来源：http://bn.chemitech.net.cn

T 其他语言补充                          60
来源：http://cq.szxytkj.cn

U 高频实用片段                         120
来源：http://yh.shxzukj.cn

------------------------------------
来源：http://hn.521024.cn

合计                                  2106 条
来源：http://ww.colortex.cn

--------------------------------------------------------------------------------
来源：http://nj.yuntaijiaju.cn

使用提醒
来源：http://qo.521024.cn

--------------------------------------------------------------------------------
来源：http://ci.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bs.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bo.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://te.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tb.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nu.jctech888.com.cn

—— 文件结束 ——
来源：http://om.colortex.cn

================================================================================
来源：http://ib.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://um.hahajie.cn

Common Programming Examples Cheat Book
来源：http://ps.bookmarksfly.cn

================================================================================
来源：http://aw.bookmarksfly.cn

【收录内容】
来源：http://zy.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dj.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nn.gzmigu.cn

SQL · Bash · C · C++
来源：http://uy.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ic.huixinmuqiang.cn

【使用说明】
来源：http://nt.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rh.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tl.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qw.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jx.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hu.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hn.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://do.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ty.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zn.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fi.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wj.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eh.asd995.cn

【文件统计】
来源：http://jh.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yg.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://qk.hahajie.cn

目  录
来源：http://vz.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uu.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pq.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gr.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qv.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://di.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uh.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wv.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xz.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gs.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gt.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ae.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eq.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dq.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fz.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tg.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nm.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ls.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://so.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vo.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ks.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aw.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ct.szxytkj.cn

================================================================================
来源：http://kb.hahajie.cn

A. 基础语法与类型
来源：http://cu.bjjhwx.cn

================================================================================
来源：http://eh.gzmigu.cn

[A01] Hello World
来源：http://iw.asd995.cn

Py:   print("Hello, World!")
来源：http://ag.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://ji.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://mm.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tm.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://jw.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://gt.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://yk.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ff.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://uc.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://in.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eq.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://st.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lk.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://yx.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://lj.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://zb.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wo.newstarts.cn

[A03] 常量定义
来源：http://jh.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vv.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://bn.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://dh.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://sj.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://dd.newstarts.cn

Go:   const PI = 3.14159
来源：http://ga.huanxung.cn

Ruby: PI = 3.14159
来源：http://is.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://ro.9csxet.cn

[A04] 判断变量类型
来源：http://oz.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wc.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qg.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://za.521024.cn

TS:   typeof x; x instanceof Date
来源：http://bo.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ge.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kt.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lt.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ww.asd995.cn

[A05] 整数除法与取模
来源：http://gj.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fe.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nq.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vf.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sk.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://hy.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://ql.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://be.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://wh.shtwfgs.cn

[A06] 字符串转数字
来源：http://ub.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://bu.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dc.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xq.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bt.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wp.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jn.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ol.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sp.bookmarksfly.cn

[A07] 数字转字符串
来源：http://sq.shxzukj.cn

Py:   str(42)
来源：http://ey.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://lq.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://ro.szsharing.cn

TS:   String(42)
来源：http://ub.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ku.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://yf.bookmarksfly.cn

Ruby: 42.to_s
来源：http://gb.hahajie.cn

C#:   42.ToString()
来源：http://dd.gzmigu.cn

[A08] 取整与四舍五入
来源：http://hz.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cs.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ko.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yj.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qx.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sa.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lh.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ho.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://el.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ma.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yj.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jr.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hx.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kj.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iu.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ua.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dk.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nm.chemitech.net.cn

[A10] 生成随机数
来源：http://pp.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://lq.nszjky.cn

PHP:  random_int(1, 100);
来源：http://ff.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yb.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hx.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://zi.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lj.szsharing.cn

Ruby: rand(1..100)
来源：http://ew.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://ap.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://um.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://bl.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cx.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ix.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xl.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://xf.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ue.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mr.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fs.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://ve.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://di.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pi.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://oa.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://qh.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://sn.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bc.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://ak.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://fo.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ec.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://un.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://xi.nicolike.cn

JS:   "第一行\n第二行"
来源：http://wk.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://zr.gzmigu.cn


<!-- 参考信息 -->