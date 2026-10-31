代发 wailian999

[U51] PHP：数组解构
来源：http://sx.nicolike.cn

[$a, $b] = $arr;
来源：http://cw.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://my.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://os.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://pf.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://su.nszjky.cn

[U54] PHP：空安全调用
来源：http://yw.szxytkj.cn

$obj?->method()
来源：http://lx.shxzskj.cn

[U55] PHP：match 表达式
来源：http://tx.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://la.muxihuayi.cn

[U56] PHP：命名参数
来源：http://bq.haigaiapp.cn

f(a: 1, b: 2)
来源：http://re.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://kz.panjiajie.cn

"值: {$a}"
来源：http://dw.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://zr.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://se.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://si.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qb.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://xv.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hg.jianghongdianzi.cn

[U61] PHP：正则
来源：http://xp.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mp.nicolike.cn

[U62] PHP：日期对象
来源：http://nv.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pq.521024.cn

[U63] PHP：文件读写
来源：http://cm.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://db.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://th.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://ag.szsharing.cn

[U65] PHP：会话
来源：http://wt.gzmigu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dx.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://yv.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mz.nszjky.cn

[U67] PHP：处理文件上传
来源：http://dn.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yq.asd995.cn

[U68] PHP：PDO 连接
来源：http://tg.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lh.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://yr.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wz.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://kv.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vy.hahajie.cn

[U71] PHP：抛出异常
来源：http://nx.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://pv.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://ww.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://xm.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ml.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://kb.nszjky.cn

[U74] PHP：读取环境变量
来源：http://vy.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://rl.nszjky.cn

[U75] PHP：依赖注入
来源：http://cw.haigaiapp.cn

composer require psr/container
来源：http://tp.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://aw.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xc.521024.cn

[U77] PHP：模板渲染
来源：http://ar.asd995.cn

composer require twig/twig
来源：http://yx.yuexingan06.cn

[U78] PHP：单元测试
来源：http://al.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://no.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://bb.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://zr.521024.cn

[U80] PHP：代码规范修复
来源：http://ye.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tf.huixiangedu.cn

[U81] JS：初始化项目
来源：http://sa.szxytkj.cn

npm init -y;  npm i express
来源：http://lo.szsharing.cn

[U82] JS：package.json 脚本
来源：http://bz.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sm.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://mt.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qg.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://bs.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pe.jctech888.com.cn

[U85] JS：可选链
来源：http://km.521024.cn

a?.b?.c
来源：http://fz.hahajie.cn

[U86] JS：空值合并
来源：http://hu.nszjky.cn

a ?? b
来源：http://yk.szxytkj.cn

[U87] JS：解构默认值
来源：http://mm.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ty.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://ie.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ne.shxzukj.cn

[U89] JS：数组去重
来源：http://fb.muxihuayi.cn

[...new Set(arr)]
来源：http://am.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://oj.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://ti.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://aq.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dl.bjjhwx.cn

[U92] JS：深拷贝
来源：http://fs.szsharing.cn

structuredClone(obj)
来源：http://rm.szsharing.cn

[U93] JS：模板字符串
来源：http://xn.chemitech.net.cn

`共 ${n} 条`
来源：http://mf.bjjhwx.cn

[U94] JS：箭头函数
来源：http://ob.huixiangedu.cn

const double = x => x * 2;
来源：http://hh.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://kc.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://fg.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://uf.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hg.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://ef.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oe.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://sf.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uq.wgjwhj.cn

[U99] JS：事件监听
来源：http://qe.colortex.cn

el.addEventListener("click", e => {})
来源：http://lf.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://en.shxzskj.cn

document.querySelector(".item")
来源：http://bn.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://gq.521024.cn

el.classList.toggle("active")
来源：http://ke.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ob.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oe.jctech888.com.cn

[U103] JS：定时器
来源：http://mm.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pq.yuexingan06.cn

[U104] JS：防抖
来源：http://cf.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.huixiangedu.cn

[U105] JS：节流
来源：http://fa.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gf.panjiajie.cn

[U106] JS：日期格式化
来源：http://oa.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dq.521024.cn

[U107] JS：数字千分位
来源：http://qc.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tw.panjiajie.cn

[U108] JS：随机整数
来源：http://ub.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sl.newstarts.cn

[U109] JS：数组分组
来源：http://ft.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://om.chemitech.net.cn

[U110] JS：数组分块
来源：http://zj.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ev.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://pw.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://uh.panjiajie.cn

[U112] JS：字符串补位
来源：http://om.haigaiapp.cn

"7".padStart(3, "0")
来源：http://zo.hnjuh.cn

[U113] JS：正则替换全部
来源：http://rg.asd995.cn

s.replaceAll("a", "b")
来源：http://tb.nicolike.cn

[U114] JS：JSON 深比较
来源：http://rc.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hc.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://qg.nicolike.cn

crypto.randomUUID()
来源：http://vw.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://wd.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://vh.lnxyls.cn

[U117] JS：单元测试
来源：http://wv.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://ia.shtwfgs.cn

[U118] JS：开发服务器
来源：http://hs.hnjuh.cn

npm i -D vite;  npx vite
来源：http://ts.nszjky.cn

[U119] JS：生产构建
来源：http://vu.yuexingan06.cn

npx vite build
来源：http://pb.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://cy.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://xe.9csxet.cn

================================================================================
来源：http://ft.521024.cn

统计汇总
来源：http://nj.gzmigu.cn

================================================================================
来源：http://aw.newstarts.cn

按语言统计（条）：
来源：http://av.szxytkj.cn

Python ......... 252
来源：http://tr.bookmarksfly.cn

PHP ............ 252
来源：http://de.9csxet.cn

JavaScript ..... 252
来源：http://fb.huixiangedu.cn

TypeScript ..... 212
来源：http://ts.gzmigu.cn

Java ........... 212
来源：http://cy.yuexingan06.cn

Go ............. 212
来源：http://bu.hahajie.cn

Ruby ........... 212
来源：http://jc.chemitech.net.cn

C# ............. 212
来源：http://ia.colortex.cn

C .............. 30
来源：http://da.chemitech.net.cn

C++ ............ 30
来源：http://yd.shxzskj.cn

SQL ............ 90
来源：http://dn.bjjhwx.cn

Bash ........... 80
来源：http://mw.newstarts.cn

Kotlin ......... 15
来源：http://zv.yuexingan06.cn

Swift .......... 15
来源：http://ot.colortex.cn

Lua ............ 10
来源：http://pw.asd995.cn

Perl ........... 10
来源：http://mx.huanxung.cn

Scala .......... 10
来源：http://eh.muxihuayi.cn

------------------------------------
来源：http://cy.newstarts.cn

合计 ........... 2106 条
来源：http://yi.hahajie.cn

按章节统计：
来源：http://vl.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wc.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://px.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ye.shtwfgs.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wz.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ev.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dd.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fk.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oz.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fa.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qu.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qx.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://au.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://um.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tj.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wg.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fj.huixiangedu.cn

Q SQL 专题                              90
来源：http://nr.asd995.cn

R Bash 专题                             80
来源：http://iw.hnjuh.cn

S C / C++ 专题                          60
来源：http://oo.szsharing.cn

T 其他语言补充                          60
来源：http://ha.bookmarksfly.cn

U 高频实用片段                         120
来源：http://ma.lnxyls.cn

------------------------------------
来源：http://ou.asd995.cn

合计                                  2106 条
来源：http://eo.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://tj.szsharing.cn

使用提醒
来源：http://xg.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ko.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rp.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cs.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xd.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zi.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ze.huixinmuqiang.cn

—— 文件结束 ——
来源：http://ww.huanxung.cn

================================================================================
来源：http://zh.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://wr.asd995.cn

Common Programming Examples Cheat Book
来源：http://jx.chemitech.net.cn

================================================================================
来源：http://wc.hnjuh.cn

【收录内容】
来源：http://wt.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://np.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gy.hahajie.cn

SQL · Bash · C · C++
来源：http://yw.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pz.huixiangedu.cn

【使用说明】
来源：http://pd.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uw.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wh.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mx.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fl.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qp.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jn.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vd.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gq.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cu.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://br.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tr.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ie.huixinmuqiang.cn

【文件统计】
来源：http://rn.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://my.huixiangedu.cn

目  录
来源：http://xp.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://kg.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kb.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bq.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lt.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xb.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ej.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ya.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kv.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qf.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lr.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ly.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qu.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kr.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fc.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://la.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zl.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wy.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qe.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oo.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jb.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zl.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qy.asd995.cn

================================================================================
来源：http://gd.haigaiapp.cn

A. 基础语法与类型
来源：http://gi.haigaiapp.cn

================================================================================
来源：http://ia.lnxyls.cn

[A01] Hello World
来源：http://kf.lnxyls.cn

Py:   print("Hello, World!")
来源：http://yw.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://jn.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://qe.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rj.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://ie.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://sa.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://nt.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wi.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://xc.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qq.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wp.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vh.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dt.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://cp.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://ga.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://tn.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tj.colortex.cn

[A03] 常量定义
来源：http://yw.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rt.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://ey.521024.cn

JS:   const PI = 3.14159;
来源：http://ld.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://lt.colortex.cn

Java: static final double PI = 3.14159;
来源：http://ed.colortex.cn

Go:   const PI = 3.14159
来源：http://oz.nszjky.cn

Ruby: PI = 3.14159
来源：http://cl.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://ae.bookmarksfly.cn

[A04] 判断变量类型
来源：http://kv.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cm.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xo.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://th.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://xx.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ob.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rm.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://zu.chemitech.net.cn

[A05] 整数除法与取模
来源：http://cr.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gj.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cy.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cz.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ub.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://eo.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://sf.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://iq.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://du.asd995.cn

[A06] 字符串转数字
来源：http://hf.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://hu.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bo.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pq.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ad.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mx.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eb.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dm.yuntaijiaju.cn


<!-- 参考信息 -->