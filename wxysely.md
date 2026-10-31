代发 wailian999

[U53] PHP：空合并运算符
来源：http://um.521024.cn

$v = $a ?? $b ?? "default";
来源：http://to.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://wc.shxzskj.cn

$obj?->method()
来源：http://bg.521024.cn

[U55] PHP：match 表达式
来源：http://mn.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gy.chemitech.net.cn

[U56] PHP：命名参数
来源：http://mt.shxzskj.cn

f(a: 1, b: 2)
来源：http://ys.521024.cn

[U57] PHP：字符串插值
来源：http://dw.wgjwhj.cn

"值: {$a}"
来源：http://go.asd995.cn

[U58] PHP：数组三件套
来源：http://vy.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ys.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://mz.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sz.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://xc.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vy.asd995.cn

[U61] PHP：正则
来源：http://as.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xb.chemitech.net.cn

[U62] PHP：日期对象
来源：http://vm.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zh.yuexingan06.cn

[U63] PHP：文件读写
来源：http://su.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ms.hahajie.cn

[U64] PHP：目录遍历
来源：http://bz.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://of.bjjhwx.cn

[U65] PHP：会话
来源：http://mt.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://my.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://sr.jctech888.com.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sk.nszjky.cn

[U67] PHP：处理文件上传
来源：http://to.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ye.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://xe.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qm.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://sq.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ih.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://sk.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jd.szsharing.cn

[U71] PHP：抛出异常
来源：http://ex.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://ze.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://vk.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://gw.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://mw.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://lx.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://ui.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://ko.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fh.bjjhwx.cn

composer require psr/container
来源：http://tr.hnjuh.cn

[U76] PHP：简单路由
来源：http://gq.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ty.hahajie.cn

[U77] PHP：模板渲染
来源：http://mp.newstarts.cn

composer require twig/twig
来源：http://ih.wgjwhj.cn

[U78] PHP：单元测试
来源：http://gi.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://nm.chemitech.net.cn

[U79] PHP：静态分析
来源：http://fo.asd995.cn

composer require --dev phpstan/phpstan
来源：http://da.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://zh.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wt.jctech888.com.cn

[U81] JS：初始化项目
来源：http://gn.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://as.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://we.521024.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uj.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://mt.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vi.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://kp.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zi.521024.cn

[U85] JS：可选链
来源：http://xf.szxytkj.cn

a?.b?.c
来源：http://yf.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://du.szsharing.cn

a ?? b
来源：http://vu.chemitech.net.cn

[U87] JS：解构默认值
来源：http://dg.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://cg.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://rm.chemitech.net.cn

{ ...a, ...b }
来源：http://vz.muxihuayi.cn

[U89] JS：数组去重
来源：http://gy.9csxet.cn

[...new Set(arr)]
来源：http://ij.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://yx.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://bi.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://ke.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ho.gzmigu.cn

[U92] JS：深拷贝
来源：http://gw.shtwfgs.cn

structuredClone(obj)
来源：http://zq.haigaiapp.cn

[U93] JS：模板字符串
来源：http://al.chemitech.net.cn

`共 ${n} 条`
来源：http://qi.shxzskj.cn

[U94] JS：箭头函数
来源：http://sl.yuntaijiaju.cn

const double = x => x * 2;
来源：http://zi.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://hw.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://th.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://hh.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lm.muxihuayi.cn

[U97] JS：并发请求
来源：http://ij.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://zy.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ka.huixiangedu.cn

[U99] JS：事件监听
来源：http://ds.nicolike.cn

el.addEventListener("click", e => {})
来源：http://vf.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://iu.newstarts.cn

document.querySelector(".item")
来源：http://bv.jctech888.com.cn

[U101] JS：classList 操作
来源：http://ds.wgjwhj.cn

el.classList.toggle("active")
来源：http://si.gzmigu.cn

[U102] JS：本地存储
来源：http://gw.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kb.jianghongdianzi.cn

[U103] JS：定时器
来源：http://vw.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hx.szsharing.cn

[U104] JS：防抖
来源：http://ba.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wl.shxzskj.cn

[U105] JS：节流
来源：http://vg.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zl.shxzskj.cn

[U106] JS：日期格式化
来源：http://sa.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://it.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ih.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hq.hahajie.cn

[U108] JS：随机整数
来源：http://qw.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zw.chemitech.net.cn

[U109] JS：数组分组
来源：http://sf.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://ra.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://zc.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fi.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://wr.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://om.muxihuayi.cn

[U112] JS：字符串补位
来源：http://su.newstarts.cn

"7".padStart(3, "0")
来源：http://bj.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ux.hnjuh.cn

s.replaceAll("a", "b")
来源：http://kz.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://mp.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fq.9csxet.cn

[U115] JS：生成 UUID
来源：http://ug.9csxet.cn

crypto.randomUUID()
来源：http://nb.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://un.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://kk.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://st.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://ok.huixiangedu.cn

[U118] JS：开发服务器
来源：http://xe.hahajie.cn

npm i -D vite;  npx vite
来源：http://ou.colortex.cn

[U119] JS：生产构建
来源：http://jj.nszjky.cn

npx vite build
来源：http://qu.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://az.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://kp.nicolike.cn

================================================================================
来源：http://bd.chemitech.net.cn

统计汇总
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://nw.gzmigu.cn

按语言统计（条）：
来源：http://ox.jctech888.com.cn

Python ......... 252
来源：http://pp.asd995.cn

PHP ............ 252
来源：http://ei.szxytkj.cn

JavaScript ..... 252
来源：http://au.szxytkj.cn

TypeScript ..... 212
来源：http://xp.gzmigu.cn

Java ........... 212
来源：http://jl.shtwfgs.cn

Go ............. 212
来源：http://sz.asd995.cn

Ruby ........... 212
来源：http://ju.huanxung.cn

C# ............. 212
来源：http://ng.huanxung.cn

C .............. 30
来源：http://mx.shxzskj.cn

C++ ............ 30
来源：http://ap.asd995.cn

SQL ............ 90
来源：http://ab.shxzukj.cn

Bash ........... 80
来源：http://pc.muxihuayi.cn

Kotlin ......... 15
来源：http://dp.szxytkj.cn

Swift .......... 15
来源：http://re.muxihuayi.cn

Lua ............ 10
来源：http://tg.asd995.cn

Perl ........... 10
来源：http://ev.asd995.cn

Scala .......... 10
来源：http://cs.hahajie.cn

------------------------------------
来源：http://jv.hnjuh.cn

合计 ........... 2106 条
来源：http://om.huixinmuqiang.cn

按章节统计：
来源：http://oj.szsharing.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ts.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ge.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wc.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rz.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gs.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sc.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gi.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cg.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bv.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nx.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://js.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ev.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wq.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://io.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qn.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lo.shxzskj.cn

Q SQL 专题                              90
来源：http://dt.huixinmuqiang.cn

R Bash 专题                             80
来源：http://im.9csxet.cn

S C / C++ 专题                          60
来源：http://bu.shxzskj.cn

T 其他语言补充                          60
来源：http://ob.shxzskj.cn

U 高频实用片段                         120
来源：http://ik.gzmigu.cn

------------------------------------
来源：http://pw.yuexingan06.cn

合计                                  2106 条
来源：http://au.colortex.cn

--------------------------------------------------------------------------------
来源：http://wf.bookmarksfly.cn

使用提醒
来源：http://ek.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://dh.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ju.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lv.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lx.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bg.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ay.szxytkj.cn

—— 文件结束 ——
来源：http://la.hnjuh.cn

================================================================================
来源：http://ll.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://nj.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://nm.hnjuh.cn

================================================================================
来源：http://ns.jctech888.com.cn

【收录内容】
来源：http://oq.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rx.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yr.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://zs.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yg.huanxung.cn

【使用说明】
来源：http://qk.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eb.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zt.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pc.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wu.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yn.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dg.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eq.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lr.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vs.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ps.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mr.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://we.szsharing.cn

【文件统计】
来源：http://so.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ij.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://fc.panjiajie.cn

目  录
来源：http://mb.huanxung.cn

--------------------------------------------------------------------------------
来源：http://wh.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jf.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gh.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ec.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bu.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://al.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dm.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fc.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cw.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mt.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wb.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mu.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hd.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yj.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ju.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://in.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vs.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tb.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hs.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cf.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ki.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nc.bjjhwx.cn

================================================================================
来源：http://ei.hahajie.cn

A. 基础语法与类型
来源：http://ab.shxzukj.cn

================================================================================
来源：http://fd.chemitech.net.cn

[A01] Hello World
来源：http://hu.gzmigu.cn

Py:   print("Hello, World!")
来源：http://on.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://la.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://mh.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://af.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://ae.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://cs.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ax.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sp.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://tm.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tx.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xh.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ee.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gm.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://mq.521024.cn

Go:   name := "Alex"; age := 20
来源：http://zb.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://xr.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pi.bookmarksfly.cn

[A03] 常量定义
来源：http://sp.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qy.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://fn.newstarts.cn

JS:   const PI = 3.14159;
来源：http://hj.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://hi.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://xp.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ic.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://lm.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://ge.szsharing.cn

[A04] 判断变量类型
来源：http://fj.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uq.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wf.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uz.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://lp.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dj.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lh.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://me.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://fk.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://bz.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ao.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://au.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kl.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hy.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://pc.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://cy.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://pg.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://hw.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://un.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://kv.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mk.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://un.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jx.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://df.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gk.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ho.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mo.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://ln.nszjky.cn

Py:   str(42)
来源：http://uc.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://cf.szxytkj.cn


<!-- 参考信息 -->