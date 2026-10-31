代发 wailian999

[U81] JS：初始化项目
来源：http://pu.lnxyls.cn

npm init -y;  npm i express
来源：http://iy.521024.cn

[U82] JS：package.json 脚本
来源：http://ga.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tw.521024.cn

[U83] JS：ES Module 导入导出
来源：http://ki.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wi.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://yt.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dh.newstarts.cn

[U85] JS：可选链
来源：http://vw.nszjky.cn

a?.b?.c
来源：http://go.asd995.cn

[U86] JS：空值合并
来源：http://qw.521024.cn

a ?? b
来源：http://qy.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://ok.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://os.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://md.jctech888.com.cn

{ ...a, ...b }
来源：http://xc.huanxung.cn

[U89] JS：数组去重
来源：http://ae.nicolike.cn

[...new Set(arr)]
来源：http://od.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://sl.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://qz.9csxet.cn

[U91] JS：对象键值遍历
来源：http://ui.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://we.szxytkj.cn

[U92] JS：深拷贝
来源：http://qn.bookmarksfly.cn

structuredClone(obj)
来源：http://xd.nicolike.cn

[U93] JS：模板字符串
来源：http://qx.yuexingan06.cn

`共 ${n} 条`
来源：http://tb.9csxet.cn

[U94] JS：箭头函数
来源：http://pd.9csxet.cn

const double = x => x * 2;
来源：http://gj.nszjky.cn

[U95] JS：Promise 包装
来源：http://bk.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://km.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ub.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vd.9csxet.cn

[U97] JS：并发请求
来源：http://zu.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://no.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://iw.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yd.szsharing.cn

[U99] JS：事件监听
来源：http://xo.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://hp.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://gl.chemitech.net.cn

document.querySelector(".item")
来源：http://vv.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://rk.521024.cn

el.classList.toggle("active")
来源：http://cd.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://xv.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xt.9csxet.cn

[U103] JS：定时器
来源：http://jn.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ym.gzmigu.cn

[U104] JS：防抖
来源：http://rv.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.asd995.cn

[U105] JS：节流
来源：http://rd.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rh.gzmigu.cn

[U106] JS：日期格式化
来源：http://za.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://by.bjjhwx.cn

[U107] JS：数字千分位
来源：http://un.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fc.colortex.cn

[U108] JS：随机整数
来源：http://nh.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pi.haigaiapp.cn

[U109] JS：数组分组
来源：http://gc.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://yb.huixiangedu.cn

[U110] JS：数组分块
来源：http://rz.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hf.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://yi.hnjuh.cn

new Map(Object.entries(obj))
来源：http://cs.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://wj.muxihuayi.cn

"7".padStart(3, "0")
来源：http://le.521024.cn

[U113] JS：正则替换全部
来源：http://ji.szsharing.cn

s.replaceAll("a", "b")
来源：http://ui.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://pp.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zh.hnjuh.cn

[U115] JS：生成 UUID
来源：http://hy.asd995.cn

crypto.randomUUID()
来源：http://he.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://ps.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://dr.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://ba.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://rf.szxytkj.cn

[U118] JS：开发服务器
来源：http://nt.hnjuh.cn

npm i -D vite;  npx vite
来源：http://yt.nicolike.cn

[U119] JS：生产构建
来源：http://wj.newstarts.cn

npx vite build
来源：http://uu.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://oy.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://da.haigaiapp.cn

统计汇总
来源：http://ad.colortex.cn

================================================================================
来源：http://ay.9csxet.cn

按语言统计（条）：
来源：http://fd.chemitech.net.cn

Python ......... 252
来源：http://do.colortex.cn

PHP ............ 252
来源：http://bu.wgjwhj.cn

JavaScript ..... 252
来源：http://lh.huixinmuqiang.cn

TypeScript ..... 212
来源：http://dx.nicolike.cn

Java ........... 212
来源：http://ma.szsharing.cn

Go ............. 212
来源：http://vp.huanxung.cn

Ruby ........... 212
来源：http://vi.chemitech.net.cn

C# ............. 212
来源：http://vn.hahajie.cn

C .............. 30
来源：http://jt.asd995.cn

C++ ............ 30
来源：http://va.gzmigu.cn

SQL ............ 90
来源：http://qc.gzmigu.cn

Bash ........... 80
来源：http://hf.shxzukj.cn

Kotlin ......... 15
来源：http://cp.jctech888.com.cn

Swift .......... 15
来源：http://dw.huixiangedu.cn

Lua ............ 10
来源：http://lj.szsharing.cn

Perl ........... 10
来源：http://pp.wgjwhj.cn

Scala .......... 10
来源：http://wd.huixiangedu.cn

------------------------------------
来源：http://wa.chemitech.net.cn

合计 ........... 2106 条
来源：http://sa.521024.cn

按章节统计：
来源：http://yh.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gt.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kv.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ii.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://np.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bm.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lk.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iq.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jq.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gs.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nw.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lu.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fg.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ii.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://am.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ki.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bv.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://ux.yuexingan06.cn

R Bash 专题                             80
来源：http://ez.shxzskj.cn

S C / C++ 专题                          60
来源：http://hr.hnjuh.cn

T 其他语言补充                          60
来源：http://cn.shxzukj.cn

U 高频实用片段                         120
来源：http://lg.yuntaijiaju.cn

------------------------------------
来源：http://xc.yuntaijiaju.cn

合计                                  2106 条
来源：http://iw.521024.cn

--------------------------------------------------------------------------------
来源：http://qo.newstarts.cn

使用提醒
来源：http://zb.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://qn.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ks.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dx.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eh.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oj.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xr.jctech888.com.cn

—— 文件结束 ——
来源：http://df.szsharing.cn

================================================================================
来源：http://pv.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://kh.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://iw.jctech888.com.cn

================================================================================
来源：http://ku.bjjhwx.cn

【收录内容】
来源：http://go.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oy.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sm.nszjky.cn

SQL · Bash · C · C++
来源：http://ak.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vg.huixiangedu.cn

【使用说明】
来源：http://il.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cx.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yi.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bq.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ga.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ya.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xe.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hk.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ql.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ze.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jf.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fd.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wc.nszjky.cn

【文件统计】
来源：http://wc.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oj.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://wl.szsharing.cn

目  录
来源：http://jl.colortex.cn

--------------------------------------------------------------------------------
来源：http://ik.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tu.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ku.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nd.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iz.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tl.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fw.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wh.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ir.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fg.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ng.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pj.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rl.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://co.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vo.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gq.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rs.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wl.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zi.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://td.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zp.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tk.nszjky.cn

================================================================================
来源：http://xo.panjiajie.cn

A. 基础语法与类型
来源：http://lx.colortex.cn

================================================================================
来源：http://gb.hahajie.cn

[A01] Hello World
来源：http://lt.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://gg.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://td.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://rb.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dm.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://ht.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://kj.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://tc.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bg.huanxung.cn

[A02] 变量声明与赋值
来源：http://wp.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yz.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ya.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://js.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qe.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://yl.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://ti.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://zs.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://od.haigaiapp.cn

[A03] 常量定义
来源：http://wg.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yn.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://lg.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://bo.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://bf.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://bt.asd995.cn

Go:   const PI = 3.14159
来源：http://qk.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://rc.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://ws.szxytkj.cn

[A04] 判断变量类型
来源：http://ne.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hf.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cq.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ys.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://pf.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gg.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bs.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yc.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://nn.haigaiapp.cn

[A05] 整数除法与取模
来源：http://lx.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qz.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cb.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oy.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xf.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://qv.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://op.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ig.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://hq.bookmarksfly.cn

[A06] 字符串转数字
来源：http://of.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://wt.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vf.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wb.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cs.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jx.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jw.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ex.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zq.jctech888.com.cn

[A07] 数字转字符串
来源：http://hb.521024.cn

Py:   str(42)
来源：http://vo.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://uf.asd995.cn

JS:   String(42); (42).toString()
来源：http://pp.bookmarksfly.cn

TS:   String(42)
来源：http://ra.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qi.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://uf.9csxet.cn

Ruby: 42.to_s
来源：http://kj.muxihuayi.cn

C#:   42.ToString()
来源：http://lb.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://ll.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ep.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nd.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cv.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xt.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rm.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lq.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gs.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dh.asd995.cn

[A09] 绝对值与最大最小值
来源：http://zq.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dq.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rd.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wp.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fh.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oj.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bv.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://du.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gs.szsharing.cn

[A10] 生成随机数
来源：http://pb.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://qt.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://aw.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ni.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://na.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://nn.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ul.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://rp.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://qj.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://gm.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://qm.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xl.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uy.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ak.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://bg.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wl.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ak.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wp.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://qa.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qm.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ur.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://vt.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://ej.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://lo.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vy.521024.cn

Ruby: "Hello, #{name}!"
来源：http://dq.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://cs.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://le.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://vr.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://in.nszjky.cn

JS:   "第一行\n第二行"
来源：http://zf.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://nl.wgjwhj.cn


<!-- 参考信息 -->