代发 wailian999

[U61] PHP：正则
来源：http://mp.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xt.huixiangedu.cn

[U62] PHP：日期对象
来源：http://hp.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://np.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://ck.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ns.colortex.cn

[U64] PHP：目录遍历
来源：http://hr.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://zo.huixiangedu.cn

[U65] PHP：会话
来源：http://np.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://an.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://og.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gv.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://we.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kr.521024.cn

[U68] PHP：PDO 连接
来源：http://ys.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vg.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://hb.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rt.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://pc.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rm.szsharing.cn

[U71] PHP：抛出异常
来源：http://nw.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://zu.asd995.cn

[U72] PHP：写错误日志
来源：http://ik.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://zy.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://ih.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://wo.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://yb.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://fn.szxytkj.cn

[U75] PHP：依赖注入
来源：http://af.huixinmuqiang.cn

composer require psr/container
来源：http://kh.jctech888.com.cn

[U76] PHP：简单路由
来源：http://zm.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://um.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://xd.shxzukj.cn

composer require twig/twig
来源：http://sr.yuexingan06.cn

[U78] PHP：单元测试
来源：http://uf.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://yg.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://pr.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://aa.9csxet.cn

[U80] PHP：代码规范修复
来源：http://bi.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pf.yuexingan06.cn

[U81] JS：初始化项目
来源：http://up.huanxung.cn

npm init -y;  npm i express
来源：http://gu.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://mt.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pp.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://gy.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qs.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://fw.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vu.shxzskj.cn

[U85] JS：可选链
来源：http://ap.shxzskj.cn

a?.b?.c
来源：http://yv.lnxyls.cn

[U86] JS：空值合并
来源：http://yw.nicolike.cn

a ?? b
来源：http://lx.9csxet.cn

[U87] JS：解构默认值
来源：http://sa.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://rv.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://zs.huixinmuqiang.cn

{ ...a, ...b }
来源：http://vg.haigaiapp.cn

[U89] JS：数组去重
来源：http://cf.bookmarksfly.cn

[...new Set(arr)]
来源：http://pr.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ec.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://de.newstarts.cn

[U91] JS：对象键值遍历
来源：http://pj.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hm.wgjwhj.cn

[U92] JS：深拷贝
来源：http://qp.jianghongdianzi.cn

structuredClone(obj)
来源：http://lt.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ni.bookmarksfly.cn

`共 ${n} 条`
来源：http://eb.panjiajie.cn

[U94] JS：箭头函数
来源：http://yk.chemitech.net.cn

const double = x => x * 2;
来源：http://aj.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://iu.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ga.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://om.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oc.colortex.cn

[U97] JS：并发请求
来源：http://lo.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mg.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ge.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ut.yuexingan06.cn

[U99] JS：事件监听
来源：http://ex.colortex.cn

el.addEventListener("click", e => {})
来源：http://bm.szsharing.cn

[U100] JS：DOM 查询
来源：http://ky.bjjhwx.cn

document.querySelector(".item")
来源：http://lx.bjjhwx.cn

[U101] JS：classList 操作
来源：http://yb.yuexingan06.cn

el.classList.toggle("active")
来源：http://al.nicolike.cn

[U102] JS：本地存储
来源：http://cu.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kr.bookmarksfly.cn

[U103] JS：定时器
来源：http://ch.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rq.asd995.cn

[U104] JS：防抖
来源：http://fg.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rr.jctech888.com.cn

[U105] JS：节流
来源：http://au.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mi.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://hp.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yv.huixinmuqiang.cn

[U107] JS：数字千分位
来源：http://ji.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ii.asd995.cn

[U108] JS：随机整数
来源：http://kt.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pq.yuexingan06.cn

[U109] JS：数组分组
来源：http://ur.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://pf.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://kb.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eb.shxzskj.cn

[U111] JS：对象转 Map
来源：http://aw.9csxet.cn

new Map(Object.entries(obj))
来源：http://iu.shtwfgs.cn

[U112] JS：字符串补位
来源：http://zr.shxzukj.cn

"7".padStart(3, "0")
来源：http://dj.shxzukj.cn

[U113] JS：正则替换全部
来源：http://iz.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://yq.521024.cn

[U114] JS：JSON 深比较
来源：http://vb.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rt.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://md.jctech888.com.cn

crypto.randomUUID()
来源：http://jy.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://bg.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://fg.521024.cn

[U117] JS：单元测试
来源：http://ie.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ed.huanxung.cn

[U118] JS：开发服务器
来源：http://fm.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://dl.szsharing.cn

[U119] JS：生产构建
来源：http://kq.yuntaijiaju.cn

npx vite build
来源：http://he.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xa.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://lm.chemitech.net.cn

================================================================================
来源：http://jp.huixinmuqiang.cn

统计汇总
来源：http://zu.yuntaijiaju.cn

================================================================================
来源：http://gn.colortex.cn

按语言统计（条）：
来源：http://zs.nicolike.cn

Python ......... 252
来源：http://us.huixiangedu.cn

PHP ............ 252
来源：http://eq.bjjhwx.cn

JavaScript ..... 252
来源：http://xx.szxytkj.cn

TypeScript ..... 212
来源：http://pa.9csxet.cn

Java ........... 212
来源：http://wh.9csxet.cn

Go ............. 212
来源：http://ok.shxzskj.cn

Ruby ........... 212
来源：http://da.hahajie.cn

C# ............. 212
来源：http://wh.chemitech.net.cn

C .............. 30
来源：http://ok.shtwfgs.cn

C++ ............ 30
来源：http://xo.bjjhwx.cn

SQL ............ 90
来源：http://xi.newstarts.cn

Bash ........... 80
来源：http://fr.gzmigu.cn

Kotlin ......... 15
来源：http://se.asd995.cn

Swift .......... 15
来源：http://pw.shtwfgs.cn

Lua ............ 10
来源：http://gj.muxihuayi.cn

Perl ........... 10
来源：http://mv.gzmigu.cn

Scala .......... 10
来源：http://zu.bjjhwx.cn

------------------------------------
来源：http://pa.haigaiapp.cn

合计 ........... 2106 条
来源：http://tu.chemitech.net.cn

按章节统计：
来源：http://jj.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://un.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ox.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yx.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jh.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pc.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wn.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://be.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gd.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://in.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ul.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://si.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ty.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xb.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ps.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://db.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jz.szxytkj.cn

Q SQL 专题                              90
来源：http://kq.bjjhwx.cn

R Bash 专题                             80
来源：http://vi.hahajie.cn

S C / C++ 专题                          60
来源：http://uy.yuexingan06.cn

T 其他语言补充                          60
来源：http://us.jctech888.com.cn

U 高频实用片段                         120
来源：http://te.nszjky.cn

------------------------------------
来源：http://uh.yuntaijiaju.cn

合计                                  2106 条
来源：http://fr.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ga.huixiangedu.cn

使用提醒
来源：http://yo.szsharing.cn

--------------------------------------------------------------------------------
来源：http://oc.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ur.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ji.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wl.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://py.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ma.newstarts.cn

—— 文件结束 ——
来源：http://mz.521024.cn

================================================================================
来源：http://po.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://vs.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://nm.bookmarksfly.cn

================================================================================
来源：http://fa.asd995.cn

【收录内容】
来源：http://nf.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://de.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ai.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://ra.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://er.yuntaijiaju.cn

【使用说明】
来源：http://xu.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wl.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zv.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tf.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://if.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://id.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pq.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ie.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gk.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nc.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rz.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zj.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fm.shtwfgs.cn

【文件统计】
来源：http://vp.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kj.521024.cn

--------------------------------------------------------------------------------
来源：http://gt.gzmigu.cn

目  录
来源：http://vy.9csxet.cn

--------------------------------------------------------------------------------
来源：http://dg.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ax.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tv.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vy.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ik.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gi.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tu.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sz.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gr.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wf.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uf.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dw.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nk.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zz.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ta.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fx.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sl.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hr.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://in.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ug.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mq.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cb.huixiangedu.cn

================================================================================
来源：http://hv.muxihuayi.cn

A. 基础语法与类型
来源：http://ef.yuexingan06.cn

================================================================================
来源：http://hb.yuntaijiaju.cn

[A01] Hello World
来源：http://eh.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://hz.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://ff.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://wc.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ix.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://gk.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://yb.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://sy.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ok.nicolike.cn

[A02] 变量声明与赋值
来源：http://be.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://it.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ra.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xu.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fh.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://pw.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://fi.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://nb.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vb.gzmigu.cn

[A03] 常量定义
来源：http://iw.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nd.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://hr.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://fe.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://bj.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ej.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://zz.gzmigu.cn

Ruby: PI = 3.14159
来源：http://iz.colortex.cn

C#:   const double PI = 3.14159;
来源：http://xl.asd995.cn

[A04] 判断变量类型
来源：http://jj.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ni.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tj.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tm.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://gi.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://df.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ci.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ts.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://ec.jctech888.com.cn

[A05] 整数除法与取模
来源：http://pp.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://om.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uw.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hn.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ca.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://gg.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://vq.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://xv.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://fb.asd995.cn

[A06] 字符串转数字
来源：http://iy.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://hn.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pg.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cb.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fc.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zt.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mr.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pp.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tx.jctech888.com.cn

[A07] 数字转字符串
来源：http://nc.panjiajie.cn

Py:   str(42)
来源：http://dk.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://gd.nszjky.cn

JS:   String(42); (42).toString()
来源：http://ji.nicolike.cn

TS:   String(42)
来源：http://vh.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://st.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://yd.shxzskj.cn

Ruby: 42.to_s
来源：http://hp.shxzskj.cn

C#:   42.ToString()
来源：http://ue.hahajie.cn

[A08] 取整与四舍五入
来源：http://ef.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vb.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xa.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://va.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://st.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ep.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hi.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ao.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pb.521024.cn

[A09] 绝对值与最大最小值
来源：http://nd.hnjuh.cn


<!-- 参考信息 -->