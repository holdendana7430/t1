代发 wailian999

[U51] PHP：数组解构
来源：http://da.shxzukj.cn

[$a, $b] = $arr;
来源：http://qu.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://kt.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://qh.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://fv.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://ge.szsharing.cn

[U54] PHP：空安全调用
来源：http://pv.nicolike.cn

$obj?->method()
来源：http://ns.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://tx.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://or.colortex.cn

[U56] PHP：命名参数
来源：http://pn.yuexingan06.cn

f(a: 1, b: 2)
来源：http://wc.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ku.newstarts.cn

"值: {$a}"
来源：http://gr.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ra.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xi.shxzukj.cn

[U59] PHP：自定义排序
来源：http://gs.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vu.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://pu.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kc.jctech888.com.cn

[U61] PHP：正则
来源：http://dj.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zs.wgjwhj.cn

[U62] PHP：日期对象
来源：http://vn.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://go.9csxet.cn

[U63] PHP：文件读写
来源：http://bg.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lv.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://yb.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://qu.521024.cn

[U65] PHP：会话
来源：http://fa.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qe.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://xx.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://su.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://kh.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lr.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://nq.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://do.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://jt.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://af.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://nt.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kb.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://ks.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://dx.szxytkj.cn

[U72] PHP：写错误日志
来源：http://jn.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://lh.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://hi.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://zy.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://hi.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://dz.hahajie.cn

[U75] PHP：依赖注入
来源：http://sg.nicolike.cn

composer require psr/container
来源：http://nb.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://pi.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://od.szsharing.cn

[U77] PHP：模板渲染
来源：http://jc.huixiangedu.cn

composer require twig/twig
来源：http://ti.shtwfgs.cn

[U78] PHP：单元测试
来源：http://cs.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://iy.colortex.cn

[U79] PHP：静态分析
来源：http://sw.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://uj.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://hp.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rd.huixiangedu.cn

[U81] JS：初始化项目
来源：http://yu.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://lb.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://wp.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nx.521024.cn

[U83] JS：ES Module 导入导出
来源：http://zw.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cl.asd995.cn

[U84] JS：CommonJS 写法
来源：http://ge.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://de.panjiajie.cn

[U85] JS：可选链
来源：http://gy.jianghongdianzi.cn

a?.b?.c
来源：http://oi.hahajie.cn

[U86] JS：空值合并
来源：http://qp.521024.cn

a ?? b
来源：http://bh.szxytkj.cn

[U87] JS：解构默认值
来源：http://vi.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://of.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://zt.newstarts.cn

{ ...a, ...b }
来源：http://js.haigaiapp.cn

[U89] JS：数组去重
来源：http://hc.newstarts.cn

[...new Set(arr)]
来源：http://pu.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ah.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://aa.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://cm.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tq.hahajie.cn

[U92] JS：深拷贝
来源：http://ku.newstarts.cn

structuredClone(obj)
来源：http://ty.shxzskj.cn

[U93] JS：模板字符串
来源：http://cx.gzmigu.cn

`共 ${n} 条`
来源：http://tu.521024.cn

[U94] JS：箭头函数
来源：http://kp.shxzukj.cn

const double = x => x * 2;
来源：http://ov.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://wr.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://be.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://jq.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://my.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://hf.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://bz.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pm.newstarts.cn

[U99] JS：事件监听
来源：http://xv.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://xc.szsharing.cn

[U100] JS：DOM 查询
来源：http://oc.yuntaijiaju.cn

document.querySelector(".item")
来源：http://oc.shxzskj.cn

[U101] JS：classList 操作
来源：http://fz.chemitech.net.cn

el.classList.toggle("active")
来源：http://mt.muxihuayi.cn

[U102] JS：本地存储
来源：http://qd.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ww.gzmigu.cn

[U103] JS：定时器
来源：http://ap.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jj.nicolike.cn

[U104] JS：防抖
来源：http://dp.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jg.hahajie.cn

[U105] JS：节流
来源：http://rx.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vb.szsharing.cn

[U106] JS：日期格式化
来源：http://oc.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mm.wgjwhj.cn

[U107] JS：数字千分位
来源：http://jg.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wq.shxzukj.cn

[U108] JS：随机整数
来源：http://bd.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ok.huixiangedu.cn

[U109] JS：数组分组
来源：http://db.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://tp.bookmarksfly.cn

[U110] JS：数组分块
来源：http://eh.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wb.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://rp.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://sy.huanxung.cn

[U112] JS：字符串补位
来源：http://rl.shtwfgs.cn

"7".padStart(3, "0")
来源：http://rd.hnjuh.cn

[U113] JS：正则替换全部
来源：http://yt.9csxet.cn

s.replaceAll("a", "b")
来源：http://ym.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://ji.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://km.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://zz.asd995.cn

crypto.randomUUID()
来源：http://oq.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://sp.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://hf.hnjuh.cn

[U117] JS：单元测试
来源：http://ne.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://uq.newstarts.cn

[U118] JS：开发服务器
来源：http://ql.szsharing.cn

npm i -D vite;  npx vite
来源：http://do.521024.cn

[U119] JS：生产构建
来源：http://ph.shxzukj.cn

npx vite build
来源：http://np.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://lo.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://rx.shxzukj.cn

================================================================================
来源：http://cp.521024.cn

统计汇总
来源：http://sz.wgjwhj.cn

================================================================================
来源：http://fi.9csxet.cn

按语言统计（条）：
来源：http://xk.shtwfgs.cn

Python ......... 252
来源：http://kk.521024.cn

PHP ............ 252
来源：http://ft.newstarts.cn

JavaScript ..... 252
来源：http://rm.huixinmuqiang.cn

TypeScript ..... 212
来源：http://cs.newstarts.cn

Java ........... 212
来源：http://td.lnxyls.cn

Go ............. 212
来源：http://lh.9csxet.cn

Ruby ........... 212
来源：http://gr.bookmarksfly.cn

C# ............. 212
来源：http://bm.521024.cn

C .............. 30
来源：http://ny.colortex.cn

C++ ............ 30
来源：http://vn.wgjwhj.cn

SQL ............ 90
来源：http://kv.521024.cn

Bash ........... 80
来源：http://ki.haigaiapp.cn

Kotlin ......... 15
来源：http://zg.panjiajie.cn

Swift .......... 15
来源：http://hf.jctech888.com.cn

Lua ............ 10
来源：http://in.yuntaijiaju.cn

Perl ........... 10
来源：http://ma.nicolike.cn

Scala .......... 10
来源：http://km.nszjky.cn

------------------------------------
来源：http://rm.bookmarksfly.cn

合计 ........... 2106 条
来源：http://ol.chemitech.net.cn

按章节统计：
来源：http://to.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kk.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hv.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://og.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sr.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rz.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ft.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zk.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yd.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sm.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gr.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vj.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vg.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rw.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ly.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dd.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lv.huanxung.cn

Q SQL 专题                              90
来源：http://jc.huixiangedu.cn

R Bash 专题                             80
来源：http://fi.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://lr.huixiangedu.cn

T 其他语言补充                          60
来源：http://wp.nicolike.cn

U 高频实用片段                         120
来源：http://ug.hnjuh.cn

------------------------------------
来源：http://xx.gzmigu.cn

合计                                  2106 条
来源：http://pl.colortex.cn

--------------------------------------------------------------------------------
来源：http://og.huixinmuqiang.cn

使用提醒
来源：http://po.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://lm.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fg.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dt.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gv.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bb.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wz.huanxung.cn

—— 文件结束 ——
来源：http://lc.haigaiapp.cn

================================================================================
来源：http://pz.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://ew.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://jh.huixiangedu.cn

================================================================================
来源：http://ul.521024.cn

【收录内容】
来源：http://on.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ee.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://um.jctech888.com.cn

SQL · Bash · C · C++
来源：http://qm.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ch.shtwfgs.cn

【使用说明】
来源：http://fr.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://as.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ui.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pa.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pv.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ti.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zy.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sv.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bk.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dg.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dh.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://en.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vr.chemitech.net.cn

【文件统计】
来源：http://ig.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vp.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://nx.shxzukj.cn

目  录
来源：http://la.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://fr.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wx.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sv.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mt.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gd.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sl.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ki.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bf.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xb.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ro.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jz.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ch.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qz.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zw.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hv.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ii.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ch.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://te.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xl.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sg.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kf.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://va.bjjhwx.cn

================================================================================
来源：http://bi.chemitech.net.cn

A. 基础语法与类型
来源：http://se.bjjhwx.cn

================================================================================
来源：http://ca.yuntaijiaju.cn

[A01] Hello World
来源：http://no.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://bh.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://zo.asd995.cn

JS:   console.log("Hello, World!");
来源：http://tv.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yd.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://qp.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://vj.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ez.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lt.hahajie.cn

[A02] 变量声明与赋值
来源：http://cr.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kl.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ao.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://an.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jb.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://rd.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://kg.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://hq.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fs.yuexingan06.cn

[A03] 常量定义
来源：http://ob.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ss.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://mt.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://nv.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://sk.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://yn.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://cr.colortex.cn

Ruby: PI = 3.14159
来源：http://bj.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://dm.newstarts.cn

[A04] 判断变量类型
来源：http://gq.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dz.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ky.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hp.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://og.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tt.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bm.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cu.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://ui.nicolike.cn

[A05] 整数除法与取模
来源：http://ka.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cd.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://of.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kn.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ti.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://el.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://fy.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://en.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://gy.nszjky.cn

[A06] 字符串转数字
来源：http://bj.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://rc.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ip.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gu.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mp.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nn.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lw.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zc.szxytkj.cn


<!-- 参考信息 -->