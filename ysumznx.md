代发 wailian999

[U67] PHP：处理文件上传
来源：http://qv.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tb.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://vb.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://la.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://lj.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aj.hahajie.cn

[U70] PHP：PDO 事务
来源：http://qw.panjiajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://da.panjiajie.cn

[U71] PHP：抛出异常
来源：http://nw.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://rz.szxytkj.cn

[U72] PHP：写错误日志
来源：http://mo.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://ou.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://lo.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://wt.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://vi.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://sv.shxzukj.cn

[U75] PHP：依赖注入
来源：http://gp.bjjhwx.cn

composer require psr/container
来源：http://io.gzmigu.cn

[U76] PHP：简单路由
来源：http://gj.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://np.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://tb.shxzskj.cn

composer require twig/twig
来源：http://ii.nicolike.cn

[U78] PHP：单元测试
来源：http://ze.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://lx.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://uz.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://qv.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://ej.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hg.chemitech.net.cn

[U81] JS：初始化项目
来源：http://ox.hahajie.cn

npm init -y;  npm i express
来源：http://ku.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://an.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mp.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://mh.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qv.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://it.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ck.gzmigu.cn

[U85] JS：可选链
来源：http://lr.szxytkj.cn

a?.b?.c
来源：http://hp.bookmarksfly.cn

[U86] JS：空值合并
来源：http://vl.shxzskj.cn

a ?? b
来源：http://ko.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://pn.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://kd.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://rl.panjiajie.cn

{ ...a, ...b }
来源：http://dt.muxihuayi.cn

[U89] JS：数组去重
来源：http://of.haigaiapp.cn

[...new Set(arr)]
来源：http://pq.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://lc.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://kc.szsharing.cn

[U91] JS：对象键值遍历
来源：http://kg.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aq.haigaiapp.cn

[U92] JS：深拷贝
来源：http://ou.hahajie.cn

structuredClone(obj)
来源：http://ps.huanxung.cn

[U93] JS：模板字符串
来源：http://uq.521024.cn

`共 ${n} 条`
来源：http://ym.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ib.521024.cn

const double = x => x * 2;
来源：http://mn.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://ly.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://kj.nszjky.cn

[U96] JS：async/await 与异常
来源：http://lx.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lr.jctech888.com.cn

[U97] JS：并发请求
来源：http://vt.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ja.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://wv.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://li.gzmigu.cn

[U99] JS：事件监听
来源：http://ts.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://pa.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://mq.muxihuayi.cn

document.querySelector(".item")
来源：http://fq.nszjky.cn

[U101] JS：classList 操作
来源：http://op.yuexingan06.cn

el.classList.toggle("active")
来源：http://uo.bjjhwx.cn

[U102] JS：本地存储
来源：http://lj.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ce.szxytkj.cn

[U103] JS：定时器
来源：http://oz.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ui.521024.cn

[U104] JS：防抖
来源：http://lx.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fe.nicolike.cn

[U105] JS：节流
来源：http://kb.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oa.huixiangedu.cn

[U106] JS：日期格式化
来源：http://ja.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gy.bjjhwx.cn

[U107] JS：数字千分位
来源：http://zh.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zz.yuexingan06.cn

[U108] JS：随机整数
来源：http://ia.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ol.521024.cn

[U109] JS：数组分组
来源：http://we.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://sj.lnxyls.cn

[U110] JS：数组分块
来源：http://ag.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hn.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://hk.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://ym.szxytkj.cn

[U112] JS：字符串补位
来源：http://ea.muxihuayi.cn

"7".padStart(3, "0")
来源：http://vw.huanxung.cn

[U113] JS：正则替换全部
来源：http://ax.nicolike.cn

s.replaceAll("a", "b")
来源：http://uq.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://uf.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vd.hahajie.cn

[U115] JS：生成 UUID
来源：http://mb.bjjhwx.cn

crypto.randomUUID()
来源：http://lz.jianghongdianzi.cn

[U116] JS：类型检查（JSDoc）
来源：http://qk.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://zo.jctech888.com.cn

[U117] JS：单元测试
来源：http://cd.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://zw.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://vu.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://iy.hahajie.cn

[U119] JS：生产构建
来源：http://gr.haigaiapp.cn

npx vite build
来源：http://py.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://ez.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://zi.521024.cn

================================================================================
来源：http://qr.yuntaijiaju.cn

统计汇总
来源：http://sx.nicolike.cn

================================================================================
来源：http://xt.asd995.cn

按语言统计（条）：
来源：http://zh.hnjuh.cn

Python ......... 252
来源：http://gi.jianghongdianzi.cn

PHP ............ 252
来源：http://hc.colortex.cn

JavaScript ..... 252
来源：http://ka.asd995.cn

TypeScript ..... 212
来源：http://yd.colortex.cn

Java ........... 212
来源：http://jn.nicolike.cn

Go ............. 212
来源：http://mc.hahajie.cn

Ruby ........... 212
来源：http://nq.wgjwhj.cn

C# ............. 212
来源：http://oh.colortex.cn

C .............. 30
来源：http://fo.muxihuayi.cn

C++ ............ 30
来源：http://kf.jianghongdianzi.cn

SQL ............ 90
来源：http://jr.hahajie.cn

Bash ........... 80
来源：http://pd.shxzukj.cn

Kotlin ......... 15
来源：http://eb.huanxung.cn

Swift .......... 15
来源：http://kq.jianghongdianzi.cn

Lua ............ 10
来源：http://cw.9csxet.cn

Perl ........... 10
来源：http://ei.shxzskj.cn

Scala .......... 10
来源：http://wx.jianghongdianzi.cn

------------------------------------
来源：http://mw.huanxung.cn

合计 ........... 2106 条
来源：http://bk.panjiajie.cn

按章节统计：
来源：http://sz.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lc.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ki.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kq.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ik.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pk.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fd.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uy.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tb.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vl.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lt.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aj.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aq.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://an.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nj.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ln.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ma.lnxyls.cn

Q SQL 专题                              90
来源：http://so.nszjky.cn

R Bash 专题                             80
来源：http://wu.jctech888.com.cn

S C / C++ 专题                          60
来源：http://fr.nicolike.cn

T 其他语言补充                          60
来源：http://kp.huixiangedu.cn

U 高频实用片段                         120
来源：http://wa.9csxet.cn

------------------------------------
来源：http://yq.asd995.cn

合计                                  2106 条
来源：http://tf.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://at.szsharing.cn

使用提醒
来源：http://ju.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://gb.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://et.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ch.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ah.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yz.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fp.yuntaijiaju.cn

—— 文件结束 ——
来源：http://hx.muxihuayi.cn

================================================================================
来源：http://ut.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://el.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://ko.newstarts.cn

================================================================================
来源：http://dj.bjjhwx.cn

【收录内容】
来源：http://dm.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ao.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fk.szxytkj.cn

SQL · Bash · C · C++
来源：http://ca.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bd.hahajie.cn

【使用说明】
来源：http://jy.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yp.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iw.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ji.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cu.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dk.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ps.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zr.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hx.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bn.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zo.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ls.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nb.lnxyls.cn

【文件统计】
来源：http://qo.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yb.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://mc.yuexingan06.cn

目  录
来源：http://ub.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://zr.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://at.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xd.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dr.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sv.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iu.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mh.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ap.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dt.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jy.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wr.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ra.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zr.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qr.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ys.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ab.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gr.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ey.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://be.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://er.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oa.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lp.jianghongdianzi.cn

================================================================================
来源：http://fs.bookmarksfly.cn

A. 基础语法与类型
来源：http://hf.bookmarksfly.cn

================================================================================
来源：http://qx.521024.cn

[A01] Hello World
来源：http://ei.shxzskj.cn

Py:   print("Hello, World!")
来源：http://ue.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://lm.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://oc.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gr.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://qv.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ib.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://bu.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wz.hahajie.cn

[A02] 变量声明与赋值
来源：http://or.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bk.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ie.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sy.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gc.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://xw.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://jh.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://hz.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ja.haigaiapp.cn

[A03] 常量定义
来源：http://ea.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://si.521024.cn

PHP:  const PI = 3.14159;
来源：http://ib.asd995.cn

JS:   const PI = 3.14159;
来源：http://cf.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://he.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://ze.lnxyls.cn

Go:   const PI = 3.14159
来源：http://dw.lnxyls.cn

Ruby: PI = 3.14159
来源：http://ud.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://pm.hahajie.cn

[A04] 判断变量类型
来源：http://jm.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tq.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ak.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ue.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://cy.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jz.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wz.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jl.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://fj.wgjwhj.cn

[A05] 整数除法与取模
来源：http://gp.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://os.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dk.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://it.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vw.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://ql.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://hf.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://kh.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://jb.asd995.cn

[A06] 字符串转数字
来源：http://fn.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://eu.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ge.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mg.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xy.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ua.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ix.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hg.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ux.nszjky.cn

[A07] 数字转字符串
来源：http://rd.bjjhwx.cn

Py:   str(42)
来源：http://cy.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://qq.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://jm.shxzukj.cn

TS:   String(42)
来源：http://un.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gs.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://jb.wgjwhj.cn

Ruby: 42.to_s
来源：http://ny.yuntaijiaju.cn

C#:   42.ToString()
来源：http://ir.shxzukj.cn

[A08] 取整与四舍五入
来源：http://xy.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qk.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sy.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zk.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gp.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pi.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://in.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://av.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://at.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://ma.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ni.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://so.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dt.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ap.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kc.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qj.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gi.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wr.szsharing.cn

[A10] 生成随机数
来源：http://he.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://hk.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://du.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qm.szsharing.cn


<!-- 参考信息 -->