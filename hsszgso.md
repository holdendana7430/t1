代发 wailian999

[U67] PHP：处理文件上传
来源：http://hg.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oy.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://zu.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vk.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://sd.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hl.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://ip.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vq.nszjky.cn

[U71] PHP：抛出异常
来源：http://sh.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://di.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://vd.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://qw.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://ng.asd995.cn

parse_ini_file("config.ini", true)
来源：http://wt.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://hl.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://pb.shxzskj.cn

[U75] PHP：依赖注入
来源：http://lj.521024.cn

composer require psr/container
来源：http://nw.shxzukj.cn

[U76] PHP：简单路由
来源：http://er.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://er.hnjuh.cn

[U77] PHP：模板渲染
来源：http://vl.hnjuh.cn

composer require twig/twig
来源：http://wv.nszjky.cn

[U78] PHP：单元测试
来源：http://uq.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://al.shxzukj.cn

[U79] PHP：静态分析
来源：http://jl.asd995.cn

composer require --dev phpstan/phpstan
来源：http://nh.newstarts.cn

[U80] PHP：代码规范修复
来源：http://ae.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://su.gzmigu.cn

[U81] JS：初始化项目
来源：http://vk.haigaiapp.cn

npm init -y;  npm i express
来源：http://bb.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://vg.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ju.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://qn.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://io.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://jn.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lm.521024.cn

[U85] JS：可选链
来源：http://mu.9csxet.cn

a?.b?.c
来源：http://yp.bookmarksfly.cn

[U86] JS：空值合并
来源：http://sq.haigaiapp.cn

a ?? b
来源：http://tc.chemitech.net.cn

[U87] JS：解构默认值
来源：http://jr.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://bg.szxytkj.cn

[U88] JS：对象展开合并
来源：http://vp.shtwfgs.cn

{ ...a, ...b }
来源：http://gg.colortex.cn

[U89] JS：数组去重
来源：http://iz.9csxet.cn

[...new Set(arr)]
来源：http://ci.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://fx.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://dx.521024.cn

[U91] JS：对象键值遍历
来源：http://re.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zn.haigaiapp.cn

[U92] JS：深拷贝
来源：http://is.bookmarksfly.cn

structuredClone(obj)
来源：http://bh.shtwfgs.cn

[U93] JS：模板字符串
来源：http://hx.bookmarksfly.cn

`共 ${n} 条`
来源：http://dd.yuntaijiaju.cn

[U94] JS：箭头函数
来源：http://ii.yuexingan06.cn

const double = x => x * 2;
来源：http://la.521024.cn

[U95] JS：Promise 包装
来源：http://yz.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://kr.nszjky.cn

[U96] JS：async/await 与异常
来源：http://sx.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qa.bjjhwx.cn

[U97] JS：并发请求
来源：http://sj.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jy.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://ht.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kg.jctech888.com.cn

[U99] JS：事件监听
来源：http://hg.521024.cn

el.addEventListener("click", e => {})
来源：http://ie.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://dz.panjiajie.cn

document.querySelector(".item")
来源：http://tg.haigaiapp.cn

[U101] JS：classList 操作
来源：http://pv.yuexingan06.cn

el.classList.toggle("active")
来源：http://ju.huanxung.cn

[U102] JS：本地存储
来源：http://gl.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jf.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ed.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://az.huanxung.cn

[U104] JS：防抖
来源：http://ej.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rg.9csxet.cn

[U105] JS：节流
来源：http://pj.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kf.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://jq.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cd.nszjky.cn

[U107] JS：数字千分位
来源：http://bh.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qq.gzmigu.cn

[U108] JS：随机整数
来源：http://ow.huixiangedu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cj.hahajie.cn

[U109] JS：数组分组
来源：http://ys.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://wa.hahajie.cn

[U110] JS：数组分块
来源：http://wv.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yo.9csxet.cn

[U111] JS：对象转 Map
来源：http://il.asd995.cn

new Map(Object.entries(obj))
来源：http://mm.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://lh.colortex.cn

"7".padStart(3, "0")
来源：http://yk.szsharing.cn

[U113] JS：正则替换全部
来源：http://ev.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://fs.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://xo.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ju.gzmigu.cn

[U115] JS：生成 UUID
来源：http://gx.jctech888.com.cn

crypto.randomUUID()
来源：http://uj.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tx.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://fs.bjjhwx.cn

[U117] JS：单元测试
来源：http://xd.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://pb.szsharing.cn

[U118] JS：开发服务器
来源：http://rv.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://gh.shxzukj.cn

[U119] JS：生产构建
来源：http://en.lnxyls.cn

npx vite build
来源：http://up.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://hm.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://vy.newstarts.cn

================================================================================
来源：http://ob.szxytkj.cn

统计汇总
来源：http://ra.yuntaijiaju.cn

================================================================================
来源：http://th.newstarts.cn

按语言统计（条）：
来源：http://tg.wgjwhj.cn

Python ......... 252
来源：http://pe.shtwfgs.cn

PHP ............ 252
来源：http://of.521024.cn

JavaScript ..... 252
来源：http://zw.shxzskj.cn

TypeScript ..... 212
来源：http://jz.haigaiapp.cn

Java ........... 212
来源：http://yc.huixiangedu.cn

Go ............. 212
来源：http://lw.szxytkj.cn

Ruby ........... 212
来源：http://ma.shxzskj.cn

C# ............. 212
来源：http://bl.yuexingan06.cn

C .............. 30
来源：http://dv.szsharing.cn

C++ ............ 30
来源：http://wn.wgjwhj.cn

SQL ............ 90
来源：http://hh.shtwfgs.cn

Bash ........... 80
来源：http://bf.haigaiapp.cn

Kotlin ......... 15
来源：http://yg.hnjuh.cn

Swift .......... 15
来源：http://uv.hahajie.cn

Lua ............ 10
来源：http://lb.shxzskj.cn

Perl ........... 10
来源：http://lw.huixinmuqiang.cn

Scala .......... 10
来源：http://ey.yuntaijiaju.cn

------------------------------------
来源：http://lc.huixiangedu.cn

合计 ........... 2106 条
来源：http://eq.gzmigu.cn

按章节统计：
来源：http://je.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yw.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hy.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ac.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rd.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zo.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aa.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hm.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wv.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zd.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ae.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rq.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kp.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yq.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eo.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mf.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://so.hahajie.cn

Q SQL 专题                              90
来源：http://lt.asd995.cn

R Bash 专题                             80
来源：http://rb.shxzskj.cn

S C / C++ 专题                          60
来源：http://mh.hahajie.cn

T 其他语言补充                          60
来源：http://mw.yuexingan06.cn

U 高频实用片段                         120
来源：http://bk.nicolike.cn

------------------------------------
来源：http://oe.huanxung.cn

合计                                  2106 条
来源：http://qq.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://mf.jctech888.com.cn

使用提醒
来源：http://rg.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ku.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://un.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bp.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rn.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zd.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gt.jctech888.com.cn

—— 文件结束 ——
来源：http://va.hahajie.cn

================================================================================
来源：http://ir.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://cy.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://ps.bookmarksfly.cn

================================================================================
来源：http://bx.huixiangedu.cn

【收录内容】
来源：http://cn.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mu.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sm.muxihuayi.cn

SQL · Bash · C · C++
来源：http://qj.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xw.shxzukj.cn

【使用说明】
来源：http://ab.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://au.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hy.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dd.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hh.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wn.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ga.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lb.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tg.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ag.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fq.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ft.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sv.9csxet.cn

【文件统计】
来源：http://ie.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zg.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ap.jianghongdianzi.cn

目  录
来源：http://la.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://tk.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://td.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mq.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sb.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ie.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xh.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tg.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jd.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sw.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tx.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kc.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yt.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oq.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hf.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xc.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gi.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://co.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://up.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pb.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sl.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ad.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gm.521024.cn

================================================================================
来源：http://tz.haigaiapp.cn

A. 基础语法与类型
来源：http://xr.9csxet.cn

================================================================================
来源：http://ec.haigaiapp.cn

[A01] Hello World
来源：http://ia.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ex.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://ck.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://hk.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gy.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://bw.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ol.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://tb.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jt.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://yd.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ie.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ug.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://aa.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tq.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://po.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://pz.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://jk.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zs.shtwfgs.cn

[A03] 常量定义
来源：http://mu.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wh.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://rj.szsharing.cn

JS:   const PI = 3.14159;
来源：http://oz.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://un.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://dz.9csxet.cn

Go:   const PI = 3.14159
来源：http://av.shxzukj.cn

Ruby: PI = 3.14159
来源：http://cg.colortex.cn

C#:   const double PI = 3.14159;
来源：http://dh.huanxung.cn

[A04] 判断变量类型
来源：http://wp.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hd.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pl.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jz.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://vu.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cj.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eb.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ms.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://jm.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://gc.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sl.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dm.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://va.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mf.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://lk.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://fn.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://og.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ol.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://cx.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://wb.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://md.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://df.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fp.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wx.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ib.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xv.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aw.yuexingan06.cn

[A07] 数字转字符串
来源：http://wc.szxytkj.cn

Py:   str(42)
来源：http://ug.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://xw.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://we.colortex.cn

TS:   String(42)
来源：http://zw.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jj.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://jn.szsharing.cn

Ruby: 42.to_s
来源：http://wp.yuexingan06.cn

C#:   42.ToString()
来源：http://bu.9csxet.cn

[A08] 取整与四舍五入
来源：http://ua.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gj.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ou.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wu.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sk.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zd.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ki.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rf.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rz.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://tf.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ee.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ru.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://al.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bl.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tj.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bv.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://il.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vl.chemitech.net.cn

[A10] 生成随机数
来源：http://rt.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://pi.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://vj.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mf.asd995.cn


<!-- 参考信息 -->