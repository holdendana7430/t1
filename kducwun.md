代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://gc.huanxung.cn

sys.stdout.isatty()
来源：http://zq.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://aq.asd995.cn

print("err", file=sys.stderr)
来源：http://cp.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://fk.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zu.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://uw.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fa.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://nv.yuntaijiaju.cn

namespace App\Http;
来源：http://rb.newstarts.cn

[U44] PHP：开启严格类型
来源：http://ua.yuntaijiaju.cn

declare(strict_types=1);
来源：http://qf.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://or.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://as.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://pf.bookmarksfly.cn

?string $name = null
来源：http://qx.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://je.nszjky.cn

int|string $id
来源：http://dc.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://kf.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mv.huanxung.cn

[U49] PHP：只读属性
来源：http://lu.huixiangedu.cn

public readonly string $name
来源：http://dh.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://oz.hahajie.cn

public function __construct(private int $id) {}
来源：http://mf.newstarts.cn

[U51] PHP：数组解构
来源：http://en.yuexingan06.cn

[$a, $b] = $arr;
来源：http://dg.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://sg.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://xu.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ob.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ak.shxzukj.cn

[U54] PHP：空安全调用
来源：http://xt.chemitech.net.cn

$obj?->method()
来源：http://wh.szsharing.cn

[U55] PHP：match 表达式
来源：http://dk.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ip.hahajie.cn

[U56] PHP：命名参数
来源：http://po.gzmigu.cn

f(a: 1, b: 2)
来源：http://nr.asd995.cn

[U57] PHP：字符串插值
来源：http://yl.huixiangedu.cn

"值: {$a}"
来源：http://qh.hahajie.cn

[U58] PHP：数组三件套
来源：http://el.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tv.lnxyls.cn

[U59] PHP：自定义排序
来源：http://qu.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aw.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://td.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gp.muxihuayi.cn

[U61] PHP：正则
来源：http://jv.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jc.wgjwhj.cn

[U62] PHP：日期对象
来源：http://lt.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ik.gzmigu.cn

[U63] PHP：文件读写
来源：http://ek.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ug.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://sc.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://yk.wgjwhj.cn

[U65] PHP：会话
来源：http://fh.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ob.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://pd.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ft.nszjky.cn

[U67] PHP：处理文件上传
来源：http://kj.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fp.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://fi.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rk.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://qg.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nf.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://bc.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xi.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://pz.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://bp.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://gh.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://cc.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://zn.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://an.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ah.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://ve.hahajie.cn

[U75] PHP：依赖注入
来源：http://lh.hahajie.cn

composer require psr/container
来源：http://zj.colortex.cn

[U76] PHP：简单路由
来源：http://pj.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://df.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://cr.szxytkj.cn

composer require twig/twig
来源：http://vn.chemitech.net.cn

[U78] PHP：单元测试
来源：http://eq.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://vb.hnjuh.cn

[U79] PHP：静态分析
来源：http://xj.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://nr.huanxung.cn

[U80] PHP：代码规范修复
来源：http://wt.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oq.hnjuh.cn

[U81] JS：初始化项目
来源：http://yz.hahajie.cn

npm init -y;  npm i express
来源：http://mv.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://cq.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jq.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://yc.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cz.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://hr.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jr.9csxet.cn

[U85] JS：可选链
来源：http://bp.muxihuayi.cn

a?.b?.c
来源：http://bh.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://yx.panjiajie.cn

a ?? b
来源：http://el.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://qp.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://lq.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://xr.jctech888.com.cn

{ ...a, ...b }
来源：http://us.lnxyls.cn

[U89] JS：数组去重
来源：http://tq.lnxyls.cn

[...new Set(arr)]
来源：http://sv.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://sg.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://pp.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://tk.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oq.newstarts.cn

[U92] JS：深拷贝
来源：http://mg.huanxung.cn

structuredClone(obj)
来源：http://rb.shxzskj.cn

[U93] JS：模板字符串
来源：http://xu.hnjuh.cn

`共 ${n} 条`
来源：http://mi.shtwfgs.cn

[U94] JS：箭头函数
来源：http://kc.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ct.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://lt.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://se.521024.cn

[U96] JS：async/await 与异常
来源：http://ii.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vj.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://az.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://so.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://wb.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nf.521024.cn

[U99] JS：事件监听
来源：http://ro.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://vn.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://rp.bjjhwx.cn

document.querySelector(".item")
来源：http://dt.521024.cn

[U101] JS：classList 操作
来源：http://aq.szxytkj.cn

el.classList.toggle("active")
来源：http://kj.hahajie.cn

[U102] JS：本地存储
来源：http://hm.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fn.shxzukj.cn

[U103] JS：定时器
来源：http://ms.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lf.nszjky.cn

[U104] JS：防抖
来源：http://tx.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.shxzskj.cn

[U105] JS：节流
来源：http://qv.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ts.haigaiapp.cn

[U106] JS：日期格式化
来源：http://ye.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bo.shtwfgs.cn

[U107] JS：数字千分位
来源：http://pl.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://na.szxytkj.cn

[U108] JS：随机整数
来源：http://oz.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jv.szsharing.cn

[U109] JS：数组分组
来源：http://ya.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://sh.chemitech.net.cn

[U110] JS：数组分块
来源：http://up.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ec.panjiajie.cn

[U111] JS：对象转 Map
来源：http://kn.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://tt.newstarts.cn

[U112] JS：字符串补位
来源：http://yz.szsharing.cn

"7".padStart(3, "0")
来源：http://cm.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://xh.lnxyls.cn

s.replaceAll("a", "b")
来源：http://va.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://zw.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cy.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://ih.9csxet.cn

crypto.randomUUID()
来源：http://to.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://og.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ts.shxzskj.cn

[U117] JS：单元测试
来源：http://we.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://bd.panjiajie.cn

[U118] JS：开发服务器
来源：http://uy.szsharing.cn

npm i -D vite;  npx vite
来源：http://xl.wgjwhj.cn

[U119] JS：生产构建
来源：http://vs.bjjhwx.cn

npx vite build
来源：http://cy.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://jo.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://gq.szxytkj.cn

================================================================================
来源：http://ac.bjjhwx.cn

统计汇总
来源：http://iw.nszjky.cn

================================================================================
来源：http://rc.szxytkj.cn

按语言统计（条）：
来源：http://rk.nszjky.cn

Python ......... 252
来源：http://fu.gzmigu.cn

PHP ............ 252
来源：http://vr.huixiangedu.cn

JavaScript ..... 252
来源：http://so.hnjuh.cn

TypeScript ..... 212
来源：http://ju.yuexingan06.cn

Java ........... 212
来源：http://xd.jianghongdianzi.cn

Go ............. 212
来源：http://ro.huixinmuqiang.cn

Ruby ........... 212
来源：http://jj.haigaiapp.cn

C# ............. 212
来源：http://df.yuexingan06.cn

C .............. 30
来源：http://ov.hnjuh.cn

C++ ............ 30
来源：http://ms.shxzukj.cn

SQL ............ 90
来源：http://hv.hahajie.cn

Bash ........... 80
来源：http://zi.nicolike.cn

Kotlin ......... 15
来源：http://rj.panjiajie.cn

Swift .......... 15
来源：http://gb.jctech888.com.cn

Lua ............ 10
来源：http://nm.newstarts.cn

Perl ........... 10
来源：http://xj.panjiajie.cn

Scala .......... 10
来源：http://wh.gzmigu.cn

------------------------------------
来源：http://au.9csxet.cn

合计 ........... 2106 条
来源：http://hh.9csxet.cn

按章节统计：
来源：http://cd.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yq.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gr.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://os.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qk.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bc.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ae.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wy.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cd.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fs.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tp.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ob.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fg.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bv.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xi.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ec.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bm.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://bt.hahajie.cn

R Bash 专题                             80
来源：http://xc.nszjky.cn

S C / C++ 专题                          60
来源：http://mn.huixiangedu.cn

T 其他语言补充                          60
来源：http://nt.jctech888.com.cn

U 高频实用片段                         120
来源：http://rq.panjiajie.cn

------------------------------------
来源：http://kx.shxzskj.cn

合计                                  2106 条
来源：http://xj.521024.cn

--------------------------------------------------------------------------------
来源：http://qd.szsharing.cn

使用提醒
来源：http://bm.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://pp.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ym.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oo.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://na.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cq.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aj.hahajie.cn

—— 文件结束 ——
来源：http://qm.asd995.cn

================================================================================
来源：http://yp.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://oa.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://ay.shxzskj.cn

================================================================================
来源：http://xv.huanxung.cn

【收录内容】
来源：http://cc.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jr.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wu.szsharing.cn

SQL · Bash · C · C++
来源：http://cn.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bd.nszjky.cn

【使用说明】
来源：http://fu.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xf.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ti.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zq.521024.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pr.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pe.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ny.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fk.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vw.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zk.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qn.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ru.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bm.muxihuayi.cn

【文件统计】
来源：http://vf.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jq.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zh.huanxung.cn

目  录
来源：http://sa.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://yx.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hk.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qw.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uu.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cy.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vy.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hd.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vh.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jl.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kn.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uw.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://io.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ga.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xs.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tv.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iu.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hb.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vp.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ty.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://np.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kw.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ao.gzmigu.cn

================================================================================
来源：http://is.huanxung.cn

A. 基础语法与类型
来源：http://wj.hnjuh.cn

================================================================================
来源：http://lq.nicolike.cn

[A01] Hello World
来源：http://xt.asd995.cn

Py:   print("Hello, World!")
来源：http://qi.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://ft.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://hp.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xs.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://tc.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://zm.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://ak.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ge.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://xg.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ze.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vx.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ko.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gt.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://tv.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://eh.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://ev.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kf.yuntaijiaju.cn

[A03] 常量定义
来源：http://si.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nr.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://lq.nicolike.cn

JS:   const PI = 3.14159;
来源：http://fl.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://be.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://nu.9csxet.cn

Go:   const PI = 3.14159
来源：http://tv.szxytkj.cn

Ruby: PI = 3.14159
来源：http://zb.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://dp.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://hk.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cv.jctech888.com.cn


<!-- 参考信息 -->