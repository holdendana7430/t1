代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://ak.wgjwhj.cn

sys.stdout.isatty()
来源：http://pg.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://bi.huanxung.cn

print("err", file=sys.stderr)
来源：http://pk.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://fa.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zf.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://qt.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ah.nicolike.cn

[U43] PHP：声明命名空间
来源：http://bh.gzmigu.cn

namespace App\Http;
来源：http://zm.nszjky.cn

[U44] PHP：开启严格类型
来源：http://me.nicolike.cn

declare(strict_types=1);
来源：http://wu.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://jp.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vt.shtwfgs.cn

[U46] PHP：可空类型
来源：http://qk.szsharing.cn

?string $name = null
来源：http://cr.shxzukj.cn

[U47] PHP：联合类型
来源：http://lk.asd995.cn

int|string $id
来源：http://ld.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://ew.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zt.shxzskj.cn

[U49] PHP：只读属性
来源：http://gu.gzmigu.cn

public readonly string $name
来源：http://fz.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://ee.panjiajie.cn

public function __construct(private int $id) {}
来源：http://wr.panjiajie.cn

[U51] PHP：数组解构
来源：http://uv.lnxyls.cn

[$a, $b] = $arr;
来源：http://tp.nicolike.cn

[U52] PHP：箭头函数
来源：http://hc.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://ol.nszjky.cn

[U53] PHP：空合并运算符
来源：http://rb.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://mn.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://cw.9csxet.cn

$obj?->method()
来源：http://pv.hahajie.cn

[U55] PHP：match 表达式
来源：http://hl.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yb.szxytkj.cn

[U56] PHP：命名参数
来源：http://fm.szxytkj.cn

f(a: 1, b: 2)
来源：http://xr.shxzskj.cn

[U57] PHP：字符串插值
来源：http://id.jctech888.com.cn

"值: {$a}"
来源：http://lp.nicolike.cn

[U58] PHP：数组三件套
来源：http://of.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sq.shxzskj.cn

[U59] PHP：自定义排序
来源：http://kr.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cl.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://cq.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vc.panjiajie.cn

[U61] PHP：正则
来源：http://hh.wgjwhj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tc.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://yn.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gq.szsharing.cn

[U63] PHP：文件读写
来源：http://ap.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cb.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ji.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://mi.szsharing.cn

[U65] PHP：会话
来源：http://cp.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eq.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ss.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rq.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://jw.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fi.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://nc.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lh.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://uu.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nc.jctech888.com.cn

[U70] PHP：PDO 事务
来源：http://kh.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qu.shxzskj.cn

[U71] PHP：抛出异常
来源：http://ke.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://px.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://mq.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://kb.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://tq.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://nr.szsharing.cn

[U74] PHP：读取环境变量
来源：http://ve.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://yg.shxzukj.cn

[U75] PHP：依赖注入
来源：http://rd.wgjwhj.cn

composer require psr/container
来源：http://jv.newstarts.cn

[U76] PHP：简单路由
来源：http://xs.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tr.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://kw.nicolike.cn

composer require twig/twig
来源：http://fs.bjjhwx.cn

[U78] PHP：单元测试
来源：http://ep.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://mu.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://sy.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://oj.9csxet.cn

[U80] PHP：代码规范修复
来源：http://xb.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ih.shxzukj.cn

[U81] JS：初始化项目
来源：http://rw.muxihuayi.cn

npm init -y;  npm i express
来源：http://up.bjjhwx.cn

[U82] JS：package.json 脚本
来源：http://sm.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wu.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://tt.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yk.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://qm.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oa.jianghongdianzi.cn

[U85] JS：可选链
来源：http://hi.yuexingan06.cn

a?.b?.c
来源：http://bs.huanxung.cn

[U86] JS：空值合并
来源：http://yg.hnjuh.cn

a ?? b
来源：http://wq.hnjuh.cn

[U87] JS：解构默认值
来源：http://zi.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://lx.521024.cn

[U88] JS：对象展开合并
来源：http://dq.jctech888.com.cn

{ ...a, ...b }
来源：http://wm.9csxet.cn

[U89] JS：数组去重
来源：http://nf.chemitech.net.cn

[...new Set(arr)]
来源：http://pc.521024.cn

[U90] JS：数字数组排序
来源：http://yt.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://na.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://ka.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tj.521024.cn

[U92] JS：深拷贝
来源：http://op.haigaiapp.cn

structuredClone(obj)
来源：http://rm.szxytkj.cn

[U93] JS：模板字符串
来源：http://vc.shxzskj.cn

`共 ${n} 条`
来源：http://aj.shxzukj.cn

[U94] JS：箭头函数
来源：http://dk.asd995.cn

const double = x => x * 2;
来源：http://gb.hahajie.cn

[U95] JS：Promise 包装
来源：http://cw.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://or.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://hx.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tc.huanxung.cn

[U97] JS：并发请求
来源：http://fj.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ua.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://qs.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fi.hnjuh.cn

[U99] JS：事件监听
来源：http://oj.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vd.hnjuh.cn

[U100] JS：DOM 查询
来源：http://jr.shxzukj.cn

document.querySelector(".item")
来源：http://pv.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ki.bookmarksfly.cn

el.classList.toggle("active")
来源：http://hl.hahajie.cn

[U102] JS：本地存储
来源：http://tc.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kg.9csxet.cn

[U103] JS：定时器
来源：http://sn.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ib.lnxyls.cn

[U104] JS：防抖
来源：http://or.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nr.jianghongdianzi.cn

[U105] JS：节流
来源：http://cg.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rk.shtwfgs.cn

[U106] JS：日期格式化
来源：http://ci.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vt.muxihuayi.cn

[U107] JS：数字千分位
来源：http://rf.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lu.huixiangedu.cn

[U108] JS：随机整数
来源：http://iu.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mv.nicolike.cn

[U109] JS：数组分组
来源：http://dc.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://tp.hahajie.cn

[U110] JS：数组分块
来源：http://gn.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://be.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://mt.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://ho.nicolike.cn

[U112] JS：字符串补位
来源：http://xh.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://gn.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ka.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://cd.huanxung.cn

[U114] JS：JSON 深比较
来源：http://kb.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ei.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://ey.szsharing.cn

crypto.randomUUID()
来源：http://tl.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://lk.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://ic.bjjhwx.cn

[U117] JS：单元测试
来源：http://pm.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://ei.gzmigu.cn

[U118] JS：开发服务器
来源：http://lc.nszjky.cn

npm i -D vite;  npx vite
来源：http://hw.jctech888.com.cn

[U119] JS：生产构建
来源：http://vq.huixiangedu.cn

npx vite build
来源：http://js.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://ij.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://cd.jctech888.com.cn

================================================================================
来源：http://qy.yuntaijiaju.cn

统计汇总
来源：http://ly.szsharing.cn

================================================================================
来源：http://zz.shxzukj.cn

按语言统计（条）：
来源：http://hr.asd995.cn

Python ......... 252
来源：http://nv.shxzskj.cn

PHP ............ 252
来源：http://jm.hnjuh.cn

JavaScript ..... 252
来源：http://je.bookmarksfly.cn

TypeScript ..... 212
来源：http://cy.shxzukj.cn

Java ........... 212
来源：http://yv.wgjwhj.cn

Go ............. 212
来源：http://ji.jctech888.com.cn

Ruby ........... 212
来源：http://pw.newstarts.cn

C# ............. 212
来源：http://rr.shtwfgs.cn

C .............. 30
来源：http://ya.huanxung.cn

C++ ............ 30
来源：http://nc.bjjhwx.cn

SQL ............ 90
来源：http://au.huanxung.cn

Bash ........... 80
来源：http://wy.shtwfgs.cn

Kotlin ......... 15
来源：http://cb.9csxet.cn

Swift .......... 15
来源：http://zb.bookmarksfly.cn

Lua ............ 10
来源：http://lv.huanxung.cn

Perl ........... 10
来源：http://ae.shxzskj.cn

Scala .......... 10
来源：http://re.jctech888.com.cn

------------------------------------
来源：http://rx.szsharing.cn

合计 ........... 2106 条
来源：http://bb.9csxet.cn

按章节统计：
来源：http://gz.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nc.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nd.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xw.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ik.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gr.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pm.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tm.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ow.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oz.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eg.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://og.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ed.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uu.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kg.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pf.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ar.nszjky.cn

Q SQL 专题                              90
来源：http://yg.chemitech.net.cn

R Bash 专题                             80
来源：http://bp.gzmigu.cn

S C / C++ 专题                          60
来源：http://tt.bookmarksfly.cn

T 其他语言补充                          60
来源：http://uv.huanxung.cn

U 高频实用片段                         120
来源：http://gh.shxzskj.cn

------------------------------------
来源：http://fz.hahajie.cn

合计                                  2106 条
来源：http://sx.colortex.cn

--------------------------------------------------------------------------------
来源：http://om.huanxung.cn

使用提醒
来源：http://sm.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://fk.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eh.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ig.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fu.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nw.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eb.huixinmuqiang.cn

—— 文件结束 ——
来源：http://jm.asd995.cn

================================================================================
来源：http://hw.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://ff.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://lo.huanxung.cn

================================================================================
来源：http://jh.shxzukj.cn

【收录内容】
来源：http://zm.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jt.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vz.jctech888.com.cn

SQL · Bash · C · C++
来源：http://gb.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://la.hahajie.cn

【使用说明】
来源：http://en.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vi.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ul.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://is.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cj.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nt.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sv.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ub.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ev.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lf.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pj.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dk.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sn.shxzskj.cn

【文件统计】
来源：http://bz.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zd.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://sx.newstarts.cn

目  录
来源：http://da.asd995.cn

--------------------------------------------------------------------------------
来源：http://nu.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dz.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tp.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fy.huixinmuqiang.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hb.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jb.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fu.shxzukj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gx.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fp.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uk.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hc.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xf.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sz.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ep.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ne.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vp.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sq.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fv.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kf.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xo.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fo.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ez.hnjuh.cn

================================================================================
来源：http://wx.huanxung.cn

A. 基础语法与类型
来源：http://wr.hnjuh.cn

================================================================================
来源：http://na.gzmigu.cn

[A01] Hello World
来源：http://eo.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://ij.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://wt.colortex.cn

JS:   console.log("Hello, World!");
来源：http://ej.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cu.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://ei.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ep.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://xn.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://km.panjiajie.cn

[A02] 变量声明与赋值
来源：http://gi.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wr.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sp.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dq.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cq.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://xv.521024.cn

Go:   name := "Alex"; age := 20
来源：http://pz.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://yi.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ag.lnxyls.cn

[A03] 常量定义
来源：http://ja.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qn.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://kn.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://wl.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://tg.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://zl.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://dc.panjiajie.cn

Ruby: PI = 3.14159
来源：http://iw.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://fy.bookmarksfly.cn

[A04] 判断变量类型
来源：http://im.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hv.lnxyls.cn


<!-- 参考信息 -->