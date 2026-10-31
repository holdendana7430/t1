代发 wailian999

[U47] PHP：联合类型
来源：http://vc.hnjuh.cn

int|string $id
来源：http://um.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://se.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cs.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://mr.shxzskj.cn

public readonly string $name
来源：http://ks.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://lk.9csxet.cn

public function __construct(private int $id) {}
来源：http://jq.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://el.panjiajie.cn

[$a, $b] = $arr;
来源：http://dm.szxytkj.cn

[U52] PHP：箭头函数
来源：http://yv.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://ki.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://xc.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://po.shxzskj.cn

[U54] PHP：空安全调用
来源：http://ix.huixinmuqiang.cn

$obj?->method()
来源：http://pe.shxzukj.cn

[U55] PHP：match 表达式
来源：http://xd.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://de.521024.cn

[U56] PHP：命名参数
来源：http://rq.nszjky.cn

f(a: 1, b: 2)
来源：http://iv.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://op.yuntaijiaju.cn

"值: {$a}"
来源：http://kf.shxzskj.cn

[U58] PHP：数组三件套
来源：http://qf.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fa.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://ya.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sf.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://fp.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tc.yuexingan06.cn

[U61] PHP：正则
来源：http://ii.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vl.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://cz.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ht.szxytkj.cn

[U63] PHP：文件读写
来源：http://tv.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vb.nicolike.cn

[U64] PHP：目录遍历
来源：http://kr.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://ro.asd995.cn

[U65] PHP：会话
来源：http://mz.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zz.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://rt.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pk.hahajie.cn

[U67] PHP：处理文件上传
来源：http://ze.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zm.asd995.cn

[U68] PHP：PDO 连接
来源：http://ee.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://au.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://ds.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qj.szsharing.cn

[U70] PHP：PDO 事务
来源：http://nb.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ia.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://qc.521024.cn

throw new RuntimeException("失败", 500);
来源：http://ok.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://wj.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://ec.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://me.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://hr.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://hn.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://uk.521024.cn

[U75] PHP：依赖注入
来源：http://cx.lnxyls.cn

composer require psr/container
来源：http://ij.haigaiapp.cn

[U76] PHP：简单路由
来源：http://sy.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hw.gzmigu.cn

[U77] PHP：模板渲染
来源：http://ce.newstarts.cn

composer require twig/twig
来源：http://ql.chemitech.net.cn

[U78] PHP：单元测试
来源：http://yz.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://hg.gzmigu.cn

[U79] PHP：静态分析
来源：http://hu.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://lu.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://wf.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dc.shtwfgs.cn

[U81] JS：初始化项目
来源：http://tz.haigaiapp.cn

npm init -y;  npm i express
来源：http://rr.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://ub.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ds.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://rz.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://re.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://ug.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sp.521024.cn

[U85] JS：可选链
来源：http://xx.bjjhwx.cn

a?.b?.c
来源：http://cd.szsharing.cn

[U86] JS：空值合并
来源：http://gj.jctech888.com.cn

a ?? b
来源：http://qf.jctech888.com.cn

[U87] JS：解构默认值
来源：http://xi.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://fd.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://ze.9csxet.cn

{ ...a, ...b }
来源：http://vq.nicolike.cn

[U89] JS：数组去重
来源：http://oc.nicolike.cn

[...new Set(arr)]
来源：http://ud.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://gp.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://aq.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://eu.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dh.gzmigu.cn

[U92] JS：深拷贝
来源：http://ez.jctech888.com.cn

structuredClone(obj)
来源：http://uw.colortex.cn

[U93] JS：模板字符串
来源：http://yb.yuexingan06.cn

`共 ${n} 条`
来源：http://hn.asd995.cn

[U94] JS：箭头函数
来源：http://ap.lnxyls.cn

const double = x => x * 2;
来源：http://zk.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://wl.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://fx.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://bc.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ez.asd995.cn

[U97] JS：并发请求
来源：http://ec.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://og.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://en.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ka.muxihuayi.cn

[U99] JS：事件监听
来源：http://uu.newstarts.cn

el.addEventListener("click", e => {})
来源：http://ff.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://yy.jctech888.com.cn

document.querySelector(".item")
来源：http://km.szsharing.cn

[U101] JS：classList 操作
来源：http://yi.521024.cn

el.classList.toggle("active")
来源：http://eu.521024.cn

[U102] JS：本地存储
来源：http://tm.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ug.huixiangedu.cn

[U103] JS：定时器
来源：http://ym.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bq.lnxyls.cn

[U104] JS：防抖
来源：http://mo.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zn.nicolike.cn

[U105] JS：节流
来源：http://ym.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nt.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://aj.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jo.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ih.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gt.hahajie.cn

[U108] JS：随机整数
来源：http://fs.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://te.huixiangedu.cn

[U109] JS：数组分组
来源：http://wz.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://vb.hahajie.cn

[U110] JS：数组分块
来源：http://yw.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kd.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://ah.9csxet.cn

new Map(Object.entries(obj))
来源：http://vm.gzmigu.cn

[U112] JS：字符串补位
来源：http://qz.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://nh.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://oh.hahajie.cn

s.replaceAll("a", "b")
来源：http://lo.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://cn.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://he.lnxyls.cn

[U115] JS：生成 UUID
来源：http://au.nszjky.cn

crypto.randomUUID()
来源：http://ew.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://df.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://jm.chemitech.net.cn

[U117] JS：单元测试
来源：http://hw.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://up.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://cu.huanxung.cn

npm i -D vite;  npx vite
来源：http://zd.huanxung.cn

[U119] JS：生产构建
来源：http://cm.asd995.cn

npx vite build
来源：http://sm.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://gf.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://fv.gzmigu.cn

================================================================================
来源：http://vl.nicolike.cn

统计汇总
来源：http://hd.panjiajie.cn

================================================================================
来源：http://ch.jctech888.com.cn

按语言统计（条）：
来源：http://pp.jctech888.com.cn

Python ......... 252
来源：http://nf.bookmarksfly.cn

PHP ............ 252
来源：http://sy.9csxet.cn

JavaScript ..... 252
来源：http://xx.huixinmuqiang.cn

TypeScript ..... 212
来源：http://eh.yuntaijiaju.cn

Java ........... 212
来源：http://wi.yuexingan06.cn

Go ............. 212
来源：http://gz.colortex.cn

Ruby ........... 212
来源：http://ik.muxihuayi.cn

C# ............. 212
来源：http://he.yuntaijiaju.cn

C .............. 30
来源：http://lz.chemitech.net.cn

C++ ............ 30
来源：http://rp.hahajie.cn

SQL ............ 90
来源：http://hg.521024.cn

Bash ........... 80
来源：http://bj.jctech888.com.cn

Kotlin ......... 15
来源：http://fu.yuntaijiaju.cn

Swift .......... 15
来源：http://gw.huanxung.cn

Lua ............ 10
来源：http://iy.huixinmuqiang.cn

Perl ........... 10
来源：http://ys.szsharing.cn

Scala .......... 10
来源：http://du.yuntaijiaju.cn

------------------------------------
来源：http://jx.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://pb.huixiangedu.cn

按章节统计：
来源：http://bz.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pt.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mf.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sx.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://id.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uy.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fd.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ba.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ri.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jy.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ka.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fu.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sq.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lf.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vf.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vi.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xz.colortex.cn

Q SQL 专题                              90
来源：http://un.521024.cn

R Bash 专题                             80
来源：http://dj.colortex.cn

S C / C++ 专题                          60
来源：http://zm.szsharing.cn

T 其他语言补充                          60
来源：http://rw.nszjky.cn

U 高频实用片段                         120
来源：http://kz.shtwfgs.cn

------------------------------------
来源：http://vt.hnjuh.cn

合计                                  2106 条
来源：http://oy.asd995.cn

--------------------------------------------------------------------------------
来源：http://cc.bjjhwx.cn

使用提醒
来源：http://bm.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ol.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qk.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vm.bjjhwx.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pt.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://er.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cv.9csxet.cn

—— 文件结束 ——
来源：http://xl.nszjky.cn

================================================================================
来源：http://wr.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://zc.newstarts.cn

Common Programming Examples Cheat Book
来源：http://bg.colortex.cn

================================================================================
来源：http://dy.bjjhwx.cn

【收录内容】
来源：http://ex.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oi.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ox.newstarts.cn

SQL · Bash · C · C++
来源：http://fj.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nv.bjjhwx.cn

【使用说明】
来源：http://ij.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://go.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kk.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://li.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zh.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://es.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jp.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dk.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gp.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://er.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hi.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zt.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zw.panjiajie.cn

【文件统计】
来源：http://cs.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dj.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://cs.asd995.cn

目  录
来源：http://fr.huanxung.cn

--------------------------------------------------------------------------------
来源：http://mw.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ni.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://un.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ma.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://il.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lz.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qi.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ts.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tv.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lr.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xa.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gx.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bf.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wj.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yx.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ks.jianghongdianzi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xv.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ag.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kd.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ct.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nz.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eh.hnjuh.cn

================================================================================
来源：http://qj.panjiajie.cn

A. 基础语法与类型
来源：http://hd.shxzskj.cn

================================================================================
来源：http://ey.haigaiapp.cn

[A01] Hello World
来源：http://fk.nszjky.cn

Py:   print("Hello, World!")
来源：http://xd.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://ck.521024.cn

JS:   console.log("Hello, World!");
来源：http://eo.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wd.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://eh.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://ql.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://wg.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://af.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://sj.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zc.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wr.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fz.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ni.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://xy.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://kw.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://uk.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iy.lnxyls.cn

[A03] 常量定义
来源：http://gr.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dy.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://xe.szsharing.cn

JS:   const PI = 3.14159;
来源：http://fr.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://pg.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://oi.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://vq.newstarts.cn

Ruby: PI = 3.14159
来源：http://hb.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://gl.newstarts.cn

[A04] 判断变量类型
来源：http://zp.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ya.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hq.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pz.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ib.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yc.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ik.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yy.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://ye.9csxet.cn

[A05] 整数除法与取模
来源：http://lv.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wc.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jo.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://va.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dg.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://bq.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://bh.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://yn.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://kt.jianghongdianzi.cn


<!-- 参考信息 -->