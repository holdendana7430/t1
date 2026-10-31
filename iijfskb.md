代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wn.szsharing.cn

sys.stdout.isatty()
来源：http://hj.colortex.cn

[U40] Py：打印到标准错误
来源：http://uy.hahajie.cn

print("err", file=sys.stderr)
来源：http://ex.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://gu.panjiajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bl.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://gj.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jq.asd995.cn

[U43] PHP：声明命名空间
来源：http://qb.lnxyls.cn

namespace App\Http;
来源：http://sp.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://xj.shxzukj.cn

declare(strict_types=1);
来源：http://un.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ql.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yg.wgjwhj.cn

[U46] PHP：可空类型
来源：http://lo.haigaiapp.cn

?string $name = null
来源：http://gr.muxihuayi.cn

[U47] PHP：联合类型
来源：http://lu.muxihuayi.cn

int|string $id
来源：http://ot.hnjuh.cn

[U48] PHP：纯枚举
来源：http://vf.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ys.szsharing.cn

[U49] PHP：只读属性
来源：http://vx.jianghongdianzi.cn

public readonly string $name
来源：http://lh.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ds.shxzukj.cn

public function __construct(private int $id) {}
来源：http://kt.jctech888.com.cn

[U51] PHP：数组解构
来源：http://xd.bjjhwx.cn

[$a, $b] = $arr;
来源：http://ah.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://ej.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://pb.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://of.jctech888.com.cn

$v = $a ?? $b ?? "default";
来源：http://el.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://cy.bjjhwx.cn

$obj?->method()
来源：http://wu.lnxyls.cn

[U55] PHP：match 表达式
来源：http://ff.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oj.haigaiapp.cn

[U56] PHP：命名参数
来源：http://dq.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ir.hahajie.cn

[U57] PHP：字符串插值
来源：http://es.asd995.cn

"值: {$a}"
来源：http://qs.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://ds.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ze.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://xz.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dl.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://ca.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ym.jctech888.com.cn

[U61] PHP：正则
来源：http://gf.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ld.colortex.cn

[U62] PHP：日期对象
来源：http://st.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iv.hnjuh.cn

[U63] PHP：文件读写
来源：http://mc.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ix.521024.cn

[U64] PHP：目录遍历
来源：http://sc.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://bs.gzmigu.cn

[U65] PHP：会话
来源：http://cd.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vo.521024.cn

[U66] PHP：设置 Cookie
来源：http://ec.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xk.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://xz.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yl.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://cs.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rf.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://pq.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nm.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://nh.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yh.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://gd.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://ol.bjjhwx.cn

[U72] PHP：写错误日志
来源：http://uc.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://od.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://kq.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://mg.asd995.cn

[U74] PHP：读取环境变量
来源：http://nj.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://yb.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://dr.hnjuh.cn

composer require psr/container
来源：http://sa.nicolike.cn

[U76] PHP：简单路由
来源：http://ne.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eg.nszjky.cn

[U77] PHP：模板渲染
来源：http://ne.yuexingan06.cn

composer require twig/twig
来源：http://fs.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://um.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://ub.szxytkj.cn

[U79] PHP：静态分析
来源：http://ii.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ez.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://sw.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dk.szsharing.cn

[U81] JS：初始化项目
来源：http://yv.panjiajie.cn

npm init -y;  npm i express
来源：http://pe.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://nq.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xn.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://no.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dx.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://yr.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bt.asd995.cn

[U85] JS：可选链
来源：http://th.yuexingan06.cn

a?.b?.c
来源：http://fw.asd995.cn

[U86] JS：空值合并
来源：http://ol.panjiajie.cn

a ?? b
来源：http://iu.9csxet.cn

[U87] JS：解构默认值
来源：http://zv.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://iz.nicolike.cn

[U88] JS：对象展开合并
来源：http://sw.huanxung.cn

{ ...a, ...b }
来源：http://la.haigaiapp.cn

[U89] JS：数组去重
来源：http://gs.panjiajie.cn

[...new Set(arr)]
来源：http://lh.shxzskj.cn

[U90] JS：数字数组排序
来源：http://kh.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://tm.colortex.cn

[U91] JS：对象键值遍历
来源：http://ir.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ky.nicolike.cn

[U92] JS：深拷贝
来源：http://or.bjjhwx.cn

structuredClone(obj)
来源：http://id.nszjky.cn

[U93] JS：模板字符串
来源：http://ra.yuexingan06.cn

`共 ${n} 条`
来源：http://ly.521024.cn

[U94] JS：箭头函数
来源：http://vr.shxzukj.cn

const double = x => x * 2;
来源：http://sh.9csxet.cn

[U95] JS：Promise 包装
来源：http://if.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://hh.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://qw.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dz.newstarts.cn

[U97] JS：并发请求
来源：http://rb.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cx.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://xa.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mg.wgjwhj.cn

[U99] JS：事件监听
来源：http://yc.huanxung.cn

el.addEventListener("click", e => {})
来源：http://xs.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://bm.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ak.lnxyls.cn

[U101] JS：classList 操作
来源：http://ky.bookmarksfly.cn

el.classList.toggle("active")
来源：http://rx.jctech888.com.cn

[U102] JS：本地存储
来源：http://gq.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mj.szxytkj.cn

[U103] JS：定时器
来源：http://ot.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pb.yuexingan06.cn

[U104] JS：防抖
来源：http://wo.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bk.panjiajie.cn

[U105] JS：节流
来源：http://pe.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ut.chemitech.net.cn

[U106] JS：日期格式化
来源：http://ua.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jo.shxzskj.cn

[U107] JS：数字千分位
来源：http://ff.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fm.hnjuh.cn

[U108] JS：随机整数
来源：http://do.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ff.lnxyls.cn

[U109] JS：数组分组
来源：http://ut.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://cr.haigaiapp.cn

[U110] JS：数组分块
来源：http://nb.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ke.szsharing.cn

[U111] JS：对象转 Map
来源：http://ab.gzmigu.cn

new Map(Object.entries(obj))
来源：http://cj.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://qt.newstarts.cn

"7".padStart(3, "0")
来源：http://qm.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ax.colortex.cn

s.replaceAll("a", "b")
来源：http://di.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://hs.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ju.szsharing.cn

[U115] JS：生成 UUID
来源：http://tp.nszjky.cn

crypto.randomUUID()
来源：http://bn.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://cp.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://zb.panjiajie.cn

[U117] JS：单元测试
来源：http://ko.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://sn.hnjuh.cn

[U118] JS：开发服务器
来源：http://uh.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://sa.panjiajie.cn

[U119] JS：生产构建
来源：http://yl.jianghongdianzi.cn

npx vite build
来源：http://tq.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://bg.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://ww.szsharing.cn

================================================================================
来源：http://iy.huanxung.cn

统计汇总
来源：http://tm.shtwfgs.cn

================================================================================
来源：http://gv.shxzskj.cn

按语言统计（条）：
来源：http://gs.yuexingan06.cn

Python ......... 252
来源：http://hk.bjjhwx.cn

PHP ............ 252
来源：http://zy.jctech888.com.cn

JavaScript ..... 252
来源：http://mf.bookmarksfly.cn

TypeScript ..... 212
来源：http://we.hnjuh.cn

Java ........... 212
来源：http://yq.jctech888.com.cn

Go ............. 212
来源：http://ba.wgjwhj.cn

Ruby ........... 212
来源：http://mo.9csxet.cn

C# ............. 212
来源：http://wl.hnjuh.cn

C .............. 30
来源：http://yr.gzmigu.cn

C++ ............ 30
来源：http://bm.panjiajie.cn

SQL ............ 90
来源：http://sc.szsharing.cn

Bash ........... 80
来源：http://mo.shxzskj.cn

Kotlin ......... 15
来源：http://rk.jctech888.com.cn

Swift .......... 15
来源：http://cs.haigaiapp.cn

Lua ............ 10
来源：http://br.hnjuh.cn

Perl ........... 10
来源：http://ly.huixinmuqiang.cn

Scala .......... 10
来源：http://pf.gzmigu.cn

------------------------------------
来源：http://zz.wgjwhj.cn

合计 ........... 2106 条
来源：http://lw.nszjky.cn

按章节统计：
来源：http://kv.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gx.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iy.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://od.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gj.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mt.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ec.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ox.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rp.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pz.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xo.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fs.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kf.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yo.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sr.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pi.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ba.bjjhwx.cn

Q SQL 专题                              90
来源：http://ws.shxzskj.cn

R Bash 专题                             80
来源：http://py.shtwfgs.cn

S C / C++ 专题                          60
来源：http://io.colortex.cn

T 其他语言补充                          60
来源：http://hf.shtwfgs.cn

U 高频实用片段                         120
来源：http://bk.jctech888.com.cn

------------------------------------
来源：http://qg.szxytkj.cn

合计                                  2106 条
来源：http://rl.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://if.huanxung.cn

使用提醒
来源：http://td.colortex.cn

--------------------------------------------------------------------------------
来源：http://xw.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ob.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dc.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ho.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wg.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cq.muxihuayi.cn

—— 文件结束 ——
来源：http://mp.shxzskj.cn

================================================================================
来源：http://af.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://te.asd995.cn

Common Programming Examples Cheat Book
来源：http://av.bookmarksfly.cn

================================================================================
来源：http://rb.shxzskj.cn

【收录内容】
来源：http://bb.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vj.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gc.newstarts.cn

SQL · Bash · C · C++
来源：http://bp.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vl.newstarts.cn

【使用说明】
来源：http://yf.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lr.huixiangedu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qh.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vb.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rl.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://be.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tc.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xk.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ip.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://va.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vn.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nz.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dy.shxzukj.cn

【文件统计】
来源：http://id.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pn.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://mf.huixinmuqiang.cn

目  录
来源：http://zv.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://tw.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fm.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jg.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pd.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mc.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fb.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jh.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vy.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ez.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uc.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ij.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xt.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vr.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ln.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zm.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rv.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ap.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hr.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qe.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ox.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ec.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vz.hnjuh.cn

================================================================================
来源：http://yh.9csxet.cn

A. 基础语法与类型
来源：http://fu.nicolike.cn

================================================================================
来源：http://fo.szsharing.cn

[A01] Hello World
来源：http://tn.hnjuh.cn

Py:   print("Hello, World!")
来源：http://kd.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://yw.asd995.cn

JS:   console.log("Hello, World!");
来源：http://to.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://il.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://wj.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://hx.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://ou.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sg.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://es.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ws.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xl.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xg.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vn.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://jz.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://tf.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://qx.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kx.shtwfgs.cn

[A03] 常量定义
来源：http://zy.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://df.colortex.cn

PHP:  const PI = 3.14159;
来源：http://fx.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://on.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://iv.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://jo.colortex.cn

Go:   const PI = 3.14159
来源：http://iq.panjiajie.cn

Ruby: PI = 3.14159
来源：http://ix.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://im.haigaiapp.cn

[A04] 判断变量类型
来源：http://gs.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jp.yuexingan06.cn


<!-- 参考信息 -->