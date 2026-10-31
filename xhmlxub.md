代发 wailian999

[U49] PHP：只读属性
来源：http://wp.gzmigu.cn

public readonly string $name
来源：http://ma.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://iw.shxzskj.cn

public function __construct(private int $id) {}
来源：http://wd.9csxet.cn

[U51] PHP：数组解构
来源：http://lt.nicolike.cn

[$a, $b] = $arr;
来源：http://tn.szxytkj.cn

[U52] PHP：箭头函数
来源：http://oa.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://qt.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://uz.521024.cn

$v = $a ?? $b ?? "default";
来源：http://kn.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://oz.shxzskj.cn

$obj?->method()
来源：http://jh.huanxung.cn

[U55] PHP：match 表达式
来源：http://cx.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zv.9csxet.cn

[U56] PHP：命名参数
来源：http://ik.panjiajie.cn

f(a: 1, b: 2)
来源：http://yr.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://ks.haigaiapp.cn

"值: {$a}"
来源：http://wb.nicolike.cn

[U58] PHP：数组三件套
来源：http://il.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ty.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://ir.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://ky.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jy.huixinmuqiang.cn

[U61] PHP：正则
来源：http://bg.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bs.gzmigu.cn

[U62] PHP：日期对象
来源：http://jy.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xo.hnjuh.cn

[U63] PHP：文件读写
来源：http://qd.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mi.lnxyls.cn

[U64] PHP：目录遍历
来源：http://ad.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://nv.szsharing.cn

[U65] PHP：会话
来源：http://vk.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ck.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://eg.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://es.newstarts.cn

[U67] PHP：处理文件上传
来源：http://sc.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://du.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://gb.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zs.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://fe.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yd.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://jq.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qb.newstarts.cn

[U71] PHP：抛出异常
来源：http://vs.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://rc.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://uk.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://hm.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://wr.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://tk.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://mp.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://qh.shxzukj.cn

[U75] PHP：依赖注入
来源：http://nt.szxytkj.cn

composer require psr/container
来源：http://mf.szsharing.cn

[U76] PHP：简单路由
来源：http://ge.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ob.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://lk.nicolike.cn

composer require twig/twig
来源：http://kq.szsharing.cn

[U78] PHP：单元测试
来源：http://ry.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://qp.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://nz.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://py.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://fb.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dh.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://qe.huanxung.cn

npm init -y;  npm i express
来源：http://mx.colortex.cn

[U82] JS：package.json 脚本
来源：http://dw.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qe.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ei.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jb.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://rp.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://am.gzmigu.cn

[U85] JS：可选链
来源：http://gs.lnxyls.cn

a?.b?.c
来源：http://mr.muxihuayi.cn

[U86] JS：空值合并
来源：http://uh.bjjhwx.cn

a ?? b
来源：http://ba.yuexingan06.cn

[U87] JS：解构默认值
来源：http://tu.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://tp.hnjuh.cn

[U88] JS：对象展开合并
来源：http://wm.hnjuh.cn

{ ...a, ...b }
来源：http://ua.haigaiapp.cn

[U89] JS：数组去重
来源：http://lo.newstarts.cn

[...new Set(arr)]
来源：http://nc.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ft.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://ah.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://bj.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uz.szsharing.cn

[U92] JS：深拷贝
来源：http://kw.gzmigu.cn

structuredClone(obj)
来源：http://yt.9csxet.cn

[U93] JS：模板字符串
来源：http://zl.jianghongdianzi.cn

`共 ${n} 条`
来源：http://ae.huixiangedu.cn

[U94] JS：箭头函数
来源：http://iu.wgjwhj.cn

const double = x => x * 2;
来源：http://fd.nicolike.cn

[U95] JS：Promise 包装
来源：http://oh.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://tz.hahajie.cn

[U96] JS：async/await 与异常
来源：http://cz.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vp.yuexingan06.cn

[U97] JS：并发请求
来源：http://wh.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://im.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://wc.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cg.lnxyls.cn

[U99] JS：事件监听
来源：http://pq.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://qm.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://hq.nszjky.cn

document.querySelector(".item")
来源：http://rs.9csxet.cn

[U101] JS：classList 操作
来源：http://co.521024.cn

el.classList.toggle("active")
来源：http://nl.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://qk.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ez.nicolike.cn

[U103] JS：定时器
来源：http://ii.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sy.521024.cn

[U104] JS：防抖
来源：http://qe.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ic.szxytkj.cn

[U105] JS：节流
来源：http://qg.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://am.szxytkj.cn

[U106] JS：日期格式化
来源：http://hr.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hu.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ot.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fh.yuexingan06.cn

[U108] JS：随机整数
来源：http://ba.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uh.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://zj.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://hx.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://fz.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mo.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://wg.hahajie.cn

new Map(Object.entries(obj))
来源：http://md.hahajie.cn

[U112] JS：字符串补位
来源：http://te.521024.cn

"7".padStart(3, "0")
来源：http://rg.szsharing.cn

[U113] JS：正则替换全部
来源：http://ub.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://re.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://lc.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fw.asd995.cn

[U115] JS：生成 UUID
来源：http://ou.521024.cn

crypto.randomUUID()
来源：http://yq.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://cj.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://up.chemitech.net.cn

[U117] JS：单元测试
来源：http://hs.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://eg.hnjuh.cn

[U118] JS：开发服务器
来源：http://te.panjiajie.cn

npm i -D vite;  npx vite
来源：http://fr.asd995.cn

[U119] JS：生产构建
来源：http://et.yuntaijiaju.cn

npx vite build
来源：http://lb.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://cd.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://lq.521024.cn

================================================================================
来源：http://hl.hnjuh.cn

统计汇总
来源：http://vk.szxytkj.cn

================================================================================
来源：http://sp.521024.cn

按语言统计（条）：
来源：http://yu.szxytkj.cn

Python ......... 252
来源：http://nq.yuexingan06.cn

PHP ............ 252
来源：http://wa.wgjwhj.cn

JavaScript ..... 252
来源：http://in.nicolike.cn

TypeScript ..... 212
来源：http://he.wgjwhj.cn

Java ........... 212
来源：http://ox.nicolike.cn

Go ............. 212
来源：http://pg.newstarts.cn

Ruby ........... 212
来源：http://gr.huixiangedu.cn

C# ............. 212
来源：http://tk.hnjuh.cn

C .............. 30
来源：http://as.asd995.cn

C++ ............ 30
来源：http://eg.yuntaijiaju.cn

SQL ............ 90
来源：http://of.bjjhwx.cn

Bash ........... 80
来源：http://nz.yuntaijiaju.cn

Kotlin ......... 15
来源：http://xe.hahajie.cn

Swift .......... 15
来源：http://kd.wgjwhj.cn

Lua ............ 10
来源：http://nf.huixinmuqiang.cn

Perl ........... 10
来源：http://ob.bjjhwx.cn

Scala .......... 10
来源：http://dt.shxzskj.cn

------------------------------------
来源：http://on.nicolike.cn

合计 ........... 2106 条
来源：http://wk.nicolike.cn

按章节统计：
来源：http://rf.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yk.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fd.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gd.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vx.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hh.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yt.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vz.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qi.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://et.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hi.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gz.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nh.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kt.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jx.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jp.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vk.wgjwhj.cn

Q SQL 专题                              90
来源：http://ft.bookmarksfly.cn

R Bash 专题                             80
来源：http://bb.wgjwhj.cn

S C / C++ 专题                          60
来源：http://qx.gzmigu.cn

T 其他语言补充                          60
来源：http://br.hnjuh.cn

U 高频实用片段                         120
来源：http://sy.asd995.cn

------------------------------------
来源：http://xi.9csxet.cn

合计                                  2106 条
来源：http://bz.szsharing.cn

--------------------------------------------------------------------------------
来源：http://gk.yuexingan06.cn

使用提醒
来源：http://ib.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://rm.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ru.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kk.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tp.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eo.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://we.newstarts.cn

—— 文件结束 ——
来源：http://xc.gzmigu.cn

================================================================================
来源：http://wy.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://pu.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://xq.nszjky.cn

================================================================================
来源：http://th.gzmigu.cn

【收录内容】
来源：http://wp.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xc.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zk.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://jx.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ub.huanxung.cn

【使用说明】
来源：http://cr.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://si.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fx.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eb.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wl.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wl.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://in.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xw.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sl.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cg.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bs.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://of.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hq.huixiangedu.cn

【文件统计】
来源：http://ps.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qu.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://dg.lnxyls.cn

目  录
来源：http://mm.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://yu.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lr.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qs.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cj.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hu.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zj.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gz.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rj.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aj.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ye.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yi.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hk.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xd.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mx.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dn.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ez.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wk.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bj.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yh.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bq.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lx.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tc.521024.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

A. 基础语法与类型
来源：http://rr.bookmarksfly.cn

================================================================================
来源：http://aq.wgjwhj.cn

[A01] Hello World
来源：http://ez.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://no.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://sn.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://rz.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jh.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://jm.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://hn.colortex.cn

Ruby: puts "Hello, World!"
来源：http://is.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qn.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://zi.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vi.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://md.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iq.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jh.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://yr.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://ni.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://xv.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rp.haigaiapp.cn

[A03] 常量定义
来源：http://fk.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ag.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://im.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://ve.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://fp.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://bx.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://yl.nicolike.cn

Ruby: PI = 3.14159
来源：http://ec.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://ym.bjjhwx.cn

[A04] 判断变量类型
来源：http://jx.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yn.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bw.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lb.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://vo.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sz.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ok.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vh.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://yv.asd995.cn

[A05] 整数除法与取模
来源：http://ww.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fp.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mf.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pq.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wv.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://ii.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://vr.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://xk.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ok.gzmigu.cn

[A06] 字符串转数字
来源：http://sg.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://lp.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ef.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nv.szxytkj.cn


<!-- 参考信息 -->