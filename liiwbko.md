代发 wailian999

[U67] PHP：处理文件上传
来源：http://sp.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pz.asd995.cn

[U68] PHP：PDO 连接
来源：http://ox.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ak.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://lk.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gw.nicolike.cn

[U70] PHP：PDO 事务
来源：http://eh.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://en.9csxet.cn

[U71] PHP：抛出异常
来源：http://tq.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://df.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://ra.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://cp.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://lf.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://el.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://dm.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://uo.hnjuh.cn

[U75] PHP：依赖注入
来源：http://jk.szxytkj.cn

composer require psr/container
来源：http://hw.asd995.cn

[U76] PHP：简单路由
来源：http://gt.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ah.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://qt.colortex.cn

composer require twig/twig
来源：http://gl.asd995.cn

[U78] PHP：单元测试
来源：http://aj.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://aa.haigaiapp.cn

[U79] PHP：静态分析
来源：http://zz.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://wt.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://pm.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cy.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://lw.wgjwhj.cn

npm init -y;  npm i express
来源：http://wc.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://fx.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://md.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://np.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yd.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://rt.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nb.szsharing.cn

[U85] JS：可选链
来源：http://ew.shxzukj.cn

a?.b?.c
来源：http://sb.huixiangedu.cn

[U86] JS：空值合并
来源：http://fs.jianghongdianzi.cn

a ?? b
来源：http://yj.szxytkj.cn

[U87] JS：解构默认值
来源：http://ja.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://rs.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://tt.haigaiapp.cn

{ ...a, ...b }
来源：http://zm.szxytkj.cn

[U89] JS：数组去重
来源：http://kq.colortex.cn

[...new Set(arr)]
来源：http://qv.hahajie.cn

[U90] JS：数字数组排序
来源：http://sb.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://il.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://js.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vl.asd995.cn

[U92] JS：深拷贝
来源：http://bq.jctech888.com.cn

structuredClone(obj)
来源：http://eo.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://hf.huixiangedu.cn

`共 ${n} 条`
来源：http://yr.szsharing.cn

[U94] JS：箭头函数
来源：http://cc.huixinmuqiang.cn

const double = x => x * 2;
来源：http://eb.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://of.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://wp.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://hv.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vi.wgjwhj.cn

[U97] JS：并发请求
来源：http://gf.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ta.huixinmuqiang.cn

[U98] JS：fetch 带 JSON
来源：http://qi.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ri.newstarts.cn

[U99] JS：事件监听
来源：http://gk.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://jw.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://xc.newstarts.cn

document.querySelector(".item")
来源：http://pe.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://fk.shxzukj.cn

el.classList.toggle("active")
来源：http://ag.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://uv.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sy.wgjwhj.cn

[U103] JS：定时器
来源：http://xs.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://it.szxytkj.cn

[U104] JS：防抖
来源：http://zc.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xq.huixinmuqiang.cn

[U105] JS：节流
来源：http://pt.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zg.9csxet.cn

[U106] JS：日期格式化
来源：http://gt.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://av.chemitech.net.cn

[U107] JS：数字千分位
来源：http://eb.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sv.hahajie.cn

[U108] JS：随机整数
来源：http://cr.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://od.szsharing.cn

[U109] JS：数组分组
来源：http://wu.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://dg.nicolike.cn

[U110] JS：数组分块
来源：http://cs.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wr.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://cw.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://ev.yuexingan06.cn

[U112] JS：字符串补位
来源：http://xz.shxzskj.cn

"7".padStart(3, "0")
来源：http://so.hnjuh.cn

[U113] JS：正则替换全部
来源：http://cy.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://gw.asd995.cn

[U114] JS：JSON 深比较
来源：http://sr.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uz.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://ih.lnxyls.cn

crypto.randomUUID()
来源：http://zx.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://gx.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ln.yuexingan06.cn

[U117] JS：单元测试
来源：http://ew.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://th.szxytkj.cn

[U118] JS：开发服务器
来源：http://ih.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://dc.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://fi.jianghongdianzi.cn

npx vite build
来源：http://ng.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ss.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://ja.yuexingan06.cn

================================================================================
来源：http://bz.hnjuh.cn

统计汇总
来源：http://ka.haigaiapp.cn

================================================================================
来源：http://tq.chemitech.net.cn

按语言统计（条）：
来源：http://az.colortex.cn

Python ......... 252
来源：http://xs.shtwfgs.cn

PHP ............ 252
来源：http://zr.szsharing.cn

JavaScript ..... 252
来源：http://su.hahajie.cn

TypeScript ..... 212
来源：http://sf.wgjwhj.cn

Java ........... 212
来源：http://vn.hahajie.cn

Go ............. 212
来源：http://wp.hnjuh.cn

Ruby ........... 212
来源：http://oi.hnjuh.cn

C# ............. 212
来源：http://lv.shtwfgs.cn

C .............. 30
来源：http://mo.521024.cn

C++ ............ 30
来源：http://qe.nicolike.cn

SQL ............ 90
来源：http://af.hnjuh.cn

Bash ........... 80
来源：http://ws.9csxet.cn

Kotlin ......... 15
来源：http://mr.chemitech.net.cn

Swift .......... 15
来源：http://ef.9csxet.cn

Lua ............ 10
来源：http://kv.hahajie.cn

Perl ........... 10
来源：http://fo.jianghongdianzi.cn

Scala .......... 10
来源：http://uj.nicolike.cn

------------------------------------
来源：http://ok.panjiajie.cn

合计 ........... 2106 条
来源：http://jg.nszjky.cn

按章节统计：
来源：http://ho.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://at.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kt.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nk.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vu.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pc.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eo.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gy.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oj.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pe.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zc.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mp.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xb.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sr.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ef.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yr.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xv.nszjky.cn

Q SQL 专题                              90
来源：http://ee.shxzskj.cn

R Bash 专题                             80
来源：http://vs.huanxung.cn

S C / C++ 专题                          60
来源：http://wg.gzmigu.cn

T 其他语言补充                          60
来源：http://it.colortex.cn

U 高频实用片段                         120
来源：http://rb.nszjky.cn

------------------------------------
来源：http://te.shtwfgs.cn

合计                                  2106 条
来源：http://oe.newstarts.cn

--------------------------------------------------------------------------------
来源：http://td.asd995.cn

使用提醒
来源：http://cs.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://qj.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sy.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zz.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gl.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fk.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hj.newstarts.cn

—— 文件结束 ——
来源：http://dp.huixiangedu.cn

================================================================================
来源：http://bl.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://fp.szsharing.cn

Common Programming Examples Cheat Book
来源：http://jc.jianghongdianzi.cn

================================================================================
来源：http://ct.jianghongdianzi.cn

【收录内容】
来源：http://ko.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vv.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qs.newstarts.cn

SQL · Bash · C · C++
来源：http://ef.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ud.huixinmuqiang.cn

【使用说明】
来源：http://qc.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sp.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yn.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hv.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://os.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ce.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uo.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://md.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jy.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zi.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xa.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dq.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wk.521024.cn

【文件统计】
来源：http://qd.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ab.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://dw.panjiajie.cn

目  录
来源：http://ac.colortex.cn

--------------------------------------------------------------------------------
来源：http://ij.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oi.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ut.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ke.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fu.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://of.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qr.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qv.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rd.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yv.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://th.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vg.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oz.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cr.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jy.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mv.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dj.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cp.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hy.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ys.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://wo.wgjwhj.cn

A. 基础语法与类型
来源：http://bg.bookmarksfly.cn

================================================================================
来源：http://jn.huixiangedu.cn

[A01] Hello World
来源：http://ko.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ad.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://ce.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://qa.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zt.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://js.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://bl.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://fc.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lz.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://dz.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qn.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ap.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jk.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tz.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://mn.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://cq.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://gq.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://st.nszjky.cn

[A03] 常量定义
来源：http://cj.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vr.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://vq.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://fi.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://jp.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://sw.huanxung.cn

Go:   const PI = 3.14159
来源：http://cq.nicolike.cn

Ruby: PI = 3.14159
来源：http://ak.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://iu.lnxyls.cn

[A04] 判断变量类型
来源：http://wn.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rt.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ao.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cd.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://qk.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vi.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zy.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bq.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://tk.hahajie.cn

[A05] 整数除法与取模
来源：http://kn.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ze.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xt.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vr.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bv.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://lq.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://kf.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://el.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://nk.chemitech.net.cn

[A06] 字符串转数字
来源：http://bc.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://eq.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zy.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qq.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yd.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gk.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cw.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xr.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nn.hnjuh.cn

[A07] 数字转字符串
来源：http://be.hahajie.cn

Py:   str(42)
来源：http://ch.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://kt.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://lx.huixiangedu.cn

TS:   String(42)
来源：http://rc.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ou.asd995.cn

Go:   strconv.Itoa(42)
来源：http://np.gzmigu.cn

Ruby: 42.to_s
来源：http://il.haigaiapp.cn

C#:   42.ToString()
来源：http://zb.szsharing.cn

[A08] 取整与四舍五入
来源：http://xw.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yo.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yy.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gk.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zs.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qg.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yx.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qd.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bk.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://at.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mf.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qm.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zf.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dx.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sq.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vn.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ws.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lh.szsharing.cn

[A10] 生成随机数
来源：http://vy.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://cj.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://bn.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xh.bookmarksfly.cn


<!-- 参考信息 -->