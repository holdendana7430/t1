代发 wailian999

[U51] PHP：数组解构
来源：http://mt.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://ff.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://da.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://ay.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://hd.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://kd.szsharing.cn

[U54] PHP：空安全调用
来源：http://zi.shxzukj.cn

$obj?->method()
来源：http://ta.panjiajie.cn

[U55] PHP：match 表达式
来源：http://jx.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mp.huixiangedu.cn

[U56] PHP：命名参数
来源：http://mo.newstarts.cn

f(a: 1, b: 2)
来源：http://zs.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://wt.hahajie.cn

"值: {$a}"
来源：http://bn.asd995.cn

[U58] PHP：数组三件套
来源：http://vo.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nf.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://qt.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ve.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://zi.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ed.huanxung.cn

[U61] PHP：正则
来源：http://gj.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pc.hahajie.cn

[U62] PHP：日期对象
来源：http://ze.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vg.huanxung.cn

[U63] PHP：文件读写
来源：http://ie.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ux.asd995.cn

[U64] PHP：目录遍历
来源：http://bw.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://so.szxytkj.cn

[U65] PHP：会话
来源：http://xe.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://de.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://mi.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ud.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://gt.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yh.9csxet.cn

[U68] PHP：PDO 连接
来源：http://vm.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kw.haigaiapp.cn

[U69] PHP：PDO 预处理
来源：http://qw.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dl.newstarts.cn

[U70] PHP：PDO 事务
来源：http://eq.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kv.szsharing.cn

[U71] PHP：抛出异常
来源：http://bw.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://jb.hnjuh.cn

[U72] PHP：写错误日志
来源：http://pi.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://dq.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://uj.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://pt.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://of.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://kp.shxzskj.cn

[U75] PHP：依赖注入
来源：http://qa.shtwfgs.cn

composer require psr/container
来源：http://ey.colortex.cn

[U76] PHP：简单路由
来源：http://uk.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kq.gzmigu.cn

[U77] PHP：模板渲染
来源：http://bi.panjiajie.cn

composer require twig/twig
来源：http://pn.jctech888.com.cn

[U78] PHP：单元测试
来源：http://yq.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://hn.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://oz.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ls.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://xd.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iq.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://qe.gzmigu.cn

npm init -y;  npm i express
来源：http://ck.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://dh.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ym.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://eq.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cu.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://rv.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cy.panjiajie.cn

[U85] JS：可选链
来源：http://lu.nszjky.cn

a?.b?.c
来源：http://la.huixiangedu.cn

[U86] JS：空值合并
来源：http://ba.muxihuayi.cn

a ?? b
来源：http://ja.wgjwhj.cn

[U87] JS：解构默认值
来源：http://fo.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://hx.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://te.huanxung.cn

{ ...a, ...b }
来源：http://va.haigaiapp.cn

[U89] JS：数组去重
来源：http://cg.nszjky.cn

[...new Set(arr)]
来源：http://xn.9csxet.cn

[U90] JS：数字数组排序
来源：http://si.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://zg.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://on.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hf.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://ww.9csxet.cn

structuredClone(obj)
来源：http://lx.hahajie.cn

[U93] JS：模板字符串
来源：http://vw.asd995.cn

`共 ${n} 条`
来源：http://po.szsharing.cn

[U94] JS：箭头函数
来源：http://ys.yuexingan06.cn

const double = x => x * 2;
来源：http://aw.nszjky.cn

[U95] JS：Promise 包装
来源：http://fq.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://wt.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://vk.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wo.szxytkj.cn

[U97] JS：并发请求
来源：http://tj.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://xj.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dv.szxytkj.cn

[U99] JS：事件监听
来源：http://oy.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://ej.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://pa.9csxet.cn

document.querySelector(".item")
来源：http://cj.chemitech.net.cn

[U101] JS：classList 操作
来源：http://gc.szxytkj.cn

el.classList.toggle("active")
来源：http://xk.lnxyls.cn

[U102] JS：本地存储
来源：http://oq.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mw.muxihuayi.cn

[U103] JS：定时器
来源：http://fh.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ga.jctech888.com.cn

[U104] JS：防抖
来源：http://oi.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.shxzukj.cn

[U105] JS：节流
来源：http://kk.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zp.szxytkj.cn

[U106] JS：日期格式化
来源：http://cv.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://na.hahajie.cn

[U107] JS：数字千分位
来源：http://yq.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://py.colortex.cn

[U108] JS：随机整数
来源：http://zc.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gt.newstarts.cn

[U109] JS：数组分组
来源：http://pn.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://oc.chemitech.net.cn

[U110] JS：数组分块
来源：http://xj.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ph.colortex.cn

[U111] JS：对象转 Map
来源：http://vb.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ah.szsharing.cn

[U112] JS：字符串补位
来源：http://lx.jctech888.com.cn

"7".padStart(3, "0")
来源：http://zs.szxytkj.cn

[U113] JS：正则替换全部
来源：http://nk.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://ut.521024.cn

[U114] JS：JSON 深比较
来源：http://cl.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ku.newstarts.cn

[U115] JS：生成 UUID
来源：http://xr.shxzskj.cn

crypto.randomUUID()
来源：http://vl.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://tz.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ts.huanxung.cn

[U117] JS：单元测试
来源：http://ad.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://rz.haigaiapp.cn

[U118] JS：开发服务器
来源：http://eb.colortex.cn

npm i -D vite;  npx vite
来源：http://tp.gzmigu.cn

[U119] JS：生产构建
来源：http://ej.lnxyls.cn

npx vite build
来源：http://tr.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://il.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://bz.haigaiapp.cn

================================================================================
来源：http://jy.yuntaijiaju.cn

统计汇总
来源：http://am.hahajie.cn

================================================================================
来源：http://td.hahajie.cn

按语言统计（条）：
来源：http://zm.colortex.cn

Python ......... 252
来源：http://ya.9csxet.cn

PHP ............ 252
来源：http://ki.huixinmuqiang.cn

JavaScript ..... 252
来源：http://as.haigaiapp.cn

TypeScript ..... 212
来源：http://sk.jctech888.com.cn

Java ........... 212
来源：http://zx.newstarts.cn

Go ............. 212
来源：http://in.nszjky.cn

Ruby ........... 212
来源：http://gp.shxzukj.cn

C# ............. 212
来源：http://om.haigaiapp.cn

C .............. 30
来源：http://as.newstarts.cn

C++ ............ 30
来源：http://vv.shxzukj.cn

SQL ............ 90
来源：http://jb.nicolike.cn

Bash ........... 80
来源：http://ie.hnjuh.cn

Kotlin ......... 15
来源：http://vz.szsharing.cn

Swift .......... 15
来源：http://pi.bookmarksfly.cn

Lua ............ 10
来源：http://oq.nszjky.cn

Perl ........... 10
来源：http://rq.hahajie.cn

Scala .......... 10
来源：http://ie.chemitech.net.cn

------------------------------------
来源：http://hl.chemitech.net.cn

合计 ........... 2106 条
来源：http://uf.huixinmuqiang.cn

按章节统计：
来源：http://va.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uw.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mw.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ea.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fg.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qp.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jp.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gg.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yr.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ej.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://un.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mf.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://px.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nk.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://af.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xy.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pc.gzmigu.cn

Q SQL 专题                              90
来源：http://pv.shxzukj.cn

R Bash 专题                             80
来源：http://bj.hnjuh.cn

S C / C++ 专题                          60
来源：http://yg.haigaiapp.cn

T 其他语言补充                          60
来源：http://nq.yuexingan06.cn

U 高频实用片段                         120
来源：http://qc.szxytkj.cn

------------------------------------
来源：http://nk.wgjwhj.cn

合计                                  2106 条
来源：http://uh.hahajie.cn

--------------------------------------------------------------------------------
来源：http://os.yuexingan06.cn

使用提醒
来源：http://tw.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://hs.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qf.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qf.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lr.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ed.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ds.huixinmuqiang.cn

—— 文件结束 ——
来源：http://by.9csxet.cn

================================================================================
来源：http://ii.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://fr.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://ub.asd995.cn

================================================================================
来源：http://sk.chemitech.net.cn

【收录内容】
来源：http://yy.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://we.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tc.panjiajie.cn

SQL · Bash · C · C++
来源：http://qq.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iw.gzmigu.cn

【使用说明】
来源：http://so.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://um.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://et.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qb.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ov.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rv.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bm.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ej.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dx.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jo.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fy.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://he.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hm.lnxyls.cn

【文件统计】
来源：http://cj.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rm.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kg.gzmigu.cn

目  录
来源：http://og.hahajie.cn

--------------------------------------------------------------------------------
来源：http://cy.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fx.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hr.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yc.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ej.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sf.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://av.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lz.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uq.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fa.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bq.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lm.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lp.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://it.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wg.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ck.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yt.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xd.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://my.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tk.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cn.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://du.shtwfgs.cn

================================================================================
来源：http://jl.hnjuh.cn

A. 基础语法与类型
来源：http://rl.9csxet.cn

================================================================================
来源：http://ci.hahajie.cn

[A01] Hello World
来源：http://lo.521024.cn

Py:   print("Hello, World!")
来源：http://ga.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://hp.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://fb.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rv.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://cn.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://wt.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://gt.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fj.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://pb.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cy.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nb.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dg.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vs.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://di.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://tg.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://po.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ou.szsharing.cn

[A03] 常量定义
来源：http://nf.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ec.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://ej.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ik.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://mn.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://yb.521024.cn

Go:   const PI = 3.14159
来源：http://ua.nicolike.cn

Ruby: PI = 3.14159
来源：http://jb.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://cx.shxzskj.cn

[A04] 判断变量类型
来源：http://rf.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cc.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uo.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vf.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://hc.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gr.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://he.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hk.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://nz.lnxyls.cn

[A05] 整数除法与取模
来源：http://ev.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ui.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dn.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vw.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ew.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://gw.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://tg.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://kp.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://jj.gzmigu.cn

[A06] 字符串转数字
来源：http://ei.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://bu.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rk.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qb.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mf.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zk.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tg.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://um.huixinmuqiang.cn


<!-- 参考信息 -->