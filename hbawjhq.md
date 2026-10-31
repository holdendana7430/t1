代发 wailian999

[U79] PHP：静态分析
来源：http://ks.521024.cn

composer require --dev phpstan/phpstan
来源：http://mm.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://ll.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ak.nicolike.cn

[U81] JS：初始化项目
来源：http://gs.bookmarksfly.cn

npm init -y;  npm i express
来源：http://ok.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://up.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://on.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://fo.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oo.asd995.cn

[U84] JS：CommonJS 写法
来源：http://eu.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bz.haigaiapp.cn

[U85] JS：可选链
来源：http://ht.wgjwhj.cn

a?.b?.c
来源：http://qy.newstarts.cn

[U86] JS：空值合并
来源：http://ue.szsharing.cn

a ?? b
来源：http://zr.hnjuh.cn

[U87] JS：解构默认值
来源：http://xb.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://bg.panjiajie.cn

[U88] JS：对象展开合并
来源：http://jm.newstarts.cn

{ ...a, ...b }
来源：http://ov.muxihuayi.cn

[U89] JS：数组去重
来源：http://un.chemitech.net.cn

[...new Set(arr)]
来源：http://qs.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://jg.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ff.colortex.cn

[U91] JS：对象键值遍历
来源：http://ms.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pp.521024.cn

[U92] JS：深拷贝
来源：http://gi.newstarts.cn

structuredClone(obj)
来源：http://rt.szsharing.cn

[U93] JS：模板字符串
来源：http://hu.nszjky.cn

`共 ${n} 条`
来源：http://ge.colortex.cn

[U94] JS：箭头函数
来源：http://nk.newstarts.cn

const double = x => x * 2;
来源：http://dg.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://lz.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://zw.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://yk.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://el.huanxung.cn

[U97] JS：并发请求
来源：http://tf.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tm.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://sy.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fp.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://bi.asd995.cn

el.addEventListener("click", e => {})
来源：http://fz.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://xi.asd995.cn

document.querySelector(".item")
来源：http://ec.huanxung.cn

[U101] JS：classList 操作
来源：http://vc.gzmigu.cn

el.classList.toggle("active")
来源：http://eo.asd995.cn

[U102] JS：本地存储
来源：http://yk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bx.colortex.cn

[U103] JS：定时器
来源：http://xj.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://on.gzmigu.cn

[U104] JS：防抖
来源：http://gp.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.muxihuayi.cn

[U105] JS：节流
来源：http://rn.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://el.hnjuh.cn

[U106] JS：日期格式化
来源：http://jo.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ta.hnjuh.cn

[U107] JS：数字千分位
来源：http://dy.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ls.hahajie.cn

[U108] JS：随机整数
来源：http://pj.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cu.panjiajie.cn

[U109] JS：数组分组
来源：http://cj.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://mb.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://cx.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dz.hnjuh.cn

[U111] JS：对象转 Map
来源：http://rg.shxzukj.cn

new Map(Object.entries(obj))
来源：http://oh.chemitech.net.cn

[U112] JS：字符串补位
来源：http://lz.chemitech.net.cn

"7".padStart(3, "0")
来源：http://vk.szxytkj.cn

[U113] JS：正则替换全部
来源：http://bf.colortex.cn

s.replaceAll("a", "b")
来源：http://mz.huanxung.cn

[U114] JS：JSON 深比较
来源：http://ug.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vm.huanxung.cn

[U115] JS：生成 UUID
来源：http://pz.521024.cn

crypto.randomUUID()
来源：http://nt.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://hj.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://sm.521024.cn

[U117] JS：单元测试
来源：http://xr.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://we.hahajie.cn

[U118] JS：开发服务器
来源：http://fo.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://ro.nszjky.cn

[U119] JS：生产构建
来源：http://ul.szxytkj.cn

npx vite build
来源：http://ri.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://bb.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://gx.shtwfgs.cn

================================================================================
来源：http://cf.huixiangedu.cn

统计汇总
来源：http://un.hnjuh.cn

================================================================================
来源：http://he.panjiajie.cn

按语言统计（条）：
来源：http://xa.wgjwhj.cn

Python ......... 252
来源：http://rv.muxihuayi.cn

PHP ............ 252
来源：http://au.chemitech.net.cn

JavaScript ..... 252
来源：http://jb.jctech888.com.cn

TypeScript ..... 212
来源：http://yz.huixinmuqiang.cn

Java ........... 212
来源：http://zw.colortex.cn

Go ............. 212
来源：http://hs.szxytkj.cn

Ruby ........... 212
来源：http://da.9csxet.cn

C# ............. 212
来源：http://ju.nicolike.cn

C .............. 30
来源：http://hf.nicolike.cn

C++ ............ 30
来源：http://ty.newstarts.cn

SQL ............ 90
来源：http://fs.jctech888.com.cn

Bash ........... 80
来源：http://kb.chemitech.net.cn

Kotlin ......... 15
来源：http://it.lnxyls.cn

Swift .......... 15
来源：http://sk.panjiajie.cn

Lua ............ 10
来源：http://xo.shxzskj.cn

Perl ........... 10
来源：http://yg.nszjky.cn

Scala .......... 10
来源：http://zp.gzmigu.cn

------------------------------------
来源：http://jp.jctech888.com.cn

合计 ........... 2106 条
来源：http://bs.szsharing.cn

按章节统计：
来源：http://dn.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bq.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hh.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://so.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mr.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cd.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tc.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jw.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tm.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iv.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yo.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fn.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jd.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oq.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nc.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eh.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dm.hahajie.cn

Q SQL 专题                              90
来源：http://to.jctech888.com.cn

R Bash 专题                             80
来源：http://jg.haigaiapp.cn

S C / C++ 专题                          60
来源：http://af.szxytkj.cn

T 其他语言补充                          60
来源：http://jm.bjjhwx.cn

U 高频实用片段                         120
来源：http://bd.lnxyls.cn

------------------------------------
来源：http://jz.haigaiapp.cn

合计                                  2106 条
来源：http://az.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://hr.nicolike.cn

使用提醒
来源：http://kn.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://mz.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nr.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zm.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qm.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jr.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xv.szxytkj.cn

—— 文件结束 ——
来源：http://ab.newstarts.cn

================================================================================
来源：http://gh.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://yf.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://qv.lnxyls.cn

================================================================================
来源：http://mt.hnjuh.cn

【收录内容】
来源：http://xd.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vg.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kk.gzmigu.cn

SQL · Bash · C · C++
来源：http://uc.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vb.wgjwhj.cn

【使用说明】
来源：http://hv.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mp.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://op.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bm.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://us.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ml.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lc.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nk.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ds.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jk.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lr.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ia.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cw.jctech888.com.cn

【文件统计】
来源：http://kt.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pt.colortex.cn

--------------------------------------------------------------------------------
来源：http://tt.yuexingan06.cn

目  录
来源：http://wc.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://vm.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rg.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jv.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uo.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hh.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nv.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vi.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hk.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ct.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nc.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zi.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pi.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kl.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fg.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jq.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://si.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://to.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lk.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wo.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ab.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nv.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jz.colortex.cn

================================================================================
来源：http://yd.szxytkj.cn

A. 基础语法与类型
来源：http://ra.huixinmuqiang.cn

================================================================================
来源：http://lp.szxytkj.cn

[A01] Hello World
来源：http://jj.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://pu.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://ul.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://zh.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dz.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://tp.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://ax.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://dx.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lu.huanxung.cn

[A02] 变量声明与赋值
来源：http://nn.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://if.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yf.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uc.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nm.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://yp.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://ik.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://sg.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://je.haigaiapp.cn

[A03] 常量定义
来源：http://zk.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tn.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://xh.colortex.cn

JS:   const PI = 3.14159;
来源：http://cu.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://sx.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://cq.colortex.cn

Go:   const PI = 3.14159
来源：http://qr.newstarts.cn

Ruby: PI = 3.14159
来源：http://aw.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://xn.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://ia.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lh.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://le.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://un.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://ns.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rp.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rb.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zh.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://wo.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://nj.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ug.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://be.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gj.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rg.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://lb.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://xr.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://bh.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://kz.asd995.cn

[A06] 字符串转数字
来源：http://mz.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://om.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bd.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kf.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zp.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kp.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ef.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://by.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ye.wgjwhj.cn

[A07] 数字转字符串
来源：http://tj.nszjky.cn

Py:   str(42)
来源：http://vw.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://qd.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://vj.shxzukj.cn

TS:   String(42)
来源：http://mk.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dw.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://sn.chemitech.net.cn

Ruby: 42.to_s
来源：http://dt.huixinmuqiang.cn

C#:   42.ToString()
来源：http://zs.szxytkj.cn

[A08] 取整与四舍五入
来源：http://ww.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://we.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pi.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ck.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jz.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yt.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sj.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nz.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fy.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://vp.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://or.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xu.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hm.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lv.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://se.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ec.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bj.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ud.nszjky.cn

[A10] 生成随机数
来源：http://ru.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://dn.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://lp.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wt.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://ea.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sv.newstarts.cn

Ruby: rand(1..100)
来源：http://qp.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://zt.hahajie.cn

[A11] 条件表达式（三元）
来源：http://fw.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://ai.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yi.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cr.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://va.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://rg.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zb.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qr.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zd.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://ox.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aw.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jo.colortex.cn

JS:   `Hello, ${name}!`
来源：http://qx.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://tp.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://jw.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hv.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://cw.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://lm.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://to.9csxet.cn


<!-- 参考信息 -->