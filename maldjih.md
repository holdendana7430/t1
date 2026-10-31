代发 wailian999

[U49] PHP：只读属性
来源：http://mb.lnxyls.cn

public readonly string $name
来源：http://bh.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://nd.hnjuh.cn

public function __construct(private int $id) {}
来源：http://bf.panjiajie.cn

[U51] PHP：数组解构
来源：http://fi.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://lk.szsharing.cn

[U52] PHP：箭头函数
来源：http://dz.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://jl.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://zu.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://ue.gzmigu.cn

[U54] PHP：空安全调用
来源：http://ke.gzmigu.cn

$obj?->method()
来源：http://vw.huanxung.cn

[U55] PHP：match 表达式
来源：http://yu.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://es.chemitech.net.cn

[U56] PHP：命名参数
来源：http://zu.hnjuh.cn

f(a: 1, b: 2)
来源：http://gm.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://ub.shtwfgs.cn

"值: {$a}"
来源：http://os.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://dc.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ld.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://oo.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gw.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://pm.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rv.wgjwhj.cn

[U61] PHP：正则
来源：http://te.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oy.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://cv.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mw.szsharing.cn

[U63] PHP：文件读写
来源：http://hx.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uh.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ac.521024.cn

glob("dir/*.php");  scandir("dir");
来源：http://uj.nszjky.cn

[U65] PHP：会话
来源：http://eq.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rw.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://ad.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uy.9csxet.cn

[U67] PHP：处理文件上传
来源：http://em.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://db.521024.cn

[U68] PHP：PDO 连接
来源：http://jz.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gb.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://bz.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ht.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://vf.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cg.panjiajie.cn

[U71] PHP：抛出异常
来源：http://rp.521024.cn

throw new RuntimeException("失败", 500);
来源：http://ql.asd995.cn

[U72] PHP：写错误日志
来源：http://bf.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://zc.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://ax.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://pg.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://rn.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://yf.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://aw.yuexingan06.cn

composer require psr/container
来源：http://nr.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://bm.lnxyls.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pq.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://of.panjiajie.cn

composer require twig/twig
来源：http://cz.panjiajie.cn

[U78] PHP：单元测试
来源：http://pc.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://lg.hnjuh.cn

[U79] PHP：静态分析
来源：http://um.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://pq.szsharing.cn

[U80] PHP：代码规范修复
来源：http://bj.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ss.hnjuh.cn

[U81] JS：初始化项目
来源：http://jx.muxihuayi.cn

npm init -y;  npm i express
来源：http://gc.huanxung.cn

[U82] JS：package.json 脚本
来源：http://yc.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fk.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ld.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nf.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://xt.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bg.shxzukj.cn

[U85] JS：可选链
来源：http://ps.hahajie.cn

a?.b?.c
来源：http://mr.nszjky.cn

[U86] JS：空值合并
来源：http://bu.jianghongdianzi.cn

a ?? b
来源：http://dt.bjjhwx.cn

[U87] JS：解构默认值
来源：http://go.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://pg.521024.cn

[U88] JS：对象展开合并
来源：http://il.panjiajie.cn

{ ...a, ...b }
来源：http://eg.muxihuayi.cn

[U89] JS：数组去重
来源：http://zs.9csxet.cn

[...new Set(arr)]
来源：http://ry.asd995.cn

[U90] JS：数字数组排序
来源：http://lx.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://dc.hahajie.cn

[U91] JS：对象键值遍历
来源：http://fg.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hw.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://sh.shxzskj.cn

structuredClone(obj)
来源：http://ti.shtwfgs.cn

[U93] JS：模板字符串
来源：http://lk.hnjuh.cn

`共 ${n} 条`
来源：http://xp.chemitech.net.cn

[U94] JS：箭头函数
来源：http://vf.nszjky.cn

const double = x => x * 2;
来源：http://nb.hnjuh.cn

[U95] JS：Promise 包装
来源：http://lu.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://fg.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://kx.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sw.szsharing.cn

[U97] JS：并发请求
来源：http://cr.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://th.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://om.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dw.shxzskj.cn

[U99] JS：事件监听
来源：http://hx.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://gh.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://lv.gzmigu.cn

document.querySelector(".item")
来源：http://ii.bjjhwx.cn

[U101] JS：classList 操作
来源：http://yj.asd995.cn

el.classList.toggle("active")
来源：http://kq.bookmarksfly.cn

[U102] JS：本地存储
来源：http://zr.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xw.jctech888.com.cn

[U103] JS：定时器
来源：http://lx.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tc.hnjuh.cn

[U104] JS：防抖
来源：http://be.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.nicolike.cn

[U105] JS：节流
来源：http://rd.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mv.shtwfgs.cn

[U106] JS：日期格式化
来源：http://ry.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ng.asd995.cn

[U107] JS：数字千分位
来源：http://vm.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kp.bookmarksfly.cn

[U108] JS：随机整数
来源：http://nu.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hw.shxzukj.cn

[U109] JS：数组分组
来源：http://zf.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://xg.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://tr.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://df.lnxyls.cn

[U111] JS：对象转 Map
来源：http://md.lnxyls.cn

new Map(Object.entries(obj))
来源：http://nb.jctech888.com.cn

[U112] JS：字符串补位
来源：http://ry.haigaiapp.cn

"7".padStart(3, "0")
来源：http://ca.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://fx.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://bq.asd995.cn

[U114] JS：JSON 深比较
来源：http://ci.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dv.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://xn.jctech888.com.cn

crypto.randomUUID()
来源：http://ix.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://cs.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://qu.szsharing.cn

[U117] JS：单元测试
来源：http://eo.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://di.jctech888.com.cn

[U118] JS：开发服务器
来源：http://hi.hahajie.cn

npm i -D vite;  npx vite
来源：http://fw.asd995.cn

[U119] JS：生产构建
来源：http://xi.colortex.cn

npx vite build
来源：http://mb.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://xh.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://vl.asd995.cn

================================================================================
来源：http://do.szsharing.cn

统计汇总
来源：http://sr.bjjhwx.cn

================================================================================
来源：http://en.szsharing.cn

按语言统计（条）：
来源：http://qm.wgjwhj.cn

Python ......... 252
来源：http://jq.bookmarksfly.cn

PHP ............ 252
来源：http://qk.haigaiapp.cn

JavaScript ..... 252
来源：http://ut.9csxet.cn

TypeScript ..... 212
来源：http://kl.nszjky.cn

Java ........... 212
来源：http://no.huixinmuqiang.cn

Go ............. 212
来源：http://ad.jianghongdianzi.cn

Ruby ........... 212
来源：http://hk.nszjky.cn

C# ............. 212
来源：http://aq.yuntaijiaju.cn

C .............. 30
来源：http://ra.haigaiapp.cn

C++ ............ 30
来源：http://nq.newstarts.cn

SQL ............ 90
来源：http://re.bjjhwx.cn

Bash ........... 80
来源：http://hw.hahajie.cn

Kotlin ......... 15
来源：http://kc.huanxung.cn

Swift .......... 15
来源：http://dv.chemitech.net.cn

Lua ............ 10
来源：http://ij.jianghongdianzi.cn

Perl ........... 10
来源：http://oc.bjjhwx.cn

Scala .......... 10
来源：http://ws.colortex.cn

------------------------------------
来源：http://mj.jctech888.com.cn

合计 ........... 2106 条
来源：http://ci.jctech888.com.cn

按章节统计：
来源：http://sh.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qp.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zf.hnjuh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pz.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ft.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ns.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qe.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ki.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://od.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uy.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fj.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nm.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tf.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dy.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://la.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nm.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xp.wgjwhj.cn

Q SQL 专题                              90
来源：http://cq.jianghongdianzi.cn

R Bash 专题                             80
来源：http://mo.bjjhwx.cn

S C / C++ 专题                          60
来源：http://fv.huixiangedu.cn

T 其他语言补充                          60
来源：http://tj.muxihuayi.cn

U 高频实用片段                         120
来源：http://bh.bjjhwx.cn

------------------------------------
来源：http://ex.shxzukj.cn

合计                                  2106 条
来源：http://cz.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ao.asd995.cn

使用提醒
来源：http://ej.hahajie.cn

--------------------------------------------------------------------------------
来源：http://js.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ju.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bu.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gc.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qc.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nh.shtwfgs.cn

—— 文件结束 ——
来源：http://om.asd995.cn

================================================================================
来源：http://ya.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://bt.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://yp.newstarts.cn

================================================================================
来源：http://kq.huixiangedu.cn

【收录内容】
来源：http://ry.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://am.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kl.521024.cn

SQL · Bash · C · C++
来源：http://bb.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tc.9csxet.cn

【使用说明】
来源：http://xv.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ec.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ho.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hy.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dr.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uv.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nh.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tx.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kz.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gn.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://or.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hp.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fo.jctech888.com.cn

【文件统计】
来源：http://pq.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ky.9csxet.cn

--------------------------------------------------------------------------------
来源：http://pz.hahajie.cn

目  录
来源：http://jc.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://sy.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ll.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zv.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zs.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eh.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://op.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gr.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kn.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ee.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ut.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cb.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ri.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vc.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qt.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://et.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gc.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aq.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lb.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jf.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hf.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cy.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mo.huanxung.cn

================================================================================
来源：http://xp.newstarts.cn

A. 基础语法与类型
来源：http://nz.bjjhwx.cn

================================================================================
来源：http://fz.newstarts.cn

[A01] Hello World
来源：http://wr.szsharing.cn

Py:   print("Hello, World!")
来源：http://jn.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://lu.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://hg.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wg.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://sg.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://er.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://wz.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xx.nicolike.cn

[A02] 变量声明与赋值
来源：http://ot.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://co.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://py.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vk.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dk.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://we.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://zv.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://or.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ag.szsharing.cn

[A03] 常量定义
来源：http://bs.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tw.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://oe.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://kd.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://sy.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://tt.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://oh.panjiajie.cn

Ruby: PI = 3.14159
来源：http://do.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://mo.hahajie.cn

[A04] 判断变量类型
来源：http://hc.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uw.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uh.szsharing.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gl.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://jb.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vl.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qa.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uz.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://pv.9csxet.cn

[A05] 整数除法与取模
来源：http://zv.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mu.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fb.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qp.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vd.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://bl.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://ts.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://is.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://rc.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ta.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://bm.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dr.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fd.521024.cn


<!-- 参考信息 -->