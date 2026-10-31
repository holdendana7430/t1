代发 wailian999

[U51] PHP：数组解构
来源：http://cv.huanxung.cn

[$a, $b] = $arr;
来源：http://ed.gzmigu.cn

[U52] PHP：箭头函数
来源：http://sd.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://no.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://uz.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://gp.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://va.newstarts.cn

$obj?->method()
来源：http://dn.9csxet.cn

[U55] PHP：match 表达式
来源：http://ts.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://do.asd995.cn

[U56] PHP：命名参数
来源：http://pz.huanxung.cn

f(a: 1, b: 2)
来源：http://lj.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://kf.lnxyls.cn

"值: {$a}"
来源：http://he.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://zo.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pr.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://fa.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://co.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ps.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gy.muxihuayi.cn

[U61] PHP：正则
来源：http://ub.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ax.szxytkj.cn

[U62] PHP：日期对象
来源：http://xk.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hj.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://nu.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ng.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://gt.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://pw.yuntaijiaju.cn

[U65] PHP：会话
来源：http://qh.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wn.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://ae.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tb.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://hp.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xb.521024.cn

[U68] PHP：PDO 连接
来源：http://jf.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xb.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://jw.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cy.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://ym.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eg.huanxung.cn

[U71] PHP：抛出异常
来源：http://ru.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://nf.9csxet.cn

[U72] PHP：写错误日志
来源：http://ac.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://sg.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://wy.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://kl.colortex.cn

[U74] PHP：读取环境变量
来源：http://my.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://qy.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://rc.jctech888.com.cn

composer require psr/container
来源：http://iw.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ex.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cb.hnjuh.cn

[U77] PHP：模板渲染
来源：http://nw.521024.cn

composer require twig/twig
来源：http://ft.haigaiapp.cn

[U78] PHP：单元测试
来源：http://rk.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://wo.gzmigu.cn

[U79] PHP：静态分析
来源：http://qu.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://pq.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://tn.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fs.bjjhwx.cn

[U81] JS：初始化项目
来源：http://tx.wgjwhj.cn

npm init -y;  npm i express
来源：http://fm.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://xv.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bd.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://ok.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rr.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://cl.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fy.shxzukj.cn

[U85] JS：可选链
来源：http://gy.huanxung.cn

a?.b?.c
来源：http://mr.gzmigu.cn

[U86] JS：空值合并
来源：http://lx.muxihuayi.cn

a ?? b
来源：http://ns.hahajie.cn

[U87] JS：解构默认值
来源：http://xx.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://pa.gzmigu.cn

[U88] JS：对象展开合并
来源：http://nh.asd995.cn

{ ...a, ...b }
来源：http://rw.gzmigu.cn

[U89] JS：数组去重
来源：http://ui.521024.cn

[...new Set(arr)]
来源：http://om.shxzukj.cn

[U90] JS：数字数组排序
来源：http://xn.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ru.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://ib.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ve.szxytkj.cn

[U92] JS：深拷贝
来源：http://dy.hnjuh.cn

structuredClone(obj)
来源：http://px.bjjhwx.cn

[U93] JS：模板字符串
来源：http://xh.nicolike.cn

`共 ${n} 条`
来源：http://wj.jctech888.com.cn

[U94] JS：箭头函数
来源：http://dj.asd995.cn

const double = x => x * 2;
来源：http://fh.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://vg.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://up.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://tq.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xl.szxytkj.cn

[U97] JS：并发请求
来源：http://vt.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kt.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://nv.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hw.asd995.cn

[U99] JS：事件监听
来源：http://sf.9csxet.cn

el.addEventListener("click", e => {})
来源：http://gx.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://xv.huixiangedu.cn

document.querySelector(".item")
来源：http://us.gzmigu.cn

[U101] JS：classList 操作
来源：http://od.huixiangedu.cn

el.classList.toggle("active")
来源：http://zz.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ca.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fb.gzmigu.cn

[U103] JS：定时器
来源：http://cc.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ai.jianghongdianzi.cn

[U104] JS：防抖
来源：http://io.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mp.nszjky.cn

[U105] JS：节流
来源：http://lo.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ur.bjjhwx.cn

[U106] JS：日期格式化
来源：http://nx.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pn.bjjhwx.cn

[U107] JS：数字千分位
来源：http://al.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kc.nszjky.cn

[U108] JS：随机整数
来源：http://xl.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iq.hahajie.cn

[U109] JS：数组分组
来源：http://ex.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://ih.wgjwhj.cn

[U110] JS：数组分块
来源：http://wh.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ir.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://zm.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://no.521024.cn

[U112] JS：字符串补位
来源：http://pc.nszjky.cn

"7".padStart(3, "0")
来源：http://ma.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://dg.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://na.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://nr.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ci.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://ae.hnjuh.cn

crypto.randomUUID()
来源：http://lq.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://yx.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://dq.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://lb.asd995.cn

npm i -D vitest;  npx vitest
来源：http://wa.nszjky.cn

[U118] JS：开发服务器
来源：http://pr.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://je.huixiangedu.cn

[U119] JS：生产构建
来源：http://gp.haigaiapp.cn

npx vite build
来源：http://my.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ts.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://au.chemitech.net.cn

================================================================================
来源：http://uq.hnjuh.cn

统计汇总
来源：http://do.jianghongdianzi.cn

================================================================================
来源：http://vo.shxzskj.cn

按语言统计（条）：
来源：http://yq.newstarts.cn

Python ......... 252
来源：http://ff.gzmigu.cn

PHP ............ 252
来源：http://va.panjiajie.cn

JavaScript ..... 252
来源：http://ua.colortex.cn

TypeScript ..... 212
来源：http://jg.shtwfgs.cn

Java ........... 212
来源：http://ed.9csxet.cn

Go ............. 212
来源：http://zt.huanxung.cn

Ruby ........... 212
来源：http://km.shxzskj.cn

C# ............. 212
来源：http://jn.hnjuh.cn

C .............. 30
来源：http://ns.szsharing.cn

C++ ............ 30
来源：http://zh.wgjwhj.cn

SQL ............ 90
来源：http://ts.szsharing.cn

Bash ........... 80
来源：http://gi.lnxyls.cn

Kotlin ......... 15
来源：http://pf.shtwfgs.cn

Swift .......... 15
来源：http://ic.panjiajie.cn

Lua ............ 10
来源：http://sr.yuexingan06.cn

Perl ........... 10
来源：http://fs.hnjuh.cn

Scala .......... 10
来源：http://oa.jianghongdianzi.cn

------------------------------------
来源：http://gb.newstarts.cn

合计 ........... 2106 条
来源：http://oy.huixinmuqiang.cn

按章节统计：
来源：http://tg.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zn.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lv.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uu.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hw.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tu.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qn.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://us.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bi.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ax.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yr.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hu.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ca.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qm.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jp.newstarts.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gq.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cc.colortex.cn

Q SQL 专题                              90
来源：http://tt.muxihuayi.cn

R Bash 专题                             80
来源：http://qc.521024.cn

S C / C++ 专题                          60
来源：http://eu.panjiajie.cn

T 其他语言补充                          60
来源：http://df.haigaiapp.cn

U 高频实用片段                         120
来源：http://rv.yuexingan06.cn

------------------------------------
来源：http://jm.huanxung.cn

合计                                  2106 条
来源：http://wa.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://fx.9csxet.cn

使用提醒
来源：http://gt.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://tf.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jg.wgjwhj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ig.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wf.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dt.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ku.yuntaijiaju.cn

—— 文件结束 ——
来源：http://zh.colortex.cn

================================================================================
来源：http://tk.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://qo.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://oj.shxzskj.cn

【收录内容】
来源：http://pe.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fd.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zk.shxzskj.cn

SQL · Bash · C · C++
来源：http://om.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zn.hnjuh.cn

【使用说明】
来源：http://gt.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://je.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sm.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rw.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yn.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nx.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ka.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dv.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vp.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uu.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://en.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jm.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dq.shxzskj.cn

【文件统计】
来源：http://xi.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ss.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xj.gzmigu.cn

目  录
来源：http://hk.9csxet.cn

--------------------------------------------------------------------------------
来源：http://yb.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://py.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pb.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sm.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mw.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yw.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qz.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ks.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://im.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://su.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dk.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oo.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fe.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mo.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gt.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sd.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://md.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tm.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xl.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ad.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nb.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gy.lnxyls.cn

================================================================================
来源：http://vd.asd995.cn

A. 基础语法与类型
来源：http://ff.bookmarksfly.cn

================================================================================
来源：http://wi.muxihuayi.cn

[A01] Hello World
来源：http://jp.colortex.cn

Py:   print("Hello, World!")
来源：http://hl.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://ct.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://yi.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tu.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://nf.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://gs.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://cn.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lp.huanxung.cn

[A02] 变量声明与赋值
来源：http://dx.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gv.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://go.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qr.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ph.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://og.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://vd.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://gf.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gf.521024.cn

[A03] 常量定义
来源：http://vx.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jl.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://me.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://tr.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://ep.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://gd.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://gc.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://rx.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ap.newstarts.cn

[A04] 判断变量类型
来源：http://ly.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pn.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ep.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bh.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://bw.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ue.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ee.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bs.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://nk.huixiangedu.cn

[A05] 整数除法与取模
来源：http://bq.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yl.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://se.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://az.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lg.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://dv.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://rk.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ap.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://qf.jctech888.com.cn

[A06] 字符串转数字
来源：http://up.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://vu.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ny.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://if.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hg.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ix.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lt.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ey.shxzukj.cn


<!-- 参考信息 -->