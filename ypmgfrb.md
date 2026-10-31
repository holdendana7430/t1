代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://yf.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://sq.521024.cn

[U74] PHP：读取环境变量
来源：http://uo.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://qv.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://ti.wgjwhj.cn

composer require psr/container
来源：http://ne.jctech888.com.cn

[U76] PHP：简单路由
来源：http://qg.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rz.shxzukj.cn

[U77] PHP：模板渲染
来源：http://xx.hahajie.cn

composer require twig/twig
来源：http://aa.9csxet.cn

[U78] PHP：单元测试
来源：http://nr.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://do.haigaiapp.cn

[U79] PHP：静态分析
来源：http://jh.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://cw.nicolike.cn

[U80] PHP：代码规范修复
来源：http://pd.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jo.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://ki.lnxyls.cn

npm init -y;  npm i express
来源：http://sw.asd995.cn

[U82] JS：package.json 脚本
来源：http://dw.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tm.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://vb.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qg.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://oz.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pz.shxzukj.cn

[U85] JS：可选链
来源：http://wx.9csxet.cn

a?.b?.c
来源：http://si.hahajie.cn

[U86] JS：空值合并
来源：http://kz.gzmigu.cn

a ?? b
来源：http://ae.chemitech.net.cn

[U87] JS：解构默认值
来源：http://kt.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://zu.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://ad.shxzukj.cn

{ ...a, ...b }
来源：http://qz.gzmigu.cn

[U89] JS：数组去重
来源：http://ct.lnxyls.cn

[...new Set(arr)]
来源：http://oq.shxzukj.cn

[U90] JS：数字数组排序
来源：http://mq.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://xg.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://bf.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://st.huixiangedu.cn

[U92] JS：深拷贝
来源：http://ad.asd995.cn

structuredClone(obj)
来源：http://hl.haigaiapp.cn

[U93] JS：模板字符串
来源：http://ij.bookmarksfly.cn

`共 ${n} 条`
来源：http://ml.chemitech.net.cn

[U94] JS：箭头函数
来源：http://dh.hnjuh.cn

const double = x => x * 2;
来源：http://mj.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ft.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://zb.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://zj.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tb.bjjhwx.cn

[U97] JS：并发请求
来源：http://kj.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://du.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://mk.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://an.haigaiapp.cn

[U99] JS：事件监听
来源：http://jf.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://ct.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://ub.asd995.cn

document.querySelector(".item")
来源：http://ug.lnxyls.cn

[U101] JS：classList 操作
来源：http://ow.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://is.nicolike.cn

[U102] JS：本地存储
来源：http://us.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ct.jianghongdianzi.cn

[U103] JS：定时器
来源：http://wv.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hh.huanxung.cn

[U104] JS：防抖
来源：http://lv.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ji.hahajie.cn

[U105] JS：节流
来源：http://oz.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oy.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://kg.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nj.newstarts.cn

[U107] JS：数字千分位
来源：http://xz.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jd.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://wj.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nz.nszjky.cn

[U109] JS：数组分组
来源：http://io.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://lp.hahajie.cn

[U110] JS：数组分块
来源：http://gq.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ca.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ej.panjiajie.cn

new Map(Object.entries(obj))
来源：http://qt.haigaiapp.cn

[U112] JS：字符串补位
来源：http://gg.chemitech.net.cn

"7".padStart(3, "0")
来源：http://pg.hnjuh.cn

[U113] JS：正则替换全部
来源：http://pk.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://fv.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://af.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fo.nicolike.cn

[U115] JS：生成 UUID
来源：http://bo.huanxung.cn

crypto.randomUUID()
来源：http://eb.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://xe.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://zo.hnjuh.cn

[U117] JS：单元测试
来源：http://od.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ge.huixiangedu.cn

[U118] JS：开发服务器
来源：http://xj.szxytkj.cn

npm i -D vite;  npx vite
来源：http://bd.lnxyls.cn

[U119] JS：生产构建
来源：http://co.shxzukj.cn

npx vite build
来源：http://zh.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://kb.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://hf.szsharing.cn

================================================================================
来源：http://qb.jctech888.com.cn

统计汇总
来源：http://up.yuntaijiaju.cn

================================================================================
来源：http://fi.lnxyls.cn

按语言统计（条）：
来源：http://qu.lnxyls.cn

Python ......... 252
来源：http://it.shxzskj.cn

PHP ............ 252
来源：http://yz.huanxung.cn

JavaScript ..... 252
来源：http://ig.haigaiapp.cn

TypeScript ..... 212
来源：http://uv.panjiajie.cn

Java ........... 212
来源：http://zj.huanxung.cn

Go ............. 212
来源：http://nc.nicolike.cn

Ruby ........... 212
来源：http://ym.colortex.cn

C# ............. 212
来源：http://ip.shxzukj.cn

C .............. 30
来源：http://dl.shxzukj.cn

C++ ............ 30
来源：http://sk.wgjwhj.cn

SQL ............ 90
来源：http://rz.colortex.cn

Bash ........... 80
来源：http://cz.chemitech.net.cn

Kotlin ......... 15
来源：http://np.bookmarksfly.cn

Swift .......... 15
来源：http://fu.gzmigu.cn

Lua ............ 10
来源：http://ja.szsharing.cn

Perl ........... 10
来源：http://us.newstarts.cn

Scala .......... 10
来源：http://uw.szsharing.cn

------------------------------------
来源：http://ks.hnjuh.cn

合计 ........... 2106 条
来源：http://or.panjiajie.cn

按章节统计：
来源：http://yl.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oq.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ap.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uq.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lh.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://th.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://et.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kh.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yy.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iq.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ya.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ku.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xs.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wt.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gu.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ry.shxzukj.cn

Q SQL 专题                              90
来源：http://em.jctech888.com.cn

R Bash 专题                             80
来源：http://ez.szsharing.cn

S C / C++ 专题                          60
来源：http://jp.9csxet.cn

T 其他语言补充                          60
来源：http://xs.haigaiapp.cn

U 高频实用片段                         120
来源：http://qc.huixinmuqiang.cn

------------------------------------
来源：http://iu.asd995.cn

合计                                  2106 条
来源：http://zh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://au.jianghongdianzi.cn

使用提醒
来源：http://ab.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://su.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pe.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rq.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yk.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bz.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ag.521024.cn

—— 文件结束 ——
来源：http://qw.asd995.cn

================================================================================
来源：http://yd.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://zi.521024.cn

Common Programming Examples Cheat Book
来源：http://kf.shtwfgs.cn

================================================================================
来源：http://oy.szsharing.cn

【收录内容】
来源：http://lz.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://du.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yt.newstarts.cn

SQL · Bash · C · C++
来源：http://rs.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ki.lnxyls.cn

【使用说明】
来源：http://qu.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gs.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oh.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eh.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xc.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://of.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xu.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://up.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qb.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qu.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sq.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bf.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ip.shxzskj.cn

【文件统计】
来源：http://aw.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xh.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://hv.huixiangedu.cn

目  录
来源：http://le.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bq.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dq.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ro.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ci.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ff.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nf.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qb.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nd.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pq.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eo.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://th.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rd.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tr.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ev.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zw.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zn.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nm.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gd.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://no.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jg.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xf.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qz.szsharing.cn

================================================================================
来源：http://wc.muxihuayi.cn

A. 基础语法与类型
来源：http://wv.muxihuayi.cn

================================================================================
来源：http://mx.haigaiapp.cn

[A01] Hello World
来源：http://wy.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://dx.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://kb.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://vq.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gp.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://xt.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://vg.521024.cn

Ruby: puts "Hello, World!"
来源：http://ia.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mu.521024.cn

[A02] 变量声明与赋值
来源：http://ky.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pb.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yj.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mm.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uf.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://fr.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://hb.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://hh.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aq.muxihuayi.cn

[A03] 常量定义
来源：http://fj.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ro.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://nk.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://lh.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://si.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://lu.lnxyls.cn

Go:   const PI = 3.14159
来源：http://zy.asd995.cn

Ruby: PI = 3.14159
来源：http://vm.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://va.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://py.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hi.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cb.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ct.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://wu.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://to.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rt.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dc.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://tc.yuexingan06.cn

[A05] 整数除法与取模
来源：http://ii.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ha.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ah.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gd.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gt.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://ui.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://gg.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://xx.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://wk.newstarts.cn

[A06] 字符串转数字
来源：http://kj.asd995.cn

Py:   int("42"); float("3.14")
来源：http://yf.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ug.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://of.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fl.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uu.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yy.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mn.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ci.521024.cn

[A07] 数字转字符串
来源：http://gf.colortex.cn

Py:   str(42)
来源：http://fc.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://fq.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://gs.bookmarksfly.cn

TS:   String(42)
来源：http://wx.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ie.asd995.cn

Go:   strconv.Itoa(42)
来源：http://qq.szsharing.cn

Ruby: 42.to_s
来源：http://sg.huixiangedu.cn

C#:   42.ToString()
来源：http://ng.hnjuh.cn

[A08] 取整与四舍五入
来源：http://jp.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://te.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gq.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ci.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wy.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gf.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zd.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wu.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ml.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://sx.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cg.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tw.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xb.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ze.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://et.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jg.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kv.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xn.nszjky.cn

[A10] 生成随机数
来源：http://uy.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://oh.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://pr.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ue.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ad.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://mu.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ee.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://py.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://zu.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://yv.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://xu.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hs.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yf.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ji.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://tl.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rt.gzmigu.cn


<!-- 参考信息 -->