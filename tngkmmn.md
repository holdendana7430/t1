代发 wailian999

[U79] PHP：静态分析
来源：http://mc.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://ny.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://hx.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ga.jctech888.com.cn

[U81] JS：初始化项目
来源：http://pg.newstarts.cn

npm init -y;  npm i express
来源：http://rs.nicolike.cn

[U82] JS：package.json 脚本
来源：http://pr.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gr.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://yq.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jw.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://wx.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vn.colortex.cn

[U85] JS：可选链
来源：http://tp.panjiajie.cn

a?.b?.c
来源：http://ax.muxihuayi.cn

[U86] JS：空值合并
来源：http://kk.newstarts.cn

a ?? b
来源：http://du.asd995.cn

[U87] JS：解构默认值
来源：http://pc.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://jg.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://cu.wgjwhj.cn

{ ...a, ...b }
来源：http://pr.huanxung.cn

[U89] JS：数组去重
来源：http://vv.jctech888.com.cn

[...new Set(arr)]
来源：http://rx.szxytkj.cn

[U90] JS：数字数组排序
来源：http://sh.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://zn.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://co.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tp.521024.cn

[U92] JS：深拷贝
来源：http://kr.hahajie.cn

structuredClone(obj)
来源：http://sv.asd995.cn

[U93] JS：模板字符串
来源：http://lr.huixinmuqiang.cn

`共 ${n} 条`
来源：http://tk.huixiangedu.cn

[U94] JS：箭头函数
来源：http://bv.wgjwhj.cn

const double = x => x * 2;
来源：http://gp.hnjuh.cn

[U95] JS：Promise 包装
来源：http://tc.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://uk.asd995.cn

[U96] JS：async/await 与异常
来源：http://zz.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tt.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://gp.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wj.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://gq.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yd.haigaiapp.cn

[U99] JS：事件监听
来源：http://bm.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://jo.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://wk.newstarts.cn

document.querySelector(".item")
来源：http://ra.wgjwhj.cn

[U101] JS：classList 操作
来源：http://zm.gzmigu.cn

el.classList.toggle("active")
来源：http://es.colortex.cn

[U102] JS：本地存储
来源：http://fx.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://to.szxytkj.cn

[U103] JS：定时器
来源：http://ep.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wx.jctech888.com.cn

[U104] JS：防抖
来源：http://zp.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.huixiangedu.cn

[U105] JS：节流
来源：http://mn.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wi.gzmigu.cn

[U106] JS：日期格式化
来源：http://yd.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sy.gzmigu.cn

[U107] JS：数字千分位
来源：http://ua.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ar.asd995.cn

[U108] JS：随机整数
来源：http://ky.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wn.muxihuayi.cn

[U109] JS：数组分组
来源：http://sa.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://dp.haigaiapp.cn

[U110] JS：数组分块
来源：http://qf.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://st.szsharing.cn

[U111] JS：对象转 Map
来源：http://yn.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://wr.shxzukj.cn

[U112] JS：字符串补位
来源：http://ay.shtwfgs.cn

"7".padStart(3, "0")
来源：http://el.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://jb.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://rg.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://ox.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://el.nszjky.cn

[U115] JS：生成 UUID
来源：http://lw.haigaiapp.cn

crypto.randomUUID()
来源：http://no.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://fd.shxzskj.cn

[U117] JS：单元测试
来源：http://nw.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://uw.shxzukj.cn

[U118] JS：开发服务器
来源：http://ts.szxytkj.cn

npm i -D vite;  npx vite
来源：http://aw.haigaiapp.cn

[U119] JS：生产构建
来源：http://mu.jctech888.com.cn

npx vite build
来源：http://nq.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://zv.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://rd.yuntaijiaju.cn

================================================================================
来源：http://ow.9csxet.cn

统计汇总
来源：http://gb.jianghongdianzi.cn

================================================================================
来源：http://cd.huixiangedu.cn

按语言统计（条）：
来源：http://un.chemitech.net.cn

Python ......... 252
来源：http://tu.wgjwhj.cn

PHP ............ 252
来源：http://xq.haigaiapp.cn

JavaScript ..... 252
来源：http://gz.colortex.cn

TypeScript ..... 212
来源：http://gx.gzmigu.cn

Java ........... 212
来源：http://va.nicolike.cn

Go ............. 212
来源：http://li.9csxet.cn

Ruby ........... 212
来源：http://al.wgjwhj.cn

C# ............. 212
来源：http://eu.yuntaijiaju.cn

C .............. 30
来源：http://jk.panjiajie.cn

C++ ............ 30
来源：http://at.hnjuh.cn

SQL ............ 90
来源：http://gh.yuexingan06.cn

Bash ........... 80
来源：http://hj.wgjwhj.cn

Kotlin ......... 15
来源：http://ov.szsharing.cn

Swift .......... 15
来源：http://je.hnjuh.cn

Lua ............ 10
来源：http://vt.panjiajie.cn

Perl ........... 10
来源：http://hq.521024.cn

Scala .......... 10
来源：http://mb.hnjuh.cn

------------------------------------
来源：http://kn.huanxung.cn

合计 ........... 2106 条
来源：http://fx.huixinmuqiang.cn

按章节统计：
来源：http://ys.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yl.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tr.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yo.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rp.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bp.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uo.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yr.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://am.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ql.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wu.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://di.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rt.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rm.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mt.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bt.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bg.yuexingan06.cn

Q SQL 专题                              90
来源：http://wd.yuntaijiaju.cn

R Bash 专题                             80
来源：http://fn.muxihuayi.cn

S C / C++ 专题                          60
来源：http://mg.newstarts.cn

T 其他语言补充                          60
来源：http://uc.colortex.cn

U 高频实用片段                         120
来源：http://zu.hnjuh.cn

------------------------------------
来源：http://xb.9csxet.cn

合计                                  2106 条
来源：http://ut.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://jk.hahajie.cn

使用提醒
来源：http://ki.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://kn.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://am.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vm.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nr.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hb.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kb.haigaiapp.cn

—— 文件结束 ——
来源：http://rb.muxihuayi.cn

================================================================================
来源：http://ay.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://mf.nszjky.cn

Common Programming Examples Cheat Book
来源：http://ml.shxzskj.cn

================================================================================
来源：http://tr.jianghongdianzi.cn

【收录内容】
来源：http://bs.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ld.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xf.bjjhwx.cn

SQL · Bash · C · C++
来源：http://pa.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tc.lnxyls.cn

【使用说明】
来源：http://go.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zi.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ck.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gp.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://td.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ii.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rc.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gb.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qv.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qo.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ja.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ja.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jb.huanxung.cn

【文件统计】
来源：http://rf.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bn.asd995.cn

--------------------------------------------------------------------------------
来源：http://kp.shxzukj.cn

目  录
来源：http://dx.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ex.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pk.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mp.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ed.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://en.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kk.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ve.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uy.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ra.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://li.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kw.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://op.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ob.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aw.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wn.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rq.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gu.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ni.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://im.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cf.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vb.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tk.521024.cn

================================================================================
来源：http://cp.hahajie.cn

A. 基础语法与类型
来源：http://fv.shxzskj.cn

================================================================================
来源：http://ni.muxihuayi.cn

[A01] Hello World
来源：http://wy.521024.cn

Py:   print("Hello, World!")
来源：http://vi.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://ag.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://yc.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fx.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://vn.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://sh.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://ts.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mi.szxytkj.cn

[A02] 变量声明与赋值
来源：http://up.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fp.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fz.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qc.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zc.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://sm.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://ii.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://wi.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fz.newstarts.cn

[A03] 常量定义
来源：http://bz.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kt.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://te.nicolike.cn

JS:   const PI = 3.14159;
来源：http://cm.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://jf.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://ht.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://wc.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://rf.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://ix.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://rf.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fs.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vg.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://th.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://en.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hf.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uk.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kq.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://kr.muxihuayi.cn

[A05] 整数除法与取模
来源：http://xd.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tm.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ol.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ra.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qc.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://pm.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://cg.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://ks.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://ex.chemitech.net.cn

[A06] 字符串转数字
来源：http://zn.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://to.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://di.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ew.huixiangedu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gg.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qr.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qp.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ep.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ph.yuexingan06.cn

[A07] 数字转字符串
来源：http://fz.hahajie.cn

Py:   str(42)
来源：http://co.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://gc.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://yg.jianghongdianzi.cn

TS:   String(42)
来源：http://so.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ss.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://lp.colortex.cn

Ruby: 42.to_s
来源：http://hb.lnxyls.cn

C#:   42.ToString()
来源：http://fj.nszjky.cn

[A08] 取整与四舍五入
来源：http://pn.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kd.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ck.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ot.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wk.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nq.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rt.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zc.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ue.521024.cn

[A09] 绝对值与最大最小值
来源：http://vl.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://us.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gg.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yv.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lp.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gr.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iq.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fu.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ak.asd995.cn

[A10] 生成随机数
来源：http://uo.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://ut.szsharing.cn

PHP:  random_int(1, 100);
来源：http://oc.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bs.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mb.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://nq.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fh.nszjky.cn

Ruby: rand(1..100)
来源：http://oi.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://bt.newstarts.cn

[A11] 条件表达式（三元）
来源：http://gl.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://pm.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jw.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wh.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tf.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://qi.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://un.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ne.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nv.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://yo.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ly.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ob.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://iv.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://wi.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://zz.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hu.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://wt.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://wv.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yi.shxzukj.cn


<!-- 参考信息 -->