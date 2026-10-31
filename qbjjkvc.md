代发 wailian999

[U43] PHP：声明命名空间
来源：http://mo.shxzskj.cn

namespace App\Http;
来源：http://zc.nszjky.cn

[U44] PHP：开启严格类型
来源：http://kq.hahajie.cn

declare(strict_types=1);
来源：http://at.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://wv.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.shxzskj.cn

[U46] PHP：可空类型
来源：http://mk.9csxet.cn

?string $name = null
来源：http://od.nicolike.cn

[U47] PHP：联合类型
来源：http://wp.bookmarksfly.cn

int|string $id
来源：http://se.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://gc.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ow.gzmigu.cn

[U49] PHP：只读属性
来源：http://ek.gzmigu.cn

public readonly string $name
来源：http://dj.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://sf.asd995.cn

public function __construct(private int $id) {}
来源：http://dy.panjiajie.cn

[U51] PHP：数组解构
来源：http://mr.shxzskj.cn

[$a, $b] = $arr;
来源：http://es.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://zq.521024.cn

$double = fn($x) => $x * 2;
来源：http://yr.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://qh.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://eh.nszjky.cn

[U54] PHP：空安全调用
来源：http://bd.yuntaijiaju.cn

$obj?->method()
来源：http://jk.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://kv.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://up.huanxung.cn

[U56] PHP：命名参数
来源：http://qt.hahajie.cn

f(a: 1, b: 2)
来源：http://pd.hahajie.cn

[U57] PHP：字符串插值
来源：http://tx.nszjky.cn

"值: {$a}"
来源：http://ui.szsharing.cn

[U58] PHP：数组三件套
来源：http://fd.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oi.gzmigu.cn

[U59] PHP：自定义排序
来源：http://cm.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fs.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://ah.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kg.gzmigu.cn

[U61] PHP：正则
来源：http://zl.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mb.shxzskj.cn

[U62] PHP：日期对象
来源：http://jk.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ul.newstarts.cn

[U63] PHP：文件读写
来源：http://od.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dx.nicolike.cn

[U64] PHP：目录遍历
来源：http://og.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://sr.gzmigu.cn

[U65] PHP：会话
来源：http://zu.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ab.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://uu.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xp.huanxung.cn

[U67] PHP：处理文件上传
来源：http://nu.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ii.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://nl.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mv.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://iv.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rt.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://hv.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tp.szxytkj.cn

[U71] PHP：抛出异常
来源：http://cs.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://up.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://kv.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://zv.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://ni.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://hs.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://sd.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://oi.colortex.cn

[U75] PHP：依赖注入
来源：http://lo.521024.cn

composer require psr/container
来源：http://eb.huanxung.cn

[U76] PHP：简单路由
来源：http://ma.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wc.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://qu.lnxyls.cn

composer require twig/twig
来源：http://ze.jctech888.com.cn

[U78] PHP：单元测试
来源：http://or.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://gk.9csxet.cn

[U79] PHP：静态分析
来源：http://oa.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://et.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://me.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gd.muxihuayi.cn

[U81] JS：初始化项目
来源：http://ie.bjjhwx.cn

npm init -y;  npm i express
来源：http://rr.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://wa.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ti.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://xs.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://md.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://ce.yuntaijiaju.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rr.szxytkj.cn

[U85] JS：可选链
来源：http://vz.521024.cn

a?.b?.c
来源：http://am.huixiangedu.cn

[U86] JS：空值合并
来源：http://ws.haigaiapp.cn

a ?? b
来源：http://zd.jctech888.com.cn

[U87] JS：解构默认值
来源：http://pc.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://tz.huanxung.cn

[U88] JS：对象展开合并
来源：http://vj.jctech888.com.cn

{ ...a, ...b }
来源：http://gq.wgjwhj.cn

[U89] JS：数组去重
来源：http://pi.panjiajie.cn

[...new Set(arr)]
来源：http://pp.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://gb.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://id.hahajie.cn

[U91] JS：对象键值遍历
来源：http://yl.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ai.nicolike.cn

[U92] JS：深拷贝
来源：http://iu.nicolike.cn

structuredClone(obj)
来源：http://lb.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://vf.nszjky.cn

`共 ${n} 条`
来源：http://eo.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://jd.wgjwhj.cn

const double = x => x * 2;
来源：http://bm.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://rq.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://yt.hahajie.cn

[U96] JS：async/await 与异常
来源：http://tk.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sf.521024.cn

[U97] JS：并发请求
来源：http://qx.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vu.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://pl.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hi.muxihuayi.cn

[U99] JS：事件监听
来源：http://av.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ts.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://sa.nicolike.cn

document.querySelector(".item")
来源：http://zr.lnxyls.cn

[U101] JS：classList 操作
来源：http://qv.chemitech.net.cn

el.classList.toggle("active")
来源：http://sy.lnxyls.cn

[U102] JS：本地存储
来源：http://vm.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sn.wgjwhj.cn

[U103] JS：定时器
来源：http://he.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://km.lnxyls.cn

[U104] JS：防抖
来源：http://ny.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pr.huixinmuqiang.cn

[U105] JS：节流
来源：http://kk.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ng.chemitech.net.cn

[U106] JS：日期格式化
来源：http://mn.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eb.panjiajie.cn

[U107] JS：数字千分位
来源：http://uq.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hc.wgjwhj.cn

[U108] JS：随机整数
来源：http://dc.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kz.jctech888.com.cn

[U109] JS：数组分组
来源：http://mi.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://dl.bookmarksfly.cn

[U110] JS：数组分块
来源：http://zi.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ft.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://an.huanxung.cn

new Map(Object.entries(obj))
来源：http://ym.lnxyls.cn

[U112] JS：字符串补位
来源：http://av.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://pf.panjiajie.cn

[U113] JS：正则替换全部
来源：http://bj.asd995.cn

s.replaceAll("a", "b")
来源：http://cb.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ea.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ju.colortex.cn

[U115] JS：生成 UUID
来源：http://at.bjjhwx.cn

crypto.randomUUID()
来源：http://ig.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://fn.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://ql.szsharing.cn

[U117] JS：单元测试
来源：http://wm.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://to.haigaiapp.cn

[U118] JS：开发服务器
来源：http://pz.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://fz.szsharing.cn

[U119] JS：生产构建
来源：http://zz.nicolike.cn

npx vite build
来源：http://fb.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://if.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://rp.wgjwhj.cn

================================================================================
来源：http://dg.panjiajie.cn

统计汇总
来源：http://ki.yuntaijiaju.cn

================================================================================
来源：http://pc.yuexingan06.cn

按语言统计（条）：
来源：http://fa.gzmigu.cn

Python ......... 252
来源：http://ko.jianghongdianzi.cn

PHP ............ 252
来源：http://dt.chemitech.net.cn

JavaScript ..... 252
来源：http://rw.chemitech.net.cn

TypeScript ..... 212
来源：http://lv.gzmigu.cn

Java ........... 212
来源：http://io.shtwfgs.cn

Go ............. 212
来源：http://se.asd995.cn

Ruby ........... 212
来源：http://tl.colortex.cn

C# ............. 212
来源：http://tv.9csxet.cn

C .............. 30
来源：http://dj.panjiajie.cn

C++ ............ 30
来源：http://wf.muxihuayi.cn

SQL ............ 90
来源：http://oz.lnxyls.cn

Bash ........... 80
来源：http://al.yuntaijiaju.cn

Kotlin ......... 15
来源：http://ln.9csxet.cn

Swift .......... 15
来源：http://kh.yuexingan06.cn

Lua ............ 10
来源：http://hy.nszjky.cn

Perl ........... 10
来源：http://la.shxzukj.cn

Scala .......... 10
来源：http://oe.shtwfgs.cn

------------------------------------
来源：http://xq.yuexingan06.cn

合计 ........... 2106 条
来源：http://oe.panjiajie.cn

按章节统计：
来源：http://hm.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wd.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bv.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mk.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hv.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yt.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ia.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://so.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gu.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gy.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mw.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gw.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qs.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eo.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sx.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cm.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uh.panjiajie.cn

Q SQL 专题                              90
来源：http://wh.yuexingan06.cn

R Bash 专题                             80
来源：http://kf.asd995.cn

S C / C++ 专题                          60
来源：http://bo.hahajie.cn

T 其他语言补充                          60
来源：http://ui.muxihuayi.cn

U 高频实用片段                         120
来源：http://rh.hahajie.cn

------------------------------------
来源：http://rw.szxytkj.cn

合计                                  2106 条
来源：http://fl.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://yq.shxzukj.cn

使用提醒
来源：http://tq.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://om.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fn.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sc.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ps.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sm.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vr.jctech888.com.cn

—— 文件结束 ——
来源：http://nu.nszjky.cn

================================================================================
来源：http://rz.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ar.huanxung.cn

Common Programming Examples Cheat Book
来源：http://dt.jctech888.com.cn

================================================================================
来源：http://xu.jianghongdianzi.cn

【收录内容】
来源：http://iu.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zb.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bi.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://dv.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://up.yuexingan06.cn

【使用说明】
来源：http://sd.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dl.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fn.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dc.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sb.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ca.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ts.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hp.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fp.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ap.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cv.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nz.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zs.9csxet.cn

【文件统计】
来源：http://nq.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://wg.haigaiapp.cn

目  录
来源：http://ix.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://xy.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qm.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pv.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lw.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oa.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dl.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mr.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fd.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zg.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bo.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://co.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ni.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zu.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gt.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vn.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sa.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lz.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kw.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lc.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kz.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uh.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fq.bookmarksfly.cn

================================================================================
来源：http://tq.wgjwhj.cn

A. 基础语法与类型
来源：http://gj.haigaiapp.cn

================================================================================
来源：http://bj.huixiangedu.cn

[A01] Hello World
来源：http://fw.nszjky.cn

Py:   print("Hello, World!")
来源：http://lb.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://cq.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://un.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zs.bjjhwx.cn

Java: System.out.println("Hello, World!");
来源：http://gp.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://lk.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://hn.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vh.newstarts.cn

[A02] 变量声明与赋值
来源：http://ky.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hb.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rn.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ui.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ck.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://ju.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://xm.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://be.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://au.jianghongdianzi.cn

[A03] 常量定义
来源：http://jd.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mo.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://km.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ij.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://nk.521024.cn

Java: static final double PI = 3.14159;
来源：http://mi.panjiajie.cn

Go:   const PI = 3.14159
来源：http://qi.szxytkj.cn

Ruby: PI = 3.14159
来源：http://be.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://no.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://aw.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ox.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gr.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mk.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://yi.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xg.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hq.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gg.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://ww.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://oz.shtwfgs.cn


<!-- 参考信息 -->