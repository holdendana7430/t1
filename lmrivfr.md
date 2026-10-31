代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://vs.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://ow.szsharing.cn

[U74] PHP：读取环境变量
来源：http://zv.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://eg.panjiajie.cn

[U75] PHP：依赖注入
来源：http://sc.521024.cn

composer require psr/container
来源：http://xu.9csxet.cn

[U76] PHP：简单路由
来源：http://hn.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zr.9csxet.cn

[U77] PHP：模板渲染
来源：http://ba.gzmigu.cn

composer require twig/twig
来源：http://uv.9csxet.cn

[U78] PHP：单元测试
来源：http://ki.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://mi.huanxung.cn

[U79] PHP：静态分析
来源：http://gq.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://cr.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://ea.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://da.yuexingan06.cn

[U81] JS：初始化项目
来源：http://uw.chemitech.net.cn

npm init -y;  npm i express
来源：http://pu.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://sm.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tw.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://wy.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://py.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://gj.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pp.9csxet.cn

[U85] JS：可选链
来源：http://gn.bjjhwx.cn

a?.b?.c
来源：http://oq.asd995.cn

[U86] JS：空值合并
来源：http://fe.huixinmuqiang.cn

a ?? b
来源：http://ue.521024.cn

[U87] JS：解构默认值
来源：http://yj.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ct.panjiajie.cn

[U88] JS：对象展开合并
来源：http://sa.huixinmuqiang.cn

{ ...a, ...b }
来源：http://jv.chemitech.net.cn

[U89] JS：数组去重
来源：http://pw.asd995.cn

[...new Set(arr)]
来源：http://ab.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://yi.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://tz.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://jz.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yn.asd995.cn

[U92] JS：深拷贝
来源：http://oy.huanxung.cn

structuredClone(obj)
来源：http://wu.bjjhwx.cn

[U93] JS：模板字符串
来源：http://he.nszjky.cn

`共 ${n} 条`
来源：http://lj.muxihuayi.cn

[U94] JS：箭头函数
来源：http://qa.shxzskj.cn

const double = x => x * 2;
来源：http://sb.shxzukj.cn

[U95] JS：Promise 包装
来源：http://dp.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://hm.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://ie.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zp.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://ob.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qa.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://mf.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yl.shtwfgs.cn

[U99] JS：事件监听
来源：http://dd.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://ux.9csxet.cn

[U100] JS：DOM 查询
来源：http://hf.newstarts.cn

document.querySelector(".item")
来源：http://gx.jctech888.com.cn

[U101] JS：classList 操作
来源：http://xq.newstarts.cn

el.classList.toggle("active")
来源：http://vg.gzmigu.cn

[U102] JS：本地存储
来源：http://qj.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qa.huanxung.cn

[U103] JS：定时器
来源：http://vk.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kz.colortex.cn

[U104] JS：防抖
来源：http://ah.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aj.shxzukj.cn

[U105] JS：节流
来源：http://ro.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yo.shxzukj.cn

[U106] JS：日期格式化
来源：http://lu.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cq.huanxung.cn

[U107] JS：数字千分位
来源：http://ed.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sf.nszjky.cn

[U108] JS：随机整数
来源：http://px.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xn.gzmigu.cn

[U109] JS：数组分组
来源：http://dl.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://vf.szxytkj.cn

[U110] JS：数组分块
来源：http://mv.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sx.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://ga.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://is.9csxet.cn

[U112] JS：字符串补位
来源：http://hf.huanxung.cn

"7".padStart(3, "0")
来源：http://ko.asd995.cn

[U113] JS：正则替换全部
来源：http://pu.9csxet.cn

s.replaceAll("a", "b")
来源：http://up.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://go.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sp.colortex.cn

[U115] JS：生成 UUID
来源：http://sm.newstarts.cn

crypto.randomUUID()
来源：http://qf.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://zy.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://tl.yuexingan06.cn

[U117] JS：单元测试
来源：http://lb.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://rp.lnxyls.cn

[U118] JS：开发服务器
来源：http://yp.colortex.cn

npm i -D vite;  npx vite
来源：http://zm.521024.cn

[U119] JS：生产构建
来源：http://hw.hnjuh.cn

npx vite build
来源：http://ab.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://tw.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://ma.shxzskj.cn

================================================================================
来源：http://ep.huixiangedu.cn

统计汇总
来源：http://hs.lnxyls.cn

================================================================================
来源：http://by.521024.cn

按语言统计（条）：
来源：http://ub.szsharing.cn

Python ......... 252
来源：http://sc.muxihuayi.cn

PHP ............ 252
来源：http://nz.bookmarksfly.cn

JavaScript ..... 252
来源：http://qk.shtwfgs.cn

TypeScript ..... 212
来源：http://nd.lnxyls.cn

Java ........... 212
来源：http://kp.shtwfgs.cn

Go ............. 212
来源：http://qh.9csxet.cn

Ruby ........... 212
来源：http://if.9csxet.cn

C# ............. 212
来源：http://fs.nszjky.cn

C .............. 30
来源：http://ny.lnxyls.cn

C++ ............ 30
来源：http://dv.huixiangedu.cn

SQL ............ 90
来源：http://kt.shxzukj.cn

Bash ........... 80
来源：http://op.9csxet.cn

Kotlin ......... 15
来源：http://zf.szxytkj.cn

Swift .......... 15
来源：http://js.yuexingan06.cn

Lua ............ 10
来源：http://iz.bookmarksfly.cn

Perl ........... 10
来源：http://bs.asd995.cn

Scala .......... 10
来源：http://cv.szxytkj.cn

------------------------------------
来源：http://ih.szxytkj.cn

合计 ........... 2106 条
来源：http://gy.hahajie.cn

按章节统计：
来源：http://bd.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fj.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yw.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fq.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bi.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nv.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xb.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kc.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zw.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yd.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vk.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qw.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gb.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bz.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zy.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rr.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nu.muxihuayi.cn

Q SQL 专题                              90
来源：http://kp.hahajie.cn

R Bash 专题                             80
来源：http://yf.huanxung.cn

S C / C++ 专题                          60
来源：http://ek.huixiangedu.cn

T 其他语言补充                          60
来源：http://fx.bjjhwx.cn

U 高频实用片段                         120
来源：http://gb.yuntaijiaju.cn

------------------------------------
来源：http://ws.yuntaijiaju.cn

合计                                  2106 条
来源：http://mt.newstarts.cn

--------------------------------------------------------------------------------
来源：http://xp.colortex.cn

使用提醒
来源：http://ec.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://iz.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yq.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zs.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ts.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fw.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://or.asd995.cn

—— 文件结束 ——
来源：http://fb.huanxung.cn

================================================================================
来源：http://sp.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://oz.nszjky.cn

Common Programming Examples Cheat Book
来源：http://jr.yuexingan06.cn

================================================================================
来源：http://wc.huixinmuqiang.cn

【收录内容】
来源：http://es.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://si.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://av.szxytkj.cn

SQL · Bash · C · C++
来源：http://mn.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wz.haigaiapp.cn

【使用说明】
来源：http://ik.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qz.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xf.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gj.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://el.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sj.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iy.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iz.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fp.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rb.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gx.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hp.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fb.shxzukj.cn

【文件统计】
来源：http://uf.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ko.huixiangedu.cn

目  录
来源：http://sg.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://pk.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gr.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fr.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cb.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jo.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eh.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://po.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gq.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wu.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lb.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ch.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cj.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hs.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ah.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ul.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gr.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ra.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kg.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sr.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ti.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vo.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pa.yuntaijiaju.cn

================================================================================
来源：http://ww.gzmigu.cn

A. 基础语法与类型
来源：http://ov.hnjuh.cn

================================================================================
来源：http://qq.colortex.cn

[A01] Hello World
来源：http://ux.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://ua.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://nm.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://as.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mh.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://lu.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://pk.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://ai.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ev.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://so.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ck.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wt.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tp.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dz.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://db.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://wb.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://az.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://np.bookmarksfly.cn

[A03] 常量定义
来源：http://xp.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lc.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://di.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://mq.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://ys.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://rt.colortex.cn

Go:   const PI = 3.14159
来源：http://cq.gzmigu.cn

Ruby: PI = 3.14159
来源：http://lp.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://vz.colortex.cn

[A04] 判断变量类型
来源：http://qq.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://td.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ou.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://im.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://qu.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ea.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qv.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kt.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://pc.hahajie.cn

[A05] 整数除法与取模
来源：http://ku.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lf.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cx.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tn.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jv.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://bi.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://yx.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://gl.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://cl.panjiajie.cn

[A06] 字符串转数字
来源：http://ap.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://qu.jctech888.com.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ib.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://om.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nw.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qo.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nj.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ix.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jf.huixiangedu.cn

[A07] 数字转字符串
来源：http://bt.yuexingan06.cn

Py:   str(42)
来源：http://ia.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://kt.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://fk.gzmigu.cn

TS:   String(42)
来源：http://lw.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xj.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://bf.muxihuayi.cn

Ruby: 42.to_s
来源：http://qs.asd995.cn

C#:   42.ToString()
来源：http://pk.newstarts.cn

[A08] 取整与四舍五入
来源：http://yr.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hf.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pa.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sy.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pb.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://km.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gv.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bz.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eb.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://jj.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xq.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sw.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://al.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qk.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tj.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hx.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jz.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bn.panjiajie.cn

[A10] 生成随机数
来源：http://hc.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://hn.hahajie.cn

PHP:  random_int(1, 100);
来源：http://fh.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ib.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://le.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://ga.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zz.nicolike.cn

Ruby: rand(1..100)
来源：http://ho.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://lo.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ra.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://pt.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nz.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vb.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://or.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ms.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iy.gzmigu.cn


<!-- 参考信息 -->