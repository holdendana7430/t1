代发 wailian999

[U79] PHP：静态分析
来源：http://vd.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://aw.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://uy.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xj.lnxyls.cn

[U81] JS：初始化项目
来源：http://pq.huixiangedu.cn

npm init -y;  npm i express
来源：http://hu.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://sd.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://td.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://vf.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fu.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://og.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://av.newstarts.cn

[U85] JS：可选链
来源：http://jo.haigaiapp.cn

a?.b?.c
来源：http://rd.szxytkj.cn

[U86] JS：空值合并
来源：http://cj.chemitech.net.cn

a ?? b
来源：http://hy.bjjhwx.cn

[U87] JS：解构默认值
来源：http://gf.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://tq.huanxung.cn

[U88] JS：对象展开合并
来源：http://uy.huixinmuqiang.cn

{ ...a, ...b }
来源：http://rg.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://wd.nszjky.cn

[...new Set(arr)]
来源：http://zs.szxytkj.cn

[U90] JS：数字数组排序
来源：http://jl.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://tt.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://oz.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cq.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://gx.yuntaijiaju.cn

structuredClone(obj)
来源：http://fb.yuexingan06.cn

[U93] JS：模板字符串
来源：http://ve.huixiangedu.cn

`共 ${n} 条`
来源：http://ob.chemitech.net.cn

[U94] JS：箭头函数
来源：http://nb.jctech888.com.cn

const double = x => x * 2;
来源：http://sb.asd995.cn

[U95] JS：Promise 包装
来源：http://rx.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://tl.szsharing.cn

[U96] JS：async/await 与异常
来源：http://xr.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://le.bookmarksfly.cn

[U97] JS：并发请求
来源：http://rp.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.521024.cn

[U98] JS：fetch 带 JSON
来源：http://zx.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rs.huixiangedu.cn

[U99] JS：事件监听
来源：http://mx.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://ft.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://kk.nszjky.cn

document.querySelector(".item")
来源：http://id.shxzukj.cn

[U101] JS：classList 操作
来源：http://kw.nszjky.cn

el.classList.toggle("active")
来源：http://th.asd995.cn

[U102] JS：本地存储
来源：http://ml.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qj.shxzukj.cn

[U103] JS：定时器
来源：http://yz.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ty.9csxet.cn

[U104] JS：防抖
来源：http://rk.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aw.nszjky.cn

[U105] JS：节流
来源：http://gb.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://in.shxzskj.cn

[U106] JS：日期格式化
来源：http://nf.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wv.hnjuh.cn

[U107] JS：数字千分位
来源：http://qq.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dc.521024.cn

[U108] JS：随机整数
来源：http://zq.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zo.shxzukj.cn

[U109] JS：数组分组
来源：http://ep.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://br.huixiangedu.cn

[U110] JS：数组分块
来源：http://lx.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wn.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://zf.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://zn.nicolike.cn

[U112] JS：字符串补位
来源：http://gb.shtwfgs.cn

"7".padStart(3, "0")
来源：http://ae.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ww.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://nc.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://il.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gy.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://tm.hnjuh.cn

crypto.randomUUID()
来源：http://ud.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://vc.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://ow.9csxet.cn

[U117] JS：单元测试
来源：http://ub.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ku.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://ca.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://yp.hnjuh.cn

[U119] JS：生产构建
来源：http://df.nszjky.cn

npx vite build
来源：http://st.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://qi.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://wi.lnxyls.cn

================================================================================
来源：http://be.9csxet.cn

统计汇总
来源：http://cf.nicolike.cn

================================================================================
来源：http://dv.muxihuayi.cn

按语言统计（条）：
来源：http://hw.bjjhwx.cn

Python ......... 252
来源：http://po.muxihuayi.cn

PHP ............ 252
来源：http://km.jctech888.com.cn

JavaScript ..... 252
来源：http://la.bookmarksfly.cn

TypeScript ..... 212
来源：http://kg.shxzskj.cn

Java ........... 212
来源：http://of.shtwfgs.cn

Go ............. 212
来源：http://as.jctech888.com.cn

Ruby ........... 212
来源：http://wp.asd995.cn

C# ............. 212
来源：http://ai.szsharing.cn

C .............. 30
来源：http://yh.hahajie.cn

C++ ............ 30
来源：http://nz.szsharing.cn

SQL ............ 90
来源：http://iv.nszjky.cn

Bash ........... 80
来源：http://pw.shxzukj.cn

Kotlin ......... 15
来源：http://ov.nszjky.cn

Swift .......... 15
来源：http://co.nicolike.cn

Lua ............ 10
来源：http://kf.jianghongdianzi.cn

Perl ........... 10
来源：http://xw.haigaiapp.cn

Scala .......... 10
来源：http://yi.9csxet.cn

------------------------------------
来源：http://td.lnxyls.cn

合计 ........... 2106 条
来源：http://zx.9csxet.cn

按章节统计：
来源：http://bo.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mn.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tx.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://no.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lr.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oh.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gr.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zr.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://me.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ie.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vn.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zk.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lc.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ps.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kx.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://un.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hm.muxihuayi.cn

Q SQL 专题                              90
来源：http://sg.hahajie.cn

R Bash 专题                             80
来源：http://jq.shtwfgs.cn

S C / C++ 专题                          60
来源：http://np.lnxyls.cn

T 其他语言补充                          60
来源：http://zy.wgjwhj.cn

U 高频实用片段                         120
来源：http://eg.shxzukj.cn

------------------------------------
来源：http://xp.nszjky.cn

合计                                  2106 条
来源：http://mu.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ro.panjiajie.cn

使用提醒
来源：http://be.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://um.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wr.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yw.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lb.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gs.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vw.gzmigu.cn

—— 文件结束 ——
来源：http://mm.bookmarksfly.cn

================================================================================
来源：http://kd.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://gd.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://dy.9csxet.cn

================================================================================
来源：http://ql.huixinmuqiang.cn

【收录内容】
来源：http://kb.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qy.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hx.wgjwhj.cn

SQL · Bash · C · C++
来源：http://jm.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dj.huixinmuqiang.cn

【使用说明】
来源：http://tg.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jr.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pi.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wp.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cu.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ft.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hn.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tr.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://em.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lk.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gi.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nc.szsharing.cn

【文件统计】
来源：http://nc.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nq.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://qi.shtwfgs.cn

目  录
来源：http://pa.huanxung.cn

--------------------------------------------------------------------------------
来源：http://lw.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aq.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://py.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hu.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wx.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mr.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fc.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jk.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://we.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pq.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gy.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cp.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://os.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aa.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zi.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kz.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vb.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kf.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://en.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pw.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fu.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qd.panjiajie.cn

================================================================================
来源：http://mh.panjiajie.cn

A. 基础语法与类型
来源：http://qe.shxzskj.cn

================================================================================
来源：http://lc.yuexingan06.cn

[A01] Hello World
来源：http://gv.szsharing.cn

Py:   print("Hello, World!")
来源：http://dg.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://by.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ll.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pg.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://bo.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://tn.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://at.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://es.szsharing.cn

[A02] 变量声明与赋值
来源：http://sm.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://et.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sz.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eb.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cc.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://mh.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://dj.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://rd.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rd.szsharing.cn

[A03] 常量定义
来源：http://bv.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gf.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://ob.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://ux.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://ck.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://th.szxytkj.cn

Go:   const PI = 3.14159
来源：http://ma.panjiajie.cn

Ruby: PI = 3.14159
来源：http://jz.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://yd.chemitech.net.cn

[A04] 判断变量类型
来源：http://xp.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ow.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ac.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pa.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://gq.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gh.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://js.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ou.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://ox.521024.cn

[A05] 整数除法与取模
来源：http://zk.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uy.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://im.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bk.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qp.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://ua.521024.cn

Go:   7 / 2; 7 % 2
来源：http://nn.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ma.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://ti.jctech888.com.cn

[A06] 字符串转数字
来源：http://rv.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://dp.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fk.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wh.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://my.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fs.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xm.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uq.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wn.nicolike.cn

[A07] 数字转字符串
来源：http://fr.nicolike.cn

Py:   str(42)
来源：http://qz.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://mh.nszjky.cn

JS:   String(42); (42).toString()
来源：http://rv.szxytkj.cn

TS:   String(42)
来源：http://bn.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ii.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://qy.521024.cn

Ruby: 42.to_s
来源：http://ku.huanxung.cn

C#:   42.ToString()
来源：http://zq.szxytkj.cn

[A08] 取整与四舍五入
来源：http://us.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ad.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hi.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hv.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mu.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xu.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pf.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cv.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nw.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://nf.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bq.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wp.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jv.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hi.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rx.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://de.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fb.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lu.bjjhwx.cn

[A10] 生成随机数
来源：http://od.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ci.nszjky.cn

PHP:  random_int(1, 100);
来源：http://uf.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bb.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rc.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://pp.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cz.huanxung.cn

Ruby: rand(1..100)
来源：http://ei.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://se.nszjky.cn

[A11] 条件表达式（三元）
来源：http://ty.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://yx.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xr.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ou.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bi.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ks.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oz.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jb.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ii.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://gl.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aw.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hr.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://zv.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://ex.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://xn.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sf.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://hl.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://yk.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://au.colortex.cn


<!-- 参考信息 -->