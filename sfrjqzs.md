代发 wailian999

[U55] PHP：match 表达式
来源：http://it.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cl.bjjhwx.cn

[U56] PHP：命名参数
来源：http://bk.lnxyls.cn

f(a: 1, b: 2)
来源：http://kp.lnxyls.cn

[U57] PHP：字符串插值
来源：http://xh.yuntaijiaju.cn

"值: {$a}"
来源：http://wm.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://rq.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uf.shxzskj.cn

[U59] PHP：自定义排序
来源：http://qc.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ni.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://fh.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pe.521024.cn

[U61] PHP：正则
来源：http://nt.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dl.shtwfgs.cn

[U62] PHP：日期对象
来源：http://fx.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cz.asd995.cn

[U63] PHP：文件读写
来源：http://kd.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xq.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://jl.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://rj.hahajie.cn

[U65] PHP：会话
来源：http://lo.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://az.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://hi.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://up.521024.cn

[U67] PHP：处理文件上传
来源：http://eo.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bt.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://gq.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ay.colortex.cn

[U69] PHP：PDO 预处理
来源：http://tx.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hn.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://nq.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ly.shxzukj.cn

[U71] PHP：抛出异常
来源：http://nh.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://zo.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://ae.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ug.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://yw.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://fv.hahajie.cn

[U74] PHP：读取环境变量
来源：http://zj.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://pp.huanxung.cn

[U75] PHP：依赖注入
来源：http://oh.newstarts.cn

composer require psr/container
来源：http://xx.shxzskj.cn

[U76] PHP：简单路由
来源：http://cx.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jm.shxzskj.cn

[U77] PHP：模板渲染
来源：http://yp.wgjwhj.cn

composer require twig/twig
来源：http://so.9csxet.cn

[U78] PHP：单元测试
来源：http://hg.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://jn.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://nf.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://ja.asd995.cn

[U80] PHP：代码规范修复
来源：http://sw.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xl.nszjky.cn

[U81] JS：初始化项目
来源：http://um.huixiangedu.cn

npm init -y;  npm i express
来源：http://jz.521024.cn

[U82] JS：package.json 脚本
来源：http://dt.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bh.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://hy.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hb.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://tb.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rt.hnjuh.cn

[U85] JS：可选链
来源：http://gt.colortex.cn

a?.b?.c
来源：http://rf.jctech888.com.cn

[U86] JS：空值合并
来源：http://ii.nicolike.cn

a ?? b
来源：http://rx.panjiajie.cn

[U87] JS：解构默认值
来源：http://bq.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://li.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://jl.muxihuayi.cn

{ ...a, ...b }
来源：http://oc.shxzskj.cn

[U89] JS：数组去重
来源：http://cg.hnjuh.cn

[...new Set(arr)]
来源：http://wh.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://rq.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://cg.nszjky.cn

[U91] JS：对象键值遍历
来源：http://cj.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rl.521024.cn

[U92] JS：深拷贝
来源：http://kp.hahajie.cn

structuredClone(obj)
来源：http://ih.nicolike.cn

[U93] JS：模板字符串
来源：http://ui.nszjky.cn

`共 ${n} 条`
来源：http://zl.hnjuh.cn

[U94] JS：箭头函数
来源：http://lt.bjjhwx.cn

const double = x => x * 2;
来源：http://tp.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://nd.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://zc.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ri.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tg.chemitech.net.cn

[U97] JS：并发请求
来源：http://cr.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ri.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://yh.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uf.asd995.cn

[U99] JS：事件监听
来源：http://zs.hahajie.cn

el.addEventListener("click", e => {})
来源：http://db.shxzukj.cn

[U100] JS：DOM 查询
来源：http://wn.lnxyls.cn

document.querySelector(".item")
来源：http://wo.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://hn.nicolike.cn

el.classList.toggle("active")
来源：http://yt.hahajie.cn

[U102] JS：本地存储
来源：http://rb.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xf.panjiajie.cn

[U103] JS：定时器
来源：http://hw.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dp.hahajie.cn

[U104] JS：防抖
来源：http://rg.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://al.gzmigu.cn

[U105] JS：节流
来源：http://bx.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pn.haigaiapp.cn

[U106] JS：日期格式化
来源：http://uq.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gd.asd995.cn

[U107] JS：数字千分位
来源：http://wu.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://da.9csxet.cn

[U108] JS：随机整数
来源：http://ap.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://px.colortex.cn

[U109] JS：数组分组
来源：http://eo.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://dw.shxzukj.cn

[U110] JS：数组分块
来源：http://vp.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xj.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://at.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://yi.yuexingan06.cn

[U112] JS：字符串补位
来源：http://gd.szsharing.cn

"7".padStart(3, "0")
来源：http://gu.hahajie.cn

[U113] JS：正则替换全部
来源：http://lx.hahajie.cn

s.replaceAll("a", "b")
来源：http://ll.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://rs.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://er.newstarts.cn

[U115] JS：生成 UUID
来源：http://nx.shxzukj.cn

crypto.randomUUID()
来源：http://br.muxihuayi.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://ea.huanxung.cn

[U117] JS：单元测试
来源：http://sf.asd995.cn

npm i -D vitest;  npx vitest
来源：http://be.wgjwhj.cn

[U118] JS：开发服务器
来源：http://ie.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://ad.9csxet.cn

[U119] JS：生产构建
来源：http://wn.newstarts.cn

npx vite build
来源：http://nd.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ig.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ve.hnjuh.cn

================================================================================
来源：http://bb.jianghongdianzi.cn

统计汇总
来源：http://ox.newstarts.cn

================================================================================
来源：http://kj.panjiajie.cn

按语言统计（条）：
来源：http://jp.huanxung.cn

Python ......... 252
来源：http://yh.panjiajie.cn

PHP ............ 252
来源：http://pu.huixiangedu.cn

JavaScript ..... 252
来源：http://sg.huanxung.cn

TypeScript ..... 212
来源：http://lm.szxytkj.cn

Java ........... 212
来源：http://hb.newstarts.cn

Go ............. 212
来源：http://hy.szsharing.cn

Ruby ........... 212
来源：http://xn.panjiajie.cn

C# ............. 212
来源：http://xb.bookmarksfly.cn

C .............. 30
来源：http://cl.gzmigu.cn

C++ ............ 30
来源：http://hz.shxzskj.cn

SQL ............ 90
来源：http://bl.nszjky.cn

Bash ........... 80
来源：http://kp.nicolike.cn

Kotlin ......... 15
来源：http://lr.521024.cn

Swift .......... 15
来源：http://dz.szsharing.cn

Lua ............ 10
来源：http://rb.yuexingan06.cn

Perl ........... 10
来源：http://dp.jianghongdianzi.cn

Scala .......... 10
来源：http://eb.shxzskj.cn

------------------------------------
来源：http://ps.hahajie.cn

合计 ........... 2106 条
来源：http://ut.gzmigu.cn

按章节统计：
来源：http://ri.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sp.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gq.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://at.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mh.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ol.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://in.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vp.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rv.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uh.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xw.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://si.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ve.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ot.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ax.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nb.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cr.shxzskj.cn

Q SQL 专题                              90
来源：http://oi.newstarts.cn

R Bash 专题                             80
来源：http://hu.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://vc.nicolike.cn

T 其他语言补充                          60
来源：http://lp.huixiangedu.cn

U 高频实用片段                         120
来源：http://sd.hahajie.cn

------------------------------------
来源：http://cp.wgjwhj.cn

合计                                  2106 条
来源：http://fr.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://xm.yuexingan06.cn

使用提醒
来源：http://tt.szsharing.cn

--------------------------------------------------------------------------------
来源：http://no.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ce.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ch.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ei.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kb.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nh.panjiajie.cn

—— 文件结束 ——
来源：http://li.asd995.cn

================================================================================
来源：http://sk.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://ed.521024.cn

Common Programming Examples Cheat Book
来源：http://pu.szxytkj.cn

================================================================================
来源：http://oe.9csxet.cn

【收录内容】
来源：http://yu.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kv.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vz.521024.cn

SQL · Bash · C · C++
来源：http://cq.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hd.gzmigu.cn

【使用说明】
来源：http://el.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gg.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://st.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qa.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ch.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ch.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gq.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ya.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ai.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vh.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jd.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ea.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eh.hnjuh.cn

【文件统计】
来源：http://qb.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kz.asd995.cn

--------------------------------------------------------------------------------
来源：http://sj.shtwfgs.cn

目  录
来源：http://fg.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://vi.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mx.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yd.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lk.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nr.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ew.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jh.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pt.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gw.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pk.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wq.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ll.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://en.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rv.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sy.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qd.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ch.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qu.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ta.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nm.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wv.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xg.bookmarksfly.cn

================================================================================
来源：http://le.chemitech.net.cn

A. 基础语法与类型
来源：http://yz.asd995.cn

================================================================================
来源：http://xa.hnjuh.cn

[A01] Hello World
来源：http://pk.nszjky.cn

Py:   print("Hello, World!")
来源：http://mt.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://sj.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://fy.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ms.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://qe.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://ck.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://rq.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ya.shxzukj.cn

[A02] 变量声明与赋值
来源：http://ha.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fx.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yw.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wv.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ew.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://wz.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://rr.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://hv.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gg.jctech888.com.cn

[A03] 常量定义
来源：http://pc.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jf.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://ke.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ek.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://li.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://in.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://gs.lnxyls.cn

Ruby: PI = 3.14159
来源：http://is.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://bb.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://ur.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vv.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sm.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fa.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ut.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://at.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jd.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fv.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://nd.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://nb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ly.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ti.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ct.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jb.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://qb.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://uu.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://al.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://uo.huanxung.cn

[A06] 字符串转数字
来源：http://uj.521024.cn

Py:   int("42"); float("3.14")
来源：http://tj.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ki.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zg.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cm.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pg.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rp.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lk.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ne.panjiajie.cn

[A07] 数字转字符串
来源：http://rt.panjiajie.cn

Py:   str(42)
来源：http://fo.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://cx.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://at.yuexingan06.cn

TS:   String(42)
来源：http://zd.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://po.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://oj.jianghongdianzi.cn


<!-- 参考信息 -->