代发 wailian999

[U75] PHP：依赖注入
来源：http://sh.szsharing.cn

composer require psr/container
来源：http://nm.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://gv.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wl.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://yy.hnjuh.cn

composer require twig/twig
来源：http://js.muxihuayi.cn

[U78] PHP：单元测试
来源：http://nw.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://ph.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://dj.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://fb.colortex.cn

[U80] PHP：代码规范修复
来源：http://vg.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wi.shtwfgs.cn

[U81] JS：初始化项目
来源：http://fb.shxzukj.cn

npm init -y;  npm i express
来源：http://up.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://bh.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kj.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ez.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jb.colortex.cn

[U84] JS：CommonJS 写法
来源：http://cw.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jq.panjiajie.cn

[U85] JS：可选链
来源：http://gf.nszjky.cn

a?.b?.c
来源：http://gb.shxzskj.cn

[U86] JS：空值合并
来源：http://cu.bjjhwx.cn

a ?? b
来源：http://sc.chemitech.net.cn

[U87] JS：解构默认值
来源：http://kn.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ek.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://yz.wgjwhj.cn

{ ...a, ...b }
来源：http://xl.bjjhwx.cn

[U89] JS：数组去重
来源：http://wv.yuntaijiaju.cn

[...new Set(arr)]
来源：http://la.nszjky.cn

[U90] JS：数字数组排序
来源：http://gh.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://kz.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://yp.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ur.szxytkj.cn

[U92] JS：深拷贝
来源：http://kp.newstarts.cn

structuredClone(obj)
来源：http://bb.chemitech.net.cn

[U93] JS：模板字符串
来源：http://nj.hnjuh.cn

`共 ${n} 条`
来源：http://hl.jctech888.com.cn

[U94] JS：箭头函数
来源：http://nn.muxihuayi.cn

const double = x => x * 2;
来源：http://wu.521024.cn

[U95] JS：Promise 包装
来源：http://yn.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://es.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://rf.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eo.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://tp.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gi.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://xe.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tu.szsharing.cn

[U99] JS：事件监听
来源：http://pt.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://ew.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://sf.yuexingan06.cn

document.querySelector(".item")
来源：http://bk.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://go.haigaiapp.cn

el.classList.toggle("active")
来源：http://on.shxzukj.cn

[U102] JS：本地存储
来源：http://vy.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nh.bjjhwx.cn

[U103] JS：定时器
来源：http://oz.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vw.huanxung.cn

[U104] JS：防抖
来源：http://oc.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ht.9csxet.cn

[U105] JS：节流
来源：http://jz.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cj.9csxet.cn

[U106] JS：日期格式化
来源：http://zg.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yg.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://xg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ak.panjiajie.cn

[U108] JS：随机整数
来源：http://yr.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tl.9csxet.cn

[U109] JS：数组分组
来源：http://vh.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://sq.panjiajie.cn

[U110] JS：数组分块
来源：http://wf.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cj.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://xj.nszjky.cn

new Map(Object.entries(obj))
来源：http://fb.panjiajie.cn

[U112] JS：字符串补位
来源：http://es.chemitech.net.cn

"7".padStart(3, "0")
来源：http://pr.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://ve.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://tu.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://zg.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tb.hahajie.cn

[U115] JS：生成 UUID
来源：http://bz.bjjhwx.cn

crypto.randomUUID()
来源：http://wf.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://sv.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://yh.shxzskj.cn

[U117] JS：单元测试
来源：http://bs.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://xq.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://za.nicolike.cn

npm i -D vite;  npx vite
来源：http://zm.huanxung.cn

[U119] JS：生产构建
来源：http://uo.huanxung.cn

npx vite build
来源：http://it.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://oa.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://mr.muxihuayi.cn

================================================================================
来源：http://ej.nicolike.cn

统计汇总
来源：http://qt.hahajie.cn

================================================================================
来源：http://nf.hnjuh.cn

按语言统计（条）：
来源：http://xi.haigaiapp.cn

Python ......... 252
来源：http://bk.9csxet.cn

PHP ............ 252
来源：http://oh.9csxet.cn

JavaScript ..... 252
来源：http://we.huanxung.cn

TypeScript ..... 212
来源：http://sp.shtwfgs.cn

Java ........... 212
来源：http://yu.gzmigu.cn

Go ............. 212
来源：http://fp.bookmarksfly.cn

Ruby ........... 212
来源：http://yz.wgjwhj.cn

C# ............. 212
来源：http://nh.shxzskj.cn

C .............. 30
来源：http://gq.colortex.cn

C++ ............ 30
来源：http://od.huixinmuqiang.cn

SQL ............ 90
来源：http://nw.nicolike.cn

Bash ........... 80
来源：http://uc.huixiangedu.cn

Kotlin ......... 15
来源：http://ce.yuexingan06.cn

Swift .......... 15
来源：http://qe.bookmarksfly.cn

Lua ............ 10
来源：http://lk.chemitech.net.cn

Perl ........... 10
来源：http://fz.huixinmuqiang.cn

Scala .......... 10
来源：http://un.shtwfgs.cn

------------------------------------
来源：http://gw.huanxung.cn

合计 ........... 2106 条
来源：http://vh.bookmarksfly.cn

按章节统计：
来源：http://ej.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wc.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ru.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sp.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yf.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fz.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cb.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mw.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://na.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tc.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ps.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ra.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jt.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ux.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yf.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://az.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rl.gzmigu.cn

Q SQL 专题                              90
来源：http://uo.muxihuayi.cn

R Bash 专题                             80
来源：http://kk.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ba.jctech888.com.cn

T 其他语言补充                          60
来源：http://oc.bjjhwx.cn

U 高频实用片段                         120
来源：http://gy.chemitech.net.cn

------------------------------------
来源：http://cr.panjiajie.cn

合计                                  2106 条
来源：http://td.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ku.jctech888.com.cn

使用提醒
来源：http://qf.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://rw.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qs.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cn.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bi.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vy.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lc.hahajie.cn

—— 文件结束 ——
来源：http://xe.lnxyls.cn

================================================================================
来源：http://kg.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://sz.huanxung.cn

Common Programming Examples Cheat Book
来源：http://sb.szxytkj.cn

================================================================================
来源：http://ze.nszjky.cn

【收录内容】
来源：http://oz.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yt.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vn.newstarts.cn

SQL · Bash · C · C++
来源：http://ab.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ik.colortex.cn

【使用说明】
来源：http://lx.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://su.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ol.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gv.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gq.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cf.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ab.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://be.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xe.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yh.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sl.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ay.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mi.9csxet.cn

【文件统计】
来源：http://qu.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ud.newstarts.cn

--------------------------------------------------------------------------------
来源：http://lf.asd995.cn

目  录
来源：http://lb.huanxung.cn

--------------------------------------------------------------------------------
来源：http://jd.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pt.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://by.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://go.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hq.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wt.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gn.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://be.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ud.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ph.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://po.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yo.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sy.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tv.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rj.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tm.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wj.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cz.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bv.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eb.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jw.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xm.newstarts.cn

================================================================================
来源：http://jp.bjjhwx.cn

A. 基础语法与类型
来源：http://jr.521024.cn

================================================================================
来源：http://nv.szsharing.cn

[A01] Hello World
来源：http://qq.szsharing.cn

Py:   print("Hello, World!")
来源：http://qx.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://oc.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://ym.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tg.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://zx.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://fm.521024.cn

Ruby: puts "Hello, World!"
来源：http://fm.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ln.nszjky.cn

[A02] 变量声明与赋值
来源：http://zh.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qf.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://is.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kl.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cu.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://vs.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://sk.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://lo.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ay.shxzskj.cn

[A03] 常量定义
来源：http://mf.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hk.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://dx.colortex.cn

JS:   const PI = 3.14159;
来源：http://ql.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://mk.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://cr.szxytkj.cn

Go:   const PI = 3.14159
来源：http://hy.colortex.cn

Ruby: PI = 3.14159
来源：http://nt.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://gm.hnjuh.cn

[A04] 判断变量类型
来源：http://aa.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gr.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pj.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ac.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://tm.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nn.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nw.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ze.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://cr.huanxung.cn

[A05] 整数除法与取模
来源：http://fm.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qs.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vt.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wa.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uh.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ux.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://js.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ea.521024.cn

C#:   7 / 2; 7 % 2
来源：http://pu.muxihuayi.cn

[A06] 字符串转数字
来源：http://cn.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://iu.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ls.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://io.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://te.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zb.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ss.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ut.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zi.newstarts.cn

[A07] 数字转字符串
来源：http://zp.szxytkj.cn

Py:   str(42)
来源：http://pd.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://ju.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://sd.shxzskj.cn

TS:   String(42)
来源：http://kk.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yr.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://xp.jctech888.com.cn

Ruby: 42.to_s
来源：http://ch.9csxet.cn

C#:   42.ToString()
来源：http://mk.gzmigu.cn

[A08] 取整与四舍五入
来源：http://dw.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jr.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://po.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ie.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ar.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oe.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qv.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qb.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xy.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://bh.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ij.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ac.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zb.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://im.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nx.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kp.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ev.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qy.521024.cn

[A10] 生成随机数
来源：http://xt.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://ne.colortex.cn

PHP:  random_int(1, 100);
来源：http://ih.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yx.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ei.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://yw.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ew.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ij.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://ji.9csxet.cn

[A11] 条件表达式（三元）
来源：http://ol.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://cn.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://he.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yf.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lj.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://js.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ao.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cn.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yq.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://pi.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fc.muxihuayi.cn


<!-- 参考信息 -->