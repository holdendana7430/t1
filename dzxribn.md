代发 wailian999

[U63] PHP：文件读写
来源：http://zv.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ju.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://iz.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://dm.nicolike.cn

[U65] PHP：会话
来源：http://bj.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ur.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://mm.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kd.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://qs.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wv.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://rg.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://si.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://yp.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qs.newstarts.cn

[U70] PHP：PDO 事务
来源：http://kl.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fo.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://mj.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ks.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://cx.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://za.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://gv.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://zk.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://uj.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://zy.lnxyls.cn

[U75] PHP：依赖注入
来源：http://jx.wgjwhj.cn

composer require psr/container
来源：http://zm.colortex.cn

[U76] PHP：简单路由
来源：http://pw.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ot.hahajie.cn

[U77] PHP：模板渲染
来源：http://fv.huixinmuqiang.cn

composer require twig/twig
来源：http://bg.shxzukj.cn

[U78] PHP：单元测试
来源：http://ur.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://xe.colortex.cn

[U79] PHP：静态分析
来源：http://yo.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://cr.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://nd.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://at.lnxyls.cn

[U81] JS：初始化项目
来源：http://nz.9csxet.cn

npm init -y;  npm i express
来源：http://zc.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://bt.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zv.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://km.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ip.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://lb.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ut.jianghongdianzi.cn

[U85] JS：可选链
来源：http://fj.shxzukj.cn

a?.b?.c
来源：http://tb.haigaiapp.cn

[U86] JS：空值合并
来源：http://ld.nicolike.cn

a ?? b
来源：http://ph.colortex.cn

[U87] JS：解构默认值
来源：http://bc.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://qi.szsharing.cn

[U88] JS：对象展开合并
来源：http://hw.haigaiapp.cn

{ ...a, ...b }
来源：http://ny.colortex.cn

[U89] JS：数组去重
来源：http://iq.nszjky.cn

[...new Set(arr)]
来源：http://vd.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://jc.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://it.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://fq.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bi.nicolike.cn

[U92] JS：深拷贝
来源：http://fv.asd995.cn

structuredClone(obj)
来源：http://vf.shxzukj.cn

[U93] JS：模板字符串
来源：http://qp.lnxyls.cn

`共 ${n} 条`
来源：http://mm.colortex.cn

[U94] JS：箭头函数
来源：http://xx.yuntaijiaju.cn

const double = x => x * 2;
来源：http://fd.szsharing.cn

[U95] JS：Promise 包装
来源：http://jg.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://ai.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://ek.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zo.9csxet.cn

[U97] JS：并发请求
来源：http://wq.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://po.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ix.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kj.nszjky.cn

[U99] JS：事件监听
来源：http://jw.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://xg.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://rb.nszjky.cn

document.querySelector(".item")
来源：http://fd.nicolike.cn

[U101] JS：classList 操作
来源：http://ez.asd995.cn

el.classList.toggle("active")
来源：http://df.jctech888.com.cn

[U102] JS：本地存储
来源：http://zx.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jh.shxzukj.cn

[U103] JS：定时器
来源：http://cd.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eq.wgjwhj.cn

[U104] JS：防抖
来源：http://sz.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tb.yuntaijiaju.cn

[U105] JS：节流
来源：http://cy.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cn.hnjuh.cn

[U106] JS：日期格式化
来源：http://on.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hj.colortex.cn

[U107] JS：数字千分位
来源：http://py.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gi.521024.cn

[U108] JS：随机整数
来源：http://bl.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fi.colortex.cn

[U109] JS：数组分组
来源：http://ey.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://xr.nicolike.cn

[U110] JS：数组分块
来源：http://sc.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ki.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://qe.hnjuh.cn

new Map(Object.entries(obj))
来源：http://yo.panjiajie.cn

[U112] JS：字符串补位
来源：http://yf.asd995.cn

"7".padStart(3, "0")
来源：http://ok.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://hh.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://bb.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://in.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mt.szxytkj.cn

[U115] JS：生成 UUID
来源：http://ld.huanxung.cn

crypto.randomUUID()
来源：http://qa.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://tw.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://an.shxzskj.cn

[U117] JS：单元测试
来源：http://xz.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://dm.hahajie.cn

[U118] JS：开发服务器
来源：http://zo.newstarts.cn

npm i -D vite;  npx vite
来源：http://on.newstarts.cn

[U119] JS：生产构建
来源：http://tb.asd995.cn

npx vite build
来源：http://ov.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://ia.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://bd.newstarts.cn

================================================================================
来源：http://dd.bjjhwx.cn

统计汇总
来源：http://np.szxytkj.cn

================================================================================
来源：http://hc.gzmigu.cn

按语言统计（条）：
来源：http://ia.bookmarksfly.cn

Python ......... 252
来源：http://xb.nszjky.cn

PHP ............ 252
来源：http://px.szxytkj.cn

JavaScript ..... 252
来源：http://wz.hnjuh.cn

TypeScript ..... 212
来源：http://qf.huixiangedu.cn

Java ........... 212
来源：http://to.newstarts.cn

Go ............. 212
来源：http://rt.huixiangedu.cn

Ruby ........... 212
来源：http://at.shtwfgs.cn

C# ............. 212
来源：http://ap.nszjky.cn

C .............. 30
来源：http://to.yuntaijiaju.cn

C++ ............ 30
来源：http://rt.hahajie.cn

SQL ............ 90
来源：http://kg.521024.cn

Bash ........... 80
来源：http://ws.gzmigu.cn

Kotlin ......... 15
来源：http://zj.lnxyls.cn

Swift .......... 15
来源：http://wu.nszjky.cn

Lua ............ 10
来源：http://un.hnjuh.cn

Perl ........... 10
来源：http://to.huixiangedu.cn

Scala .......... 10
来源：http://lu.huixinmuqiang.cn

------------------------------------
来源：http://hu.bookmarksfly.cn

合计 ........... 2106 条
来源：http://kb.haigaiapp.cn

按章节统计：
来源：http://wc.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xx.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ja.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mf.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ev.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yl.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ij.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pr.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xt.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ai.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ij.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gn.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cq.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dc.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lq.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xl.haigaiapp.cn

Q SQL 专题                              90
来源：http://hk.9csxet.cn

R Bash 专题                             80
来源：http://du.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://sa.shtwfgs.cn

T 其他语言补充                          60
来源：http://cu.jctech888.com.cn

U 高频实用片段                         120
来源：http://im.haigaiapp.cn

------------------------------------
来源：http://iu.gzmigu.cn

合计                                  2106 条
来源：http://kr.huanxung.cn

--------------------------------------------------------------------------------
来源：http://xp.yuexingan06.cn

使用提醒
来源：http://ma.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://of.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://or.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cq.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://br.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lr.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ym.shtwfgs.cn

—— 文件结束 ——
来源：http://nf.521024.cn

================================================================================
来源：http://jn.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://yx.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://ek.shxzskj.cn

================================================================================
来源：http://wg.nicolike.cn

【收录内容】
来源：http://fb.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fn.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uj.haigaiapp.cn

SQL · Bash · C · C++
来源：http://ky.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kr.chemitech.net.cn

【使用说明】
来源：http://kl.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lf.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wt.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://el.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fs.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tq.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vq.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iz.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sd.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fe.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nd.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gx.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jw.jctech888.com.cn

【文件统计】
来源：http://em.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jn.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://yn.jctech888.com.cn

目  录
来源：http://bg.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://yx.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ka.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fg.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://me.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ws.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tf.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jj.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cc.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oc.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://um.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hg.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tx.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yp.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yd.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qt.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cb.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dt.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xk.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jd.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jc.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gx.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hh.asd995.cn

================================================================================
来源：http://jk.yuntaijiaju.cn

A. 基础语法与类型
来源：http://kf.szsharing.cn

================================================================================
来源：http://lf.yuexingan06.cn

[A01] Hello World
来源：http://ru.lnxyls.cn

Py:   print("Hello, World!")
来源：http://hs.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://ag.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://fo.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dl.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://pu.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://gq.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://zo.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://am.9csxet.cn

[A02] 变量声明与赋值
来源：http://xk.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sg.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qt.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yv.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yv.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://xw.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://ha.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://hv.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xn.jctech888.com.cn

[A03] 常量定义
来源：http://xu.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hk.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://hg.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://jd.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://gq.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://yu.nszjky.cn

Go:   const PI = 3.14159
来源：http://bd.colortex.cn

Ruby: PI = 3.14159
来源：http://im.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://ol.shtwfgs.cn

[A04] 判断变量类型
来源：http://lv.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bh.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zm.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fl.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://lz.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://je.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bc.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kx.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://sb.chemitech.net.cn

[A05] 整数除法与取模
来源：http://nx.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jz.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yp.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ul.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hd.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://ry.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://px.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://zh.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://mb.bjjhwx.cn

[A06] 字符串转数字
来源：http://ha.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://nx.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dm.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rw.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mt.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nn.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nc.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://um.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ft.shxzskj.cn

[A07] 数字转字符串
来源：http://hs.hahajie.cn

Py:   str(42)
来源：http://az.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://ll.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://iv.yuntaijiaju.cn

TS:   String(42)
来源：http://yr.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nu.szxytkj.cn

Go:   strconv.Itoa(42)
来源：http://vw.521024.cn

Ruby: 42.to_s
来源：http://ok.jianghongdianzi.cn

C#:   42.ToString()
来源：http://np.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://ck.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ua.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hr.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://by.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xt.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cp.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kh.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pm.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lk.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://ij.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jn.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ro.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jn.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ci.yuntaijiaju.cn


<!-- 参考信息 -->