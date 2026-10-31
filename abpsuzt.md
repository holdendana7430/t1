代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://im.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gg.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://hw.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ny.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://di.bjjhwx.cn

namespace App\Http;
来源：http://jg.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://fv.shxzukj.cn

declare(strict_types=1);
来源：http://ze.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://dq.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://la.panjiajie.cn

[U46] PHP：可空类型
来源：http://vg.yuexingan06.cn

?string $name = null
来源：http://tk.jctech888.com.cn

[U47] PHP：联合类型
来源：http://es.szsharing.cn

int|string $id
来源：http://dn.szsharing.cn

[U48] PHP：纯枚举
来源：http://tk.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cd.lnxyls.cn

[U49] PHP：只读属性
来源：http://nx.asd995.cn

public readonly string $name
来源：http://ha.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://cz.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://ae.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://mw.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://dr.huanxung.cn

[U52] PHP：箭头函数
来源：http://ir.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://ns.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://qf.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://gj.shxzskj.cn

[U54] PHP：空安全调用
来源：http://na.hahajie.cn

$obj?->method()
来源：http://wm.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://ua.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rs.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://fz.9csxet.cn

f(a: 1, b: 2)
来源：http://nh.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ho.lnxyls.cn

"值: {$a}"
来源：http://re.hahajie.cn

[U58] PHP：数组三件套
来源：http://wy.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oi.newstarts.cn

[U59] PHP：自定义排序
来源：http://mh.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.asd995.cn

[U60] PHP：JSON 编解码
来源：http://wx.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nh.hahajie.cn

[U61] PHP：正则
来源：http://py.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qy.521024.cn

[U62] PHP：日期对象
来源：http://kb.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jr.jctech888.com.cn

[U63] PHP：文件读写
来源：http://em.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bv.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://qi.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ki.panjiajie.cn

[U65] PHP：会话
来源：http://ah.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pc.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://il.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nu.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://bc.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aq.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://gq.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rs.521024.cn

[U69] PHP：PDO 预处理
来源：http://ll.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qh.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://qy.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ci.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://hn.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://dq.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://qs.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://my.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://qh.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://nw.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://mt.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://bs.nszjky.cn

[U75] PHP：依赖注入
来源：http://bl.huanxung.cn

composer require psr/container
来源：http://rs.szxytkj.cn

[U76] PHP：简单路由
来源：http://zn.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://or.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://ya.nszjky.cn

composer require twig/twig
来源：http://wy.gzmigu.cn

[U78] PHP：单元测试
来源：http://rk.asd995.cn

composer require --dev phpunit/phpunit
来源：http://mt.newstarts.cn

[U79] PHP：静态分析
来源：http://ue.colortex.cn

composer require --dev phpstan/phpstan
来源：http://wa.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://yj.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://st.gzmigu.cn

[U81] JS：初始化项目
来源：http://qg.asd995.cn

npm init -y;  npm i express
来源：http://rh.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://pp.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hh.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://wi.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ae.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://pe.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ud.bookmarksfly.cn

[U85] JS：可选链
来源：http://hx.hnjuh.cn

a?.b?.c
来源：http://cv.521024.cn

[U86] JS：空值合并
来源：http://pt.hahajie.cn

a ?? b
来源：http://vo.jctech888.com.cn

[U87] JS：解构默认值
来源：http://qe.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://al.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://xq.szxytkj.cn

{ ...a, ...b }
来源：http://tk.asd995.cn

[U89] JS：数组去重
来源：http://aa.asd995.cn

[...new Set(arr)]
来源：http://pi.shxzskj.cn

[U90] JS：数字数组排序
来源：http://zg.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://by.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://pn.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vx.521024.cn

[U92] JS：深拷贝
来源：http://kg.wgjwhj.cn

structuredClone(obj)
来源：http://xm.asd995.cn

[U93] JS：模板字符串
来源：http://gz.lnxyls.cn

`共 ${n} 条`
来源：http://vs.shxzukj.cn

[U94] JS：箭头函数
来源：http://mi.asd995.cn

const double = x => x * 2;
来源：http://gt.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://qm.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://ey.asd995.cn

[U96] JS：async/await 与异常
来源：http://px.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ul.muxihuayi.cn

[U97] JS：并发请求
来源：http://rb.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mm.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://se.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ra.panjiajie.cn

[U99] JS：事件监听
来源：http://ma.huanxung.cn

el.addEventListener("click", e => {})
来源：http://hl.nicolike.cn

[U100] JS：DOM 查询
来源：http://zk.wgjwhj.cn

document.querySelector(".item")
来源：http://gd.colortex.cn

[U101] JS：classList 操作
来源：http://pl.bookmarksfly.cn

el.classList.toggle("active")
来源：http://qw.huanxung.cn

[U102] JS：本地存储
来源：http://wi.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://md.shtwfgs.cn

[U103] JS：定时器
来源：http://os.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://di.newstarts.cn

[U104] JS：防抖
来源：http://hs.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.muxihuayi.cn

[U105] JS：节流
来源：http://il.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ej.gzmigu.cn

[U106] JS：日期格式化
来源：http://xx.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vf.shxzskj.cn

[U107] JS：数字千分位
来源：http://tq.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yv.wgjwhj.cn

[U108] JS：随机整数
来源：http://ne.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xq.colortex.cn

[U109] JS：数组分组
来源：http://hj.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://cp.shxzukj.cn

[U110] JS：数组分块
来源：http://pi.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://me.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://cd.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://lx.colortex.cn

[U112] JS：字符串补位
来源：http://ft.gzmigu.cn

"7".padStart(3, "0")
来源：http://el.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://bn.huanxung.cn

s.replaceAll("a", "b")
来源：http://wr.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://px.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tf.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://os.bjjhwx.cn

crypto.randomUUID()
来源：http://ro.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://mu.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://fc.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://fg.colortex.cn

npm i -D vitest;  npx vitest
来源：http://ap.yuexingan06.cn

[U118] JS：开发服务器
来源：http://rk.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://bx.shtwfgs.cn

[U119] JS：生产构建
来源：http://rz.gzmigu.cn

npx vite build
来源：http://fq.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rc.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://oz.panjiajie.cn

================================================================================
来源：http://af.haigaiapp.cn

统计汇总
来源：http://fz.huixiangedu.cn

================================================================================
来源：http://cx.jctech888.com.cn

按语言统计（条）：
来源：http://ft.colortex.cn

Python ......... 252
来源：http://ri.nicolike.cn

PHP ............ 252
来源：http://vf.yuexingan06.cn

JavaScript ..... 252
来源：http://ys.haigaiapp.cn

TypeScript ..... 212
来源：http://ai.huixiangedu.cn

Java ........... 212
来源：http://cc.521024.cn

Go ............. 212
来源：http://fq.shxzskj.cn

Ruby ........... 212
来源：http://kw.huanxung.cn

C# ............. 212
来源：http://rv.huixinmuqiang.cn

C .............. 30
来源：http://wq.bjjhwx.cn

C++ ............ 30
来源：http://sp.shxzskj.cn

SQL ............ 90
来源：http://ou.9csxet.cn

Bash ........... 80
来源：http://ih.wgjwhj.cn

Kotlin ......... 15
来源：http://en.asd995.cn

Swift .......... 15
来源：http://al.bjjhwx.cn

Lua ............ 10
来源：http://cu.521024.cn

Perl ........... 10
来源：http://qa.jianghongdianzi.cn

Scala .......... 10
来源：http://kr.newstarts.cn

------------------------------------
来源：http://ji.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://uf.bookmarksfly.cn

按章节统计：
来源：http://iv.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kh.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lg.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://np.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://el.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ky.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://il.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mt.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dy.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rb.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://to.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://up.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ec.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ue.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pf.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wh.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pn.huanxung.cn

Q SQL 专题                              90
来源：http://jy.jianghongdianzi.cn

R Bash 专题                             80
来源：http://tf.asd995.cn

S C / C++ 专题                          60
来源：http://sz.huixiangedu.cn

T 其他语言补充                          60
来源：http://fc.haigaiapp.cn

U 高频实用片段                         120
来源：http://yn.chemitech.net.cn

------------------------------------
来源：http://zk.bookmarksfly.cn

合计                                  2106 条
来源：http://dx.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://mq.shtwfgs.cn

使用提醒
来源：http://ar.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://xp.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qc.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ni.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qy.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mf.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qs.huixinmuqiang.cn

—— 文件结束 ——
来源：http://lv.hahajie.cn

================================================================================
来源：http://xu.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://ny.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://ww.wgjwhj.cn

================================================================================
来源：http://zs.muxihuayi.cn

【收录内容】
来源：http://ey.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iv.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zo.szxytkj.cn

SQL · Bash · C · C++
来源：http://hu.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zk.lnxyls.cn

【使用说明】
来源：http://vb.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oq.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qp.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wz.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jj.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xb.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ka.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jj.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mj.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mr.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ys.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://as.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qy.wgjwhj.cn

【文件统计】
来源：http://np.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://da.muxihuayi.cn

目  录
来源：http://xq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ir.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zj.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mq.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sc.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ef.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ha.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vb.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yi.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tk.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zj.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fv.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mn.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://er.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yr.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eq.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://up.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xg.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pz.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ny.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uw.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ft.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zc.shtwfgs.cn

================================================================================
来源：http://yx.szxytkj.cn

A. 基础语法与类型
来源：http://dx.hnjuh.cn

================================================================================
来源：http://be.huixiangedu.cn

[A01] Hello World
来源：http://ec.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://ml.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://cs.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://az.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ak.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://zh.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://ea.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://ky.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ln.gzmigu.cn

[A02] 变量声明与赋值
来源：http://cj.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zn.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cf.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zv.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://id.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://rs.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://us.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://cf.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yv.shxzskj.cn

[A03] 常量定义
来源：http://ou.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wi.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://eu.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://tc.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://sh.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://qt.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://rh.9csxet.cn

Ruby: PI = 3.14159
来源：http://kj.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ar.asd995.cn

[A04] 判断变量类型
来源：http://xb.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ox.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xu.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nz.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://ct.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ey.9csxet.cn


<!-- 参考信息 -->