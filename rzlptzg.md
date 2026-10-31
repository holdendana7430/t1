代发 wailian999

[U55] PHP：match 表达式
来源：http://qi.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gi.muxihuayi.cn

[U56] PHP：命名参数
来源：http://wv.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://nu.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ob.hnjuh.cn

"值: {$a}"
来源：http://cy.huanxung.cn

[U58] PHP：数组三件套
来源：http://ou.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fn.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://pm.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xg.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://hy.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eu.haigaiapp.cn

[U61] PHP：正则
来源：http://be.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pk.nicolike.cn

[U62] PHP：日期对象
来源：http://vx.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qp.muxihuayi.cn

[U63] PHP：文件读写
来源：http://sz.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ik.newstarts.cn

[U64] PHP：目录遍历
来源：http://ai.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://cf.newstarts.cn

[U65] PHP：会话
来源：http://vb.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://io.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ks.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ds.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://bv.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rp.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://vv.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bv.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://fi.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yj.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://kf.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lo.shxzskj.cn

[U71] PHP：抛出异常
来源：http://ej.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://yz.hnjuh.cn

[U72] PHP：写错误日志
来源：http://bv.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ls.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://nc.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://ry.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://nu.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://jx.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://bl.nicolike.cn

composer require psr/container
来源：http://wq.wgjwhj.cn

[U76] PHP：简单路由
来源：http://ch.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qn.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://lh.szsharing.cn

composer require twig/twig
来源：http://re.colortex.cn

[U78] PHP：单元测试
来源：http://oy.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://eg.huixiangedu.cn

[U79] PHP：静态分析
来源：http://ab.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://vx.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://lu.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qf.wgjwhj.cn

[U81] JS：初始化项目
来源：http://um.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://kx.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://kw.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oa.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://ch.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qw.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://bo.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eq.521024.cn

[U85] JS：可选链
来源：http://sf.jctech888.com.cn

a?.b?.c
来源：http://qa.521024.cn

[U86] JS：空值合并
来源：http://fg.szsharing.cn

a ?? b
来源：http://ke.colortex.cn

[U87] JS：解构默认值
来源：http://wa.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://zv.gzmigu.cn

[U88] JS：对象展开合并
来源：http://ji.hahajie.cn

{ ...a, ...b }
来源：http://ma.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://uq.shxzukj.cn

[...new Set(arr)]
来源：http://bs.521024.cn

[U90] JS：数字数组排序
来源：http://jb.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://hi.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://ie.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sb.chemitech.net.cn

[U92] JS：深拷贝
来源：http://pm.wgjwhj.cn

structuredClone(obj)
来源：http://wg.wgjwhj.cn

[U93] JS：模板字符串
来源：http://qm.hnjuh.cn

`共 ${n} 条`
来源：http://au.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://nx.lnxyls.cn

const double = x => x * 2;
来源：http://ik.gzmigu.cn

[U95] JS：Promise 包装
来源：http://ew.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://zg.521024.cn

[U96] JS：async/await 与异常
来源：http://pz.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ng.panjiajie.cn

[U97] JS：并发请求
来源：http://ue.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://nu.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wj.huanxung.cn

[U99] JS：事件监听
来源：http://zr.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://ml.huanxung.cn

[U100] JS：DOM 查询
来源：http://yl.colortex.cn

document.querySelector(".item")
来源：http://ac.wgjwhj.cn

[U101] JS：classList 操作
来源：http://bw.huanxung.cn

el.classList.toggle("active")
来源：http://lz.shxzskj.cn

[U102] JS：本地存储
来源：http://qy.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://db.yuntaijiaju.cn

[U103] JS：定时器
来源：http://lw.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cx.9csxet.cn

[U104] JS：防抖
来源：http://yb.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vb.shtwfgs.cn

[U105] JS：节流
来源：http://nf.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ni.hahajie.cn

[U106] JS：日期格式化
来源：http://mp.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://um.gzmigu.cn

[U107] JS：数字千分位
来源：http://nc.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nf.newstarts.cn

[U108] JS：随机整数
来源：http://cf.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ho.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://ul.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://ys.gzmigu.cn

[U110] JS：数组分块
来源：http://yu.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lo.shxzskj.cn

[U111] JS：对象转 Map
来源：http://tr.gzmigu.cn

new Map(Object.entries(obj))
来源：http://dv.newstarts.cn

[U112] JS：字符串补位
来源：http://rx.lnxyls.cn

"7".padStart(3, "0")
来源：http://xo.hnjuh.cn

[U113] JS：正则替换全部
来源：http://ye.521024.cn

s.replaceAll("a", "b")
来源：http://dt.huanxung.cn

[U114] JS：JSON 深比较
来源：http://mq.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yc.szsharing.cn

[U115] JS：生成 UUID
来源：http://dz.nicolike.cn

crypto.randomUUID()
来源：http://zo.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://oe.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://br.jctech888.com.cn

[U117] JS：单元测试
来源：http://eo.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://gf.yuexingan06.cn

[U118] JS：开发服务器
来源：http://lp.szsharing.cn

npm i -D vite;  npx vite
来源：http://rp.9csxet.cn

[U119] JS：生产构建
来源：http://sb.huixinmuqiang.cn

npx vite build
来源：http://cu.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://dj.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://kd.shtwfgs.cn

================================================================================
来源：http://dx.yuexingan06.cn

统计汇总
来源：http://at.bookmarksfly.cn

================================================================================
来源：http://by.nicolike.cn

按语言统计（条）：
来源：http://lz.shtwfgs.cn

Python ......... 252
来源：http://qy.shxzukj.cn

PHP ............ 252
来源：http://fp.shxzukj.cn

JavaScript ..... 252
来源：http://ef.panjiajie.cn

TypeScript ..... 212
来源：http://ri.szxytkj.cn

Java ........... 212
来源：http://uq.shxzukj.cn

Go ............. 212
来源：http://ha.muxihuayi.cn

Ruby ........... 212
来源：http://os.nicolike.cn

C# ............. 212
来源：http://sf.hnjuh.cn

C .............. 30
来源：http://di.huixiangedu.cn

C++ ............ 30
来源：http://fd.gzmigu.cn

SQL ............ 90
来源：http://nk.lnxyls.cn

Bash ........... 80
来源：http://ya.wgjwhj.cn

Kotlin ......... 15
来源：http://gi.yuexingan06.cn

Swift .......... 15
来源：http://na.huixiangedu.cn

Lua ............ 10
来源：http://zd.yuntaijiaju.cn

Perl ........... 10
来源：http://gb.bookmarksfly.cn

Scala .......... 10
来源：http://ka.huixiangedu.cn

------------------------------------
来源：http://vz.muxihuayi.cn

合计 ........... 2106 条
来源：http://ic.wgjwhj.cn

按章节统计：
来源：http://rr.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ox.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://be.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://em.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sa.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ym.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qs.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ao.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vz.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kh.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kz.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eo.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yc.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ki.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nx.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mr.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://qi.nicolike.cn

R Bash 专题                             80
来源：http://iq.chemitech.net.cn

S C / C++ 专题                          60
来源：http://ja.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://eh.hnjuh.cn

U 高频实用片段                         120
来源：http://ew.shxzukj.cn

------------------------------------
来源：http://zu.shxzskj.cn

合计                                  2106 条
来源：http://jo.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://gr.newstarts.cn

使用提醒
来源：http://ku.nszjky.cn

--------------------------------------------------------------------------------
来源：http://vf.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sv.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sv.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cc.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yd.newstarts.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jv.jctech888.com.cn

—— 文件结束 ——
来源：http://so.lnxyls.cn

================================================================================
来源：http://mb.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://uh.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://xq.jianghongdianzi.cn

================================================================================
来源：http://gf.lnxyls.cn

【收录内容】
来源：http://gr.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bx.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://si.lnxyls.cn

SQL · Bash · C · C++
来源：http://px.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wl.gzmigu.cn

【使用说明】
来源：http://cs.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ka.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wz.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yv.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ub.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qd.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vm.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tx.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ze.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cl.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gs.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bx.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yn.huanxung.cn

【文件统计】
来源：http://ir.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nb.9csxet.cn

--------------------------------------------------------------------------------
来源：http://mb.haigaiapp.cn

目  录
来源：http://in.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://am.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ho.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rk.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wf.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gh.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fb.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ss.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kb.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sr.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ez.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dg.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kn.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xl.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pm.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fl.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eb.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://op.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zh.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ry.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fv.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fy.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kd.huanxung.cn

================================================================================
来源：http://tg.newstarts.cn

A. 基础语法与类型
来源：http://qn.huixiangedu.cn

================================================================================
来源：http://qx.521024.cn

[A01] Hello World
来源：http://st.521024.cn

Py:   print("Hello, World!")
来源：http://bz.asd995.cn

PHP:  echo "Hello, World!";
来源：http://wt.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://bf.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nk.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://zj.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://oj.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://sm.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uh.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://lc.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wb.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ux.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qm.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jy.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://hp.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://qt.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://kd.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ut.newstarts.cn

[A03] 常量定义
来源：http://dh.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dc.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://qr.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://pn.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://xf.521024.cn

Java: static final double PI = 3.14159;
来源：http://qk.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://tp.huanxung.cn

Ruby: PI = 3.14159
来源：http://ki.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://wv.hnjuh.cn

[A04] 判断变量类型
来源：http://uw.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qy.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nd.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ua.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://ni.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://az.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ve.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ci.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://wd.asd995.cn

[A05] 整数除法与取模
来源：http://og.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://da.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yn.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://je.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vn.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://ck.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://wo.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ra.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://fu.nszjky.cn

[A06] 字符串转数字
来源：http://ou.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://rw.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dt.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rj.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mz.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://am.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gw.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fx.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wa.haigaiapp.cn

[A07] 数字转字符串
来源：http://re.asd995.cn

Py:   str(42)
来源：http://jt.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://vg.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://xu.muxihuayi.cn

TS:   String(42)
来源：http://vn.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://je.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://oq.panjiajie.cn


<!-- 参考信息 -->