代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://sj.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://ql.nszjky.cn

[U74] PHP：读取环境变量
来源：http://li.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ur.huanxung.cn

[U75] PHP：依赖注入
来源：http://fn.521024.cn

composer require psr/container
来源：http://wq.nicolike.cn

[U76] PHP：简单路由
来源：http://qi.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uo.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://zv.jctech888.com.cn

composer require twig/twig
来源：http://wv.9csxet.cn

[U78] PHP：单元测试
来源：http://ht.521024.cn

composer require --dev phpunit/phpunit
来源：http://mi.jctech888.com.cn

[U79] PHP：静态分析
来源：http://xh.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://xv.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://ni.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sm.chemitech.net.cn

[U81] JS：初始化项目
来源：http://gr.bjjhwx.cn

npm init -y;  npm i express
来源：http://wt.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://tq.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sv.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://yl.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pt.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://pu.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ig.shxzskj.cn

[U85] JS：可选链
来源：http://vp.jctech888.com.cn

a?.b?.c
来源：http://dk.panjiajie.cn

[U86] JS：空值合并
来源：http://vn.huixiangedu.cn

a ?? b
来源：http://ok.hahajie.cn

[U87] JS：解构默认值
来源：http://yy.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://gh.nicolike.cn

[U88] JS：对象展开合并
来源：http://ey.521024.cn

{ ...a, ...b }
来源：http://kf.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://qe.9csxet.cn

[...new Set(arr)]
来源：http://ln.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://bz.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://sd.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://bh.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lg.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://qm.haigaiapp.cn

structuredClone(obj)
来源：http://db.chemitech.net.cn

[U93] JS：模板字符串
来源：http://op.panjiajie.cn

`共 ${n} 条`
来源：http://vq.lnxyls.cn

[U94] JS：箭头函数
来源：http://hh.nicolike.cn

const double = x => x * 2;
来源：http://sc.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://yh.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://zb.521024.cn

[U96] JS：async/await 与异常
来源：http://vn.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ir.bjjhwx.cn

[U97] JS：并发请求
来源：http://uh.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://na.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://fc.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ay.huixiangedu.cn

[U99] JS：事件监听
来源：http://rj.nszjky.cn

el.addEventListener("click", e => {})
来源：http://ci.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://ih.hnjuh.cn

document.querySelector(".item")
来源：http://ag.hnjuh.cn

[U101] JS：classList 操作
来源：http://cn.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://cg.chemitech.net.cn

[U102] JS：本地存储
来源：http://rz.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zw.haigaiapp.cn

[U103] JS：定时器
来源：http://cq.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://od.gzmigu.cn

[U104] JS：防抖
来源：http://ve.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ow.lnxyls.cn

[U105] JS：节流
来源：http://uc.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yk.chemitech.net.cn

[U106] JS：日期格式化
来源：http://iz.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ds.gzmigu.cn

[U107] JS：数字千分位
来源：http://hf.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cv.newstarts.cn

[U108] JS：随机整数
来源：http://hl.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://es.newstarts.cn

[U109] JS：数组分组
来源：http://ea.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://yi.521024.cn

[U110] JS：数组分块
来源：http://cw.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fv.huanxung.cn

[U111] JS：对象转 Map
来源：http://aw.gzmigu.cn

new Map(Object.entries(obj))
来源：http://oe.muxihuayi.cn

[U112] JS：字符串补位
来源：http://bq.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ng.colortex.cn

[U113] JS：正则替换全部
来源：http://py.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://cg.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://mj.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ex.colortex.cn

[U115] JS：生成 UUID
来源：http://ms.asd995.cn

crypto.randomUUID()
来源：http://ea.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://il.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://nf.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://tw.colortex.cn

npm i -D vitest;  npx vitest
来源：http://oi.nszjky.cn

[U118] JS：开发服务器
来源：http://vo.shxzskj.cn

npm i -D vite;  npx vite
来源：http://gr.asd995.cn

[U119] JS：生产构建
来源：http://cz.hnjuh.cn

npx vite build
来源：http://su.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://yn.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://ne.9csxet.cn

================================================================================
来源：http://zr.yuexingan06.cn

统计汇总
来源：http://ta.shtwfgs.cn

================================================================================
来源：http://bb.hahajie.cn

按语言统计（条）：
来源：http://fk.huanxung.cn

Python ......... 252
来源：http://st.jctech888.com.cn

PHP ............ 252
来源：http://rp.lnxyls.cn

JavaScript ..... 252
来源：http://iz.9csxet.cn

TypeScript ..... 212
来源：http://ob.panjiajie.cn

Java ........... 212
来源：http://ux.wgjwhj.cn

Go ............. 212
来源：http://ne.shxzukj.cn

Ruby ........... 212
来源：http://uu.huixiangedu.cn

C# ............. 212
来源：http://yg.wgjwhj.cn

C .............. 30
来源：http://nj.521024.cn

C++ ............ 30
来源：http://bw.muxihuayi.cn

SQL ............ 90
来源：http://li.yuexingan06.cn

Bash ........... 80
来源：http://jl.newstarts.cn

Kotlin ......... 15
来源：http://lx.colortex.cn

Swift .......... 15
来源：http://dg.shxzukj.cn

Lua ............ 10
来源：http://fm.huixiangedu.cn

Perl ........... 10
来源：http://zf.newstarts.cn

Scala .......... 10
来源：http://xk.szxytkj.cn

------------------------------------
来源：http://yu.newstarts.cn

合计 ........... 2106 条
来源：http://ch.bjjhwx.cn

按章节统计：
来源：http://od.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ws.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yb.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nu.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ig.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fs.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lz.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hi.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pk.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jj.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wu.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ir.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rv.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cf.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jx.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eq.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uz.szxytkj.cn

Q SQL 专题                              90
来源：http://zj.bjjhwx.cn

R Bash 专题                             80
来源：http://de.huanxung.cn

S C / C++ 专题                          60
来源：http://ie.shtwfgs.cn

T 其他语言补充                          60
来源：http://eh.chemitech.net.cn

U 高频实用片段                         120
来源：http://uw.jctech888.com.cn

------------------------------------
来源：http://oi.hahajie.cn

合计                                  2106 条
来源：http://rn.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://qw.huanxung.cn

使用提醒
来源：http://de.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://fc.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bq.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yy.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://th.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pm.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cx.gzmigu.cn

—— 文件结束 ——
来源：http://qn.gzmigu.cn

================================================================================
来源：http://kw.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://xp.huanxung.cn

Common Programming Examples Cheat Book
来源：http://ik.szsharing.cn

================================================================================
来源：http://xz.chemitech.net.cn

【收录内容】
来源：http://vf.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ir.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://am.haigaiapp.cn

SQL · Bash · C · C++
来源：http://ez.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vq.newstarts.cn

【使用说明】
来源：http://xo.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://od.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ai.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ew.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rx.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qc.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uf.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pb.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://of.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ud.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lc.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://un.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ro.bookmarksfly.cn

【文件统计】
来源：http://he.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ff.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ir.hnjuh.cn

目  录
来源：http://ya.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ln.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jo.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qu.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zo.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sv.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vt.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fy.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lm.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oo.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jb.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mm.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nr.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ek.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gq.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ow.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ub.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wm.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ci.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fk.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yu.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qa.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gf.huanxung.cn

================================================================================
来源：http://ak.jianghongdianzi.cn

A. 基础语法与类型
来源：http://gt.huixiangedu.cn

================================================================================
来源：http://mp.lnxyls.cn

[A01] Hello World
来源：http://jr.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://jj.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://hi.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://dk.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://og.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://av.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://wr.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://vm.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rn.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://ek.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nr.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ey.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ok.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iv.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://rk.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://jw.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://mm.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mb.jctech888.com.cn

[A03] 常量定义
来源：http://iy.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mg.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://ui.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://sv.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://hb.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://tq.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://id.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://ce.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://dj.szxytkj.cn

[A04] 判断变量类型
来源：http://is.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pu.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cp.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zn.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://iu.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://em.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xn.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hl.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://sk.jctech888.com.cn

[A05] 整数除法与取模
来源：http://ih.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oc.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ed.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ft.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oq.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://jr.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://es.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://iz.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://rw.szxytkj.cn

[A06] 字符串转数字
来源：http://ip.colortex.cn

Py:   int("42"); float("3.14")
来源：http://fz.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pa.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fx.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wp.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dx.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ls.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kk.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dr.colortex.cn

[A07] 数字转字符串
来源：http://us.bjjhwx.cn

Py:   str(42)
来源：http://uz.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://hi.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://ys.shtwfgs.cn

TS:   String(42)
来源：http://qr.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://li.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://ox.muxihuayi.cn

Ruby: 42.to_s
来源：http://ty.bjjhwx.cn

C#:   42.ToString()
来源：http://rz.shxzukj.cn

[A08] 取整与四舍五入
来源：http://ub.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fu.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ty.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nt.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://la.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pp.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rd.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ih.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gb.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://bq.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bh.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lo.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rf.521024.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hu.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oo.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zw.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pn.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ou.szxytkj.cn

[A10] 生成随机数
来源：http://oj.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://ja.newstarts.cn

PHP:  random_int(1, 100);
来源：http://cz.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jw.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xt.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://sk.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ez.9csxet.cn

Ruby: rand(1..100)
来源：http://mz.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://cb.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://xh.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://gh.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sz.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tx.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fx.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://yi.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zh.9csxet.cn


<!-- 参考信息 -->