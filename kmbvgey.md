代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://gy.newstarts.cn

sys.stdout.isatty()
来源：http://jy.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://dr.hahajie.cn

print("err", file=sys.stderr)
来源：http://fs.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://de.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dt.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://mn.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rt.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://pf.huixiangedu.cn

namespace App\Http;
来源：http://im.nicolike.cn

[U44] PHP：开启严格类型
来源：http://gd.panjiajie.cn

declare(strict_types=1);
来源：http://nw.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://au.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://re.9csxet.cn

[U46] PHP：可空类型
来源：http://hr.nicolike.cn

?string $name = null
来源：http://tz.shxzukj.cn

[U47] PHP：联合类型
来源：http://zl.szsharing.cn

int|string $id
来源：http://yk.hahajie.cn

[U48] PHP：纯枚举
来源：http://rr.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://en.jctech888.com.cn

[U49] PHP：只读属性
来源：http://jg.chemitech.net.cn

public readonly string $name
来源：http://ud.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://zi.nicolike.cn

public function __construct(private int $id) {}
来源：http://lr.newstarts.cn

[U51] PHP：数组解构
来源：http://rk.yuexingan06.cn

[$a, $b] = $arr;
来源：http://uf.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://vm.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://wr.9csxet.cn

[U53] PHP：空合并运算符
来源：http://zc.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://ve.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ol.huanxung.cn

$obj?->method()
来源：http://or.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://gh.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xd.muxihuayi.cn

[U56] PHP：命名参数
来源：http://ir.9csxet.cn

f(a: 1, b: 2)
来源：http://ai.asd995.cn

[U57] PHP：字符串插值
来源：http://jh.9csxet.cn

"值: {$a}"
来源：http://ti.hahajie.cn

[U58] PHP：数组三件套
来源：http://rf.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bn.newstarts.cn

[U59] PHP：自定义排序
来源：http://il.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gc.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://rb.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zi.9csxet.cn

[U61] PHP：正则
来源：http://cs.chemitech.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rx.9csxet.cn

[U62] PHP：日期对象
来源：http://ba.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qa.szsharing.cn

[U63] PHP：文件读写
来源：http://hz.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gv.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://hf.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://rq.hnjuh.cn

[U65] PHP：会话
来源：http://ly.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://by.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://zq.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jm.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://iu.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wm.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://ap.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://og.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://nw.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pq.colortex.cn

[U70] PHP：PDO 事务
来源：http://nz.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://it.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://rz.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://az.shxzskj.cn

[U72] PHP：写错误日志
来源：http://wl.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://kf.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://xp.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://up.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://yu.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://ok.nicolike.cn

[U75] PHP：依赖注入
来源：http://cp.huixiangedu.cn

composer require psr/container
来源：http://le.yuexingan06.cn

[U76] PHP：简单路由
来源：http://yg.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yf.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://ah.wgjwhj.cn

composer require twig/twig
来源：http://ub.shxzukj.cn

[U78] PHP：单元测试
来源：http://lc.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://qg.huanxung.cn

[U79] PHP：静态分析
来源：http://wh.newstarts.cn

composer require --dev phpstan/phpstan
来源：http://zs.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://jp.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fh.gzmigu.cn

[U81] JS：初始化项目
来源：http://mh.yuexingan06.cn

npm init -y;  npm i express
来源：http://oe.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://fm.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://px.521024.cn

[U83] JS：ES Module 导入导出
来源：http://en.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ss.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://xy.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://td.shtwfgs.cn

[U85] JS：可选链
来源：http://mw.521024.cn

a?.b?.c
来源：http://bu.jctech888.com.cn

[U86] JS：空值合并
来源：http://og.szsharing.cn

a ?? b
来源：http://go.wgjwhj.cn

[U87] JS：解构默认值
来源：http://ld.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://kp.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://mw.bookmarksfly.cn

{ ...a, ...b }
来源：http://sd.wgjwhj.cn

[U89] JS：数组去重
来源：http://du.lnxyls.cn

[...new Set(arr)]
来源：http://ep.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://hl.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://ex.521024.cn

[U91] JS：对象键值遍历
来源：http://pn.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fp.nszjky.cn

[U92] JS：深拷贝
来源：http://rz.muxihuayi.cn

structuredClone(obj)
来源：http://xb.bjjhwx.cn

[U93] JS：模板字符串
来源：http://jy.newstarts.cn

`共 ${n} 条`
来源：http://vl.521024.cn

[U94] JS：箭头函数
来源：http://xq.yuntaijiaju.cn

const double = x => x * 2;
来源：http://gj.colortex.cn

[U95] JS：Promise 包装
来源：http://cq.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://dw.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://wd.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pe.panjiajie.cn

[U97] JS：并发请求
来源：http://tk.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yf.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://tp.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xp.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://ml.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://md.lnxyls.cn

[U100] JS：DOM 查询
来源：http://dr.nszjky.cn

document.querySelector(".item")
来源：http://mt.bjjhwx.cn

[U101] JS：classList 操作
来源：http://sy.szxytkj.cn

el.classList.toggle("active")
来源：http://ph.bookmarksfly.cn

[U102] JS：本地存储
来源：http://yt.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gb.yuexingan06.cn

[U103] JS：定时器
来源：http://yz.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gd.gzmigu.cn

[U104] JS：防抖
来源：http://na.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wt.chemitech.net.cn

[U105] JS：节流
来源：http://zv.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lu.haigaiapp.cn

[U106] JS：日期格式化
来源：http://pf.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gg.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ma.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ri.yuexingan06.cn

[U108] JS：随机整数
来源：http://lv.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://er.shtwfgs.cn

[U109] JS：数组分组
来源：http://ll.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://vb.huanxung.cn

[U110] JS：数组分块
来源：http://ru.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bt.lnxyls.cn

[U111] JS：对象转 Map
来源：http://aw.521024.cn

new Map(Object.entries(obj))
来源：http://zv.hnjuh.cn

[U112] JS：字符串补位
来源：http://yz.newstarts.cn

"7".padStart(3, "0")
来源：http://df.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://lu.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://hw.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://ww.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tc.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://jf.muxihuayi.cn

crypto.randomUUID()
来源：http://iz.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://pk.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://ie.shxzskj.cn

[U117] JS：单元测试
来源：http://fa.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://cl.nszjky.cn

[U118] JS：开发服务器
来源：http://xx.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://te.wgjwhj.cn

[U119] JS：生产构建
来源：http://dv.nszjky.cn

npx vite build
来源：http://gu.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://gs.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://yy.newstarts.cn

================================================================================
来源：http://aj.nszjky.cn

统计汇总
来源：http://md.lnxyls.cn

================================================================================
来源：http://bt.9csxet.cn

按语言统计（条）：
来源：http://en.9csxet.cn

Python ......... 252
来源：http://uu.huixiangedu.cn

PHP ............ 252
来源：http://wh.shxzskj.cn

JavaScript ..... 252
来源：http://lv.521024.cn

TypeScript ..... 212
来源：http://qd.huanxung.cn

Java ........... 212
来源：http://bi.yuntaijiaju.cn

Go ............. 212
来源：http://sl.muxihuayi.cn

Ruby ........... 212
来源：http://bx.lnxyls.cn

C# ............. 212
来源：http://vh.bookmarksfly.cn

C .............. 30
来源：http://lz.yuexingan06.cn

C++ ............ 30
来源：http://lv.newstarts.cn

SQL ............ 90
来源：http://bm.521024.cn

Bash ........... 80
来源：http://hd.huixinmuqiang.cn

Kotlin ......... 15
来源：http://mm.muxihuayi.cn

Swift .......... 15
来源：http://bo.chemitech.net.cn

Lua ............ 10
来源：http://qq.huixinmuqiang.cn

Perl ........... 10
来源：http://bn.jianghongdianzi.cn

Scala .......... 10
来源：http://dl.bjjhwx.cn

------------------------------------
来源：http://uo.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://ep.huixiangedu.cn

按章节统计：
来源：http://yp.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nl.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gq.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mn.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wl.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zt.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vr.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gc.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zd.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rb.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ct.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ug.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fq.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vx.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fw.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hq.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eq.asd995.cn

Q SQL 专题                              90
来源：http://ly.szsharing.cn

R Bash 专题                             80
来源：http://wo.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://tp.shtwfgs.cn

T 其他语言补充                          60
来源：http://iu.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://ea.gzmigu.cn

------------------------------------
来源：http://ug.yuexingan06.cn

合计                                  2106 条
来源：http://xf.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://rk.muxihuayi.cn

使用提醒
来源：http://wu.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://bs.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lu.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lf.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kj.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ix.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mq.newstarts.cn

—— 文件结束 ——
来源：http://lu.hahajie.cn

================================================================================
来源：http://mb.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://mz.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://vs.yuntaijiaju.cn

================================================================================
来源：http://ka.panjiajie.cn

【收录内容】
来源：http://ha.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zi.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ty.newstarts.cn

SQL · Bash · C · C++
来源：http://qi.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pl.jianghongdianzi.cn

【使用说明】
来源：http://gp.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rf.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lb.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sb.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vf.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mt.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yo.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ul.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ps.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qr.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://au.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://as.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ou.jctech888.com.cn

【文件统计】
来源：http://af.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iu.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://pq.panjiajie.cn

目  录
来源：http://hg.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://eo.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lz.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ri.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gi.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tf.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tc.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ij.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gj.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dn.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xj.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://de.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gz.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bs.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hs.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qt.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ld.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tq.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vn.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cb.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vz.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rm.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pt.szsharing.cn

================================================================================
来源：http://iz.hnjuh.cn

A. 基础语法与类型
来源：http://yr.nszjky.cn

================================================================================
来源：http://gr.shtwfgs.cn

[A01] Hello World
来源：http://rz.521024.cn

Py:   print("Hello, World!")
来源：http://dw.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://mf.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://ni.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xm.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://kr.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://oa.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://gw.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vo.colortex.cn

[A02] 变量声明与赋值
来源：http://sf.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jb.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xd.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bj.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fm.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://wp.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://hs.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://as.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lw.lnxyls.cn

[A03] 常量定义
来源：http://us.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qu.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://za.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://bz.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://zk.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://js.szsharing.cn

Go:   const PI = 3.14159
来源：http://ls.asd995.cn

Ruby: PI = 3.14159
来源：http://po.asd995.cn

C#:   const double PI = 3.14159;
来源：http://nc.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://az.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qt.newstarts.cn


<!-- 参考信息 -->