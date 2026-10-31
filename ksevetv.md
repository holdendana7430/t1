代发 wailian999

[U37] Py：读写 Excel
来源：http://kq.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fk.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://kk.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://mk.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://qq.nszjky.cn

sys.stdout.isatty()
来源：http://gx.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ia.hnjuh.cn

print("err", file=sys.stderr)
来源：http://mr.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://tl.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zh.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://mm.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ys.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ph.muxihuayi.cn

namespace App\Http;
来源：http://hf.szsharing.cn

[U44] PHP：开启严格类型
来源：http://nj.huixinmuqiang.cn

declare(strict_types=1);
来源：http://we.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://tp.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bl.jctech888.com.cn

[U46] PHP：可空类型
来源：http://au.shxzukj.cn

?string $name = null
来源：http://nl.shxzukj.cn

[U47] PHP：联合类型
来源：http://rx.yuexingan06.cn

int|string $id
来源：http://uv.lnxyls.cn

[U48] PHP：纯枚举
来源：http://vz.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gd.huanxung.cn

[U49] PHP：只读属性
来源：http://kb.huanxung.cn

public readonly string $name
来源：http://zz.521024.cn

[U50] PHP：构造器属性提升
来源：http://vd.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://ea.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ip.shtwfgs.cn

[$a, $b] = $arr;
来源：http://do.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://iw.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://zd.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://ao.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://gm.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://fh.bjjhwx.cn

$obj?->method()
来源：http://vr.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://it.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ad.newstarts.cn

[U56] PHP：命名参数
来源：http://lk.9csxet.cn

f(a: 1, b: 2)
来源：http://ih.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://kf.hnjuh.cn

"值: {$a}"
来源：http://ji.521024.cn

[U58] PHP：数组三件套
来源：http://oe.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pl.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://ip.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dj.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://vr.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iq.bookmarksfly.cn

[U61] PHP：正则
来源：http://hh.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sx.wgjwhj.cn

[U62] PHP：日期对象
来源：http://zq.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hs.colortex.cn

[U63] PHP：文件读写
来源：http://kr.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kg.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://wf.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://wm.szxytkj.cn

[U65] PHP：会话
来源：http://wz.521024.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ti.521024.cn

[U66] PHP：设置 Cookie
来源：http://yh.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zx.9csxet.cn

[U67] PHP：处理文件上传
来源：http://gk.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hl.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://yt.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zl.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://uu.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oz.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://xl.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tn.shxzskj.cn

[U71] PHP：抛出异常
来源：http://dw.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://wk.szsharing.cn

[U72] PHP：写错误日志
来源：http://md.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://vw.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://fl.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://cd.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://nv.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ai.nicolike.cn

[U75] PHP：依赖注入
来源：http://fn.huanxung.cn

composer require psr/container
来源：http://rp.asd995.cn

[U76] PHP：简单路由
来源：http://xi.huixinmuqiang.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://km.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://fu.haigaiapp.cn

composer require twig/twig
来源：http://is.hnjuh.cn

[U78] PHP：单元测试
来源：http://xo.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://pa.asd995.cn

[U79] PHP：静态分析
来源：http://wb.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://bm.asd995.cn

[U80] PHP：代码规范修复
来源：http://ou.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fz.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://uw.shxzukj.cn

npm init -y;  npm i express
来源：http://df.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://cq.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sx.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://tj.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ux.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://kl.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ev.bjjhwx.cn

[U85] JS：可选链
来源：http://bp.huanxung.cn

a?.b?.c
来源：http://zq.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://ly.shxzskj.cn

a ?? b
来源：http://te.huanxung.cn

[U87] JS：解构默认值
来源：http://ol.jctech888.com.cn

const { a = 1, b = 2 } = obj;
来源：http://sq.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://hf.chemitech.net.cn

{ ...a, ...b }
来源：http://cv.colortex.cn

[U89] JS：数组去重
来源：http://bp.jctech888.com.cn

[...new Set(arr)]
来源：http://dm.szxytkj.cn

[U90] JS：数字数组排序
来源：http://kx.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://pb.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://yx.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yl.muxihuayi.cn

[U92] JS：深拷贝
来源：http://au.9csxet.cn

structuredClone(obj)
来源：http://wj.yuexingan06.cn

[U93] JS：模板字符串
来源：http://ru.szsharing.cn

`共 ${n} 条`
来源：http://yx.haigaiapp.cn

[U94] JS：箭头函数
来源：http://nm.nicolike.cn

const double = x => x * 2;
来源：http://sc.szxytkj.cn

[U95] JS：Promise 包装
来源：http://iz.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://tv.hahajie.cn

[U96] JS：async/await 与异常
来源：http://kt.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ty.newstarts.cn

[U97] JS：并发请求
来源：http://is.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hk.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://xz.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fo.bookmarksfly.cn

[U99] JS：事件监听
来源：http://km.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://or.9csxet.cn

[U100] JS：DOM 查询
来源：http://xy.9csxet.cn

document.querySelector(".item")
来源：http://po.bjjhwx.cn

[U101] JS：classList 操作
来源：http://bf.bookmarksfly.cn

el.classList.toggle("active")
来源：http://pe.colortex.cn

[U102] JS：本地存储
来源：http://mt.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://di.bjjhwx.cn

[U103] JS：定时器
来源：http://od.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tm.nszjky.cn

[U104] JS：防抖
来源：http://mb.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xi.jianghongdianzi.cn

[U105] JS：节流
来源：http://dy.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ti.newstarts.cn

[U106] JS：日期格式化
来源：http://uw.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cz.jctech888.com.cn

[U107] JS：数字千分位
来源：http://bh.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nx.muxihuayi.cn

[U108] JS：随机整数
来源：http://gn.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nszjky.cn

[U109] JS：数组分组
来源：http://qh.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ft.shxzukj.cn

[U110] JS：数组分块
来源：http://kw.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dc.521024.cn

[U111] JS：对象转 Map
来源：http://bw.szxytkj.cn

new Map(Object.entries(obj))
来源：http://qd.szsharing.cn

[U112] JS：字符串补位
来源：http://qr.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://qo.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://mx.nszjky.cn

s.replaceAll("a", "b")
来源：http://zn.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://dn.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ut.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://hd.colortex.cn

crypto.randomUUID()
来源：http://vz.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://iu.521024.cn

/** @param {string} name */ function f(name) {}
来源：http://dm.asd995.cn

[U117] JS：单元测试
来源：http://dx.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://zq.gzmigu.cn

[U118] JS：开发服务器
来源：http://wp.newstarts.cn

npm i -D vite;  npx vite
来源：http://qv.huixiangedu.cn

[U119] JS：生产构建
来源：http://mc.shxzskj.cn

npx vite build
来源：http://tv.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://nv.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://eh.gzmigu.cn

================================================================================
来源：http://uq.chemitech.net.cn

统计汇总
来源：http://av.lnxyls.cn

================================================================================
来源：http://yy.huixiangedu.cn

按语言统计（条）：
来源：http://xb.panjiajie.cn

Python ......... 252
来源：http://cr.shxzukj.cn

PHP ............ 252
来源：http://ge.bookmarksfly.cn

JavaScript ..... 252
来源：http://lc.lnxyls.cn

TypeScript ..... 212
来源：http://ut.521024.cn

Java ........... 212
来源：http://wv.muxihuayi.cn

Go ............. 212
来源：http://bv.chemitech.net.cn

Ruby ........... 212
来源：http://ns.huanxung.cn

C# ............. 212
来源：http://li.nicolike.cn

C .............. 30
来源：http://ns.huanxung.cn

C++ ............ 30
来源：http://zl.lnxyls.cn

SQL ............ 90
来源：http://op.shxzskj.cn

Bash ........... 80
来源：http://uo.hnjuh.cn

Kotlin ......... 15
来源：http://cr.huixinmuqiang.cn

Swift .......... 15
来源：http://bd.521024.cn

Lua ............ 10
来源：http://im.hahajie.cn

Perl ........... 10
来源：http://mh.bookmarksfly.cn

Scala .......... 10
来源：http://cf.shxzskj.cn

------------------------------------
来源：http://xp.shxzukj.cn

合计 ........... 2106 条
来源：http://ib.gzmigu.cn

按章节统计：
来源：http://dx.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zp.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vk.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yr.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://li.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ih.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://af.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ga.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zz.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pw.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uj.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dj.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qq.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ni.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aj.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ak.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sz.bjjhwx.cn

Q SQL 专题                              90
来源：http://yn.asd995.cn

R Bash 专题                             80
来源：http://ua.nicolike.cn

S C / C++ 专题                          60
来源：http://lb.yuexingan06.cn

T 其他语言补充                          60
来源：http://em.bjjhwx.cn

U 高频实用片段                         120
来源：http://zo.colortex.cn

------------------------------------
来源：http://tp.yuntaijiaju.cn

合计                                  2106 条
来源：http://gm.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ja.nszjky.cn

使用提醒
来源：http://uk.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://th.yuexingan06.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gy.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bd.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fu.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ig.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vf.yuexingan06.cn

—— 文件结束 ——
来源：http://fs.wgjwhj.cn

================================================================================
来源：http://em.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://yd.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://yu.nszjky.cn

================================================================================
来源：http://zf.huixinmuqiang.cn

【收录内容】
来源：http://rl.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vy.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lz.nicolike.cn

SQL · Bash · C · C++
来源：http://zt.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uz.lnxyls.cn

【使用说明】
来源：http://ne.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gn.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xc.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hn.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iv.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://md.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rk.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xa.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://op.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://di.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rz.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qm.bjjhwx.cn

【文件统计】
来源：http://dk.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hs.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://jz.huixinmuqiang.cn

目  录
来源：http://yt.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ib.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wa.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ri.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ep.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lm.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ht.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mi.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fw.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wh.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bx.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cq.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kk.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mt.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ck.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vd.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ve.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://si.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hy.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wa.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gb.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pn.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vr.asd995.cn

================================================================================
来源：http://wg.szxytkj.cn

A. 基础语法与类型
来源：http://jg.szxytkj.cn

================================================================================
来源：http://po.yuntaijiaju.cn

[A01] Hello World
来源：http://bk.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://al.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://hx.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://dp.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tb.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://mw.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://rb.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://qw.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://po.nszjky.cn

[A02] 变量声明与赋值
来源：http://ey.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ki.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zp.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ic.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iy.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://ke.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://jx.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://pf.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gp.muxihuayi.cn

[A03] 常量定义
来源：http://ik.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hi.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://pq.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://rt.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://dp.asd995.cn

Java: static final double PI = 3.14159;
来源：http://ov.panjiajie.cn

Go:   const PI = 3.14159
来源：http://il.wgjwhj.cn


<!-- 参考信息 -->