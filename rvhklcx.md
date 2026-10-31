代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://sa.panjiajie.cn

sys.stdout.isatty()
来源：http://md.hahajie.cn

[U40] Py：打印到标准错误
来源：http://sj.colortex.cn

print("err", file=sys.stderr)
来源：http://bp.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ux.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://na.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://of.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rt.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://vd.huanxung.cn

namespace App\Http;
来源：http://zm.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://wr.gzmigu.cn

declare(strict_types=1);
来源：http://ru.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://zc.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://di.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://hi.shxzukj.cn

?string $name = null
来源：http://gc.shxzukj.cn

[U47] PHP：联合类型
来源：http://yp.9csxet.cn

int|string $id
来源：http://xk.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://kk.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wo.shxzskj.cn

[U49] PHP：只读属性
来源：http://az.asd995.cn

public readonly string $name
来源：http://tx.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://fk.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://de.colortex.cn

[U51] PHP：数组解构
来源：http://kh.lnxyls.cn

[$a, $b] = $arr;
来源：http://ye.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://fg.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://kx.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://by.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://nd.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://ay.panjiajie.cn

$obj?->method()
来源：http://ix.nszjky.cn

[U55] PHP：match 表达式
来源：http://de.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nf.wgjwhj.cn

[U56] PHP：命名参数
来源：http://lv.nicolike.cn

f(a: 1, b: 2)
来源：http://pw.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://fb.hnjuh.cn

"值: {$a}"
来源：http://jq.colortex.cn

[U58] PHP：数组三件套
来源：http://qa.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ou.nszjky.cn

[U59] PHP：自定义排序
来源：http://bt.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qg.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://jh.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dc.nszjky.cn

[U61] PHP：正则
来源：http://ji.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ls.bjjhwx.cn

[U62] PHP：日期对象
来源：http://zr.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ac.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://kg.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.9csxet.cn

[U64] PHP：目录遍历
来源：http://pl.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ud.yuntaijiaju.cn

[U65] PHP：会话
来源：http://qv.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hx.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://ny.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ji.newstarts.cn

[U67] PHP：处理文件上传
来源：http://iv.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qn.521024.cn

[U68] PHP：PDO 连接
来源：http://ba.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fw.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://gm.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lp.wgjwhj.cn

[U70] PHP：PDO 事务
来源：http://xi.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bi.szxytkj.cn

[U71] PHP：抛出异常
来源：http://kt.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://rb.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://ri.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://eq.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ns.521024.cn

parse_ini_file("config.ini", true)
来源：http://vp.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://oy.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://gk.huanxung.cn

[U75] PHP：依赖注入
来源：http://cd.lnxyls.cn

composer require psr/container
来源：http://sb.hnjuh.cn

[U76] PHP：简单路由
来源：http://lz.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sa.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://mh.yuntaijiaju.cn

composer require twig/twig
来源：http://kr.haigaiapp.cn

[U78] PHP：单元测试
来源：http://ek.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://el.lnxyls.cn

[U79] PHP：静态分析
来源：http://eb.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://vw.nicolike.cn

[U80] PHP：代码规范修复
来源：http://je.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ti.wgjwhj.cn

[U81] JS：初始化项目
来源：http://td.huanxung.cn

npm init -y;  npm i express
来源：http://az.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://sq.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cu.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://xk.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://op.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://jd.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://js.szsharing.cn

[U85] JS：可选链
来源：http://ae.hnjuh.cn

a?.b?.c
来源：http://mt.bjjhwx.cn

[U86] JS：空值合并
来源：http://ks.nicolike.cn

a ?? b
来源：http://pn.asd995.cn

[U87] JS：解构默认值
来源：http://qh.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://uh.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://dj.9csxet.cn

{ ...a, ...b }
来源：http://qu.lnxyls.cn

[U89] JS：数组去重
来源：http://qo.asd995.cn

[...new Set(arr)]
来源：http://um.asd995.cn

[U90] JS：数字数组排序
来源：http://oz.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://kx.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://ur.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://od.lnxyls.cn

[U92] JS：深拷贝
来源：http://jr.huixiangedu.cn

structuredClone(obj)
来源：http://yu.huanxung.cn

[U93] JS：模板字符串
来源：http://fw.jctech888.com.cn

`共 ${n} 条`
来源：http://zx.nszjky.cn

[U94] JS：箭头函数
来源：http://fo.hnjuh.cn

const double = x => x * 2;
来源：http://ik.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://oy.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://sp.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://wu.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ww.chemitech.net.cn

[U97] JS：并发请求
来源：http://ff.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://rv.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zw.huanxung.cn

[U99] JS：事件监听
来源：http://fe.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://ka.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://nv.asd995.cn

document.querySelector(".item")
来源：http://lv.szsharing.cn

[U101] JS：classList 操作
来源：http://bx.newstarts.cn

el.classList.toggle("active")
来源：http://ft.huixiangedu.cn

[U102] JS：本地存储
来源：http://cl.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://et.yuntaijiaju.cn

[U103] JS：定时器
来源：http://sp.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ac.huixiangedu.cn

[U104] JS：防抖
来源：http://vt.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yj.jctech888.com.cn

[U105] JS：节流
来源：http://nu.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yx.bjjhwx.cn

[U106] JS：日期格式化
来源：http://oz.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iq.nicolike.cn

[U107] JS：数字千分位
来源：http://ze.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://om.lnxyls.cn

[U108] JS：随机整数
来源：http://yx.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yz.wgjwhj.cn

[U109] JS：数组分组
来源：http://tq.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://gv.9csxet.cn

[U110] JS：数组分块
来源：http://rt.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zz.gzmigu.cn

[U111] JS：对象转 Map
来源：http://br.szxytkj.cn

new Map(Object.entries(obj))
来源：http://um.shxzskj.cn

[U112] JS：字符串补位
来源：http://ns.521024.cn

"7".padStart(3, "0")
来源：http://hg.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://fh.lnxyls.cn

s.replaceAll("a", "b")
来源：http://qi.hahajie.cn

[U114] JS：JSON 深比较
来源：http://mh.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xy.nszjky.cn

[U115] JS：生成 UUID
来源：http://ku.nicolike.cn

crypto.randomUUID()
来源：http://py.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://to.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://rv.colortex.cn

[U117] JS：单元测试
来源：http://io.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://yz.gzmigu.cn

[U118] JS：开发服务器
来源：http://xn.asd995.cn

npm i -D vite;  npx vite
来源：http://xa.haigaiapp.cn

[U119] JS：生产构建
来源：http://ol.yuntaijiaju.cn

npx vite build
来源：http://td.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://xh.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://tr.shxzskj.cn

================================================================================
来源：http://gv.wgjwhj.cn

统计汇总
来源：http://iy.shtwfgs.cn

================================================================================
来源：http://pl.9csxet.cn

按语言统计（条）：
来源：http://pq.asd995.cn

Python ......... 252
来源：http://dj.bookmarksfly.cn

PHP ............ 252
来源：http://th.szxytkj.cn

JavaScript ..... 252
来源：http://af.shxzukj.cn

TypeScript ..... 212
来源：http://uc.nicolike.cn

Java ........... 212
来源：http://nz.jctech888.com.cn

Go ............. 212
来源：http://nj.asd995.cn

Ruby ........... 212
来源：http://zu.521024.cn

C# ............. 212
来源：http://pm.9csxet.cn

C .............. 30
来源：http://mv.muxihuayi.cn

C++ ............ 30
来源：http://pr.panjiajie.cn

SQL ............ 90
来源：http://ce.colortex.cn

Bash ........... 80
来源：http://jc.szxytkj.cn

Kotlin ......... 15
来源：http://cx.muxihuayi.cn

Swift .......... 15
来源：http://rm.gzmigu.cn

Lua ............ 10
来源：http://ar.nszjky.cn

Perl ........... 10
来源：http://ag.muxihuayi.cn

Scala .......... 10
来源：http://af.hnjuh.cn

------------------------------------
来源：http://wh.9csxet.cn

合计 ........... 2106 条
来源：http://ag.huixinmuqiang.cn

按章节统计：
来源：http://da.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pt.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fv.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aw.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wy.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://my.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cp.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sh.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zx.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yd.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ek.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ou.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hi.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vj.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gx.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kp.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sm.jctech888.com.cn

Q SQL 专题                              90
来源：http://kk.jctech888.com.cn

R Bash 专题                             80
来源：http://qb.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://mu.haigaiapp.cn

T 其他语言补充                          60
来源：http://eg.shxzskj.cn

U 高频实用片段                         120
来源：http://la.bookmarksfly.cn

------------------------------------
来源：http://zf.newstarts.cn

合计                                  2106 条
来源：http://wf.huanxung.cn

--------------------------------------------------------------------------------
来源：http://rt.hnjuh.cn

使用提醒
来源：http://sa.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://oy.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bw.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yp.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jc.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://js.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oi.bookmarksfly.cn

—— 文件结束 ——
来源：http://fg.hahajie.cn

================================================================================
来源：http://sa.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://al.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://vf.huixinmuqiang.cn

================================================================================
来源：http://uy.haigaiapp.cn

【收录内容】
来源：http://qs.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://th.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iv.colortex.cn

SQL · Bash · C · C++
来源：http://zr.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oc.hnjuh.cn

【使用说明】
来源：http://tg.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zl.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ro.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gt.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://my.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sr.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lo.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wt.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://am.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nb.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jr.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xw.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xf.asd995.cn

【文件统计】
来源：http://nr.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ee.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ap.yuntaijiaju.cn

目  录
来源：http://km.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://kz.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xi.muxihuayi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lg.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mb.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tg.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://te.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://at.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qs.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vy.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://np.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fw.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mt.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zq.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://my.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ai.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hp.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://js.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bf.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ec.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qu.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://es.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eg.asd995.cn

================================================================================
来源：http://bz.yuexingan06.cn

A. 基础语法与类型
来源：http://jn.hahajie.cn

================================================================================
来源：http://jr.bookmarksfly.cn

[A01] Hello World
来源：http://wc.hahajie.cn

Py:   print("Hello, World!")
来源：http://tl.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://uf.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://pt.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cf.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://xr.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://om.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://vg.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fy.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://cc.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vb.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yx.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nu.wgjwhj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bm.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://lv.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://kh.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://pm.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://so.gzmigu.cn

[A03] 常量定义
来源：http://an.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yl.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://kf.9csxet.cn

JS:   const PI = 3.14159;
来源：http://ln.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://wh.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://by.huanxung.cn

Go:   const PI = 3.14159
来源：http://gc.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://no.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://wc.lnxyls.cn

[A04] 判断变量类型
来源：http://rm.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://td.bookmarksfly.cn


<!-- 参考信息 -->