代发 wailian999

[U51] PHP：数组解构
来源：http://qn.muxihuayi.cn

[$a, $b] = $arr;
来源：http://aw.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://rj.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://vj.huanxung.cn

[U53] PHP：空合并运算符
来源：http://if.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://yh.szxytkj.cn

[U54] PHP：空安全调用
来源：http://bj.nicolike.cn

$obj?->method()
来源：http://fh.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://bm.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ae.wgjwhj.cn

[U56] PHP：命名参数
来源：http://tu.szsharing.cn

f(a: 1, b: 2)
来源：http://tx.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://jz.asd995.cn

"值: {$a}"
来源：http://tu.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://kl.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ux.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://gx.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mz.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://qm.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ti.huixinmuqiang.cn

[U61] PHP：正则
来源：http://zj.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hw.nszjky.cn

[U62] PHP：日期对象
来源：http://ly.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fy.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://ty.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yu.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://fk.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.haigaiapp.cn

[U65] PHP：会话
来源：http://wl.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ml.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://zh.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rf.asd995.cn

[U67] PHP：处理文件上传
来源：http://mq.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cm.asd995.cn

[U68] PHP：PDO 连接
来源：http://mk.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zu.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://sg.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wu.9csxet.cn

[U70] PHP：PDO 事务
来源：http://bm.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gv.asd995.cn

[U71] PHP：抛出异常
来源：http://jj.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://js.shxzukj.cn

[U72] PHP：写错误日志
来源：http://xw.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://ir.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://gj.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://wv.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://wd.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://kh.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://zn.colortex.cn

composer require psr/container
来源：http://qe.jctech888.com.cn

[U76] PHP：简单路由
来源：http://cs.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cz.asd995.cn

[U77] PHP：模板渲染
来源：http://zo.asd995.cn

composer require twig/twig
来源：http://uc.9csxet.cn

[U78] PHP：单元测试
来源：http://hs.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://kv.gzmigu.cn

[U79] PHP：静态分析
来源：http://ks.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://ve.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://cs.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eg.lnxyls.cn

[U81] JS：初始化项目
来源：http://ep.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://ja.colortex.cn

[U82] JS：package.json 脚本
来源：http://ua.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gd.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://pm.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://as.colortex.cn

[U84] JS：CommonJS 写法
来源：http://ye.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://if.lnxyls.cn

[U85] JS：可选链
来源：http://vy.hnjuh.cn

a?.b?.c
来源：http://hb.chemitech.net.cn

[U86] JS：空值合并
来源：http://hl.hnjuh.cn

a ?? b
来源：http://jm.jctech888.com.cn

[U87] JS：解构默认值
来源：http://hd.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://sx.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://da.huixiangedu.cn

{ ...a, ...b }
来源：http://zz.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://gl.haigaiapp.cn

[...new Set(arr)]
来源：http://sv.lnxyls.cn

[U90] JS：数字数组排序
来源：http://pe.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://hx.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://wq.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bt.521024.cn

[U92] JS：深拷贝
来源：http://lo.wgjwhj.cn

structuredClone(obj)
来源：http://op.chemitech.net.cn

[U93] JS：模板字符串
来源：http://sw.bookmarksfly.cn

`共 ${n} 条`
来源：http://ay.jctech888.com.cn

[U94] JS：箭头函数
来源：http://kt.521024.cn

const double = x => x * 2;
来源：http://op.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://fy.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://oi.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://nk.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ll.szsharing.cn

[U97] JS：并发请求
来源：http://eo.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oi.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://lq.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ad.bjjhwx.cn

[U99] JS：事件监听
来源：http://zc.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://ij.colortex.cn

[U100] JS：DOM 查询
来源：http://yl.jctech888.com.cn

document.querySelector(".item")
来源：http://ug.huanxung.cn

[U101] JS：classList 操作
来源：http://ct.colortex.cn

el.classList.toggle("active")
来源：http://ph.colortex.cn

[U102] JS：本地存储
来源：http://st.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nt.bookmarksfly.cn

[U103] JS：定时器
来源：http://em.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ms.panjiajie.cn

[U104] JS：防抖
来源：http://qg.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dm.shxzskj.cn

[U105] JS：节流
来源：http://lq.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://er.huixiangedu.cn

[U106] JS：日期格式化
来源：http://eu.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qs.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://nk.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vj.huixiangedu.cn

[U108] JS：随机整数
来源：http://tx.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oi.521024.cn

[U109] JS：数组分组
来源：http://cp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://vl.haigaiapp.cn

[U110] JS：数组分块
来源：http://zw.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qw.hahajie.cn

[U111] JS：对象转 Map
来源：http://xm.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://ou.lnxyls.cn

[U112] JS：字符串补位
来源：http://qr.9csxet.cn

"7".padStart(3, "0")
来源：http://qn.9csxet.cn

[U113] JS：正则替换全部
来源：http://fc.hnjuh.cn

s.replaceAll("a", "b")
来源：http://wo.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://iv.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wq.huanxung.cn

[U115] JS：生成 UUID
来源：http://yg.gzmigu.cn

crypto.randomUUID()
来源：http://nh.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://ph.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://ig.haigaiapp.cn

[U117] JS：单元测试
来源：http://em.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://vt.nicolike.cn

[U118] JS：开发服务器
来源：http://sx.szxytkj.cn

npm i -D vite;  npx vite
来源：http://ot.huanxung.cn

[U119] JS：生产构建
来源：http://vc.yuexingan06.cn

npx vite build
来源：http://nv.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://te.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://or.panjiajie.cn

================================================================================
来源：http://xa.yuntaijiaju.cn

统计汇总
来源：http://qe.yuexingan06.cn

================================================================================
来源：http://af.nszjky.cn

按语言统计（条）：
来源：http://gm.haigaiapp.cn

Python ......... 252
来源：http://jh.szsharing.cn

PHP ............ 252
来源：http://vq.huixinmuqiang.cn

JavaScript ..... 252
来源：http://lx.gzmigu.cn

TypeScript ..... 212
来源：http://au.szxytkj.cn

Java ........... 212
来源：http://lh.wgjwhj.cn

Go ............. 212
来源：http://ub.szxytkj.cn

Ruby ........... 212
来源：http://oh.yuntaijiaju.cn

C# ............. 212
来源：http://ez.bookmarksfly.cn

C .............. 30
来源：http://rh.jianghongdianzi.cn

C++ ............ 30
来源：http://yw.jctech888.com.cn

SQL ............ 90
来源：http://ml.asd995.cn

Bash ........... 80
来源：http://yw.yuntaijiaju.cn

Kotlin ......... 15
来源：http://jw.nszjky.cn

Swift .......... 15
来源：http://cy.jctech888.com.cn

Lua ............ 10
来源：http://mm.jctech888.com.cn

Perl ........... 10
来源：http://hm.chemitech.net.cn

Scala .......... 10
来源：http://id.colortex.cn

------------------------------------
来源：http://sv.yuexingan06.cn

合计 ........... 2106 条
来源：http://tm.wgjwhj.cn

按章节统计：
来源：http://zu.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zu.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mr.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xw.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jj.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xh.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://if.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sj.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hc.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mh.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yv.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fm.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nt.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://go.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tc.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mm.haigaiapp.cn

Q SQL 专题                              90
来源：http://zn.huixinmuqiang.cn

R Bash 专题                             80
来源：http://rg.haigaiapp.cn

S C / C++ 专题                          60
来源：http://lq.szxytkj.cn

T 其他语言补充                          60
来源：http://vu.bjjhwx.cn

U 高频实用片段                         120
来源：http://xq.colortex.cn

------------------------------------
来源：http://ub.muxihuayi.cn

合计                                  2106 条
来源：http://id.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://uc.asd995.cn

使用提醒
来源：http://hr.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zs.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pg.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://co.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sp.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://or.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dj.gzmigu.cn

—— 文件结束 ——
来源：http://bj.shtwfgs.cn

================================================================================
来源：http://vm.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://kn.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://yr.szsharing.cn

================================================================================
来源：http://qt.gzmigu.cn

【收录内容】
来源：http://nc.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qf.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://au.wgjwhj.cn

SQL · Bash · C · C++
来源：http://xo.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ty.colortex.cn

【使用说明】
来源：http://sq.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://st.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jg.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lj.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ki.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://td.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sk.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yd.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nk.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://un.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://js.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mf.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jg.szxytkj.cn

【文件统计】
来源：http://ev.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cm.hahajie.cn

--------------------------------------------------------------------------------
来源：http://so.shtwfgs.cn

目  录
来源：http://xs.nszjky.cn

--------------------------------------------------------------------------------
来源：http://xa.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pw.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yu.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cf.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gr.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sj.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ay.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qw.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://te.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jy.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nu.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zo.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cs.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lb.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gx.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eg.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zg.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gb.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pk.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iy.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qg.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zk.hahajie.cn

================================================================================
来源：http://wn.chemitech.net.cn

A. 基础语法与类型
来源：http://ao.jianghongdianzi.cn

================================================================================
来源：http://ra.shtwfgs.cn

[A01] Hello World
来源：http://qi.shxzskj.cn

Py:   print("Hello, World!")
来源：http://zk.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://oo.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://bp.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jo.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://ly.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://fk.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://lo.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://io.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://qv.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lb.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hg.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ks.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jb.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://of.521024.cn

Go:   name := "Alex"; age := 20
来源：http://su.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://hu.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qt.chemitech.net.cn

[A03] 常量定义
来源：http://nr.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hx.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://xi.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ln.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://bg.521024.cn

Java: static final double PI = 3.14159;
来源：http://yb.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://lt.hnjuh.cn

Ruby: PI = 3.14159
来源：http://hc.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://fu.shxzskj.cn

[A04] 判断变量类型
来源：http://ka.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bv.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hj.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bc.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://vz.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wn.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ck.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mb.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://du.yuexingan06.cn

[A05] 整数除法与取模
来源：http://wg.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://km.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gl.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qm.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wi.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://bl.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://sx.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://tt.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://bx.szxytkj.cn

[A06] 字符串转数字
来源：http://sx.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://mg.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nq.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://il.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kr.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://go.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jm.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vb.panjiajie.cn


<!-- 参考信息 -->