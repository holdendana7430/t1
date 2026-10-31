代发 wailian999

[U37] Py：读写 Excel
来源：http://tg.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fw.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://mq.lnxyls.cn

Path(__file__).resolve().parent
来源：http://yy.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://ky.bookmarksfly.cn

sys.stdout.isatty()
来源：http://cy.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://wv.newstarts.cn

print("err", file=sys.stderr)
来源：http://jh.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://xq.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xj.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://jy.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ma.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://rb.bookmarksfly.cn

namespace App\Http;
来源：http://im.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://yb.shxzskj.cn

declare(strict_types=1);
来源：http://jl.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://ux.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rh.hahajie.cn

[U46] PHP：可空类型
来源：http://fm.colortex.cn

?string $name = null
来源：http://yu.521024.cn

[U47] PHP：联合类型
来源：http://ge.521024.cn

int|string $id
来源：http://qw.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://pz.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sp.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://ng.shxzskj.cn

public readonly string $name
来源：http://no.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ri.szxytkj.cn

public function __construct(private int $id) {}
来源：http://it.gzmigu.cn

[U51] PHP：数组解构
来源：http://xa.hnjuh.cn

[$a, $b] = $arr;
来源：http://hh.nszjky.cn

[U52] PHP：箭头函数
来源：http://no.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://zk.wgjwhj.cn

[U53] PHP：空合并运算符
来源：http://px.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://zd.szsharing.cn

[U54] PHP：空安全调用
来源：http://rx.bookmarksfly.cn

$obj?->method()
来源：http://ts.newstarts.cn

[U55] PHP：match 表达式
来源：http://hq.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://df.jctech888.com.cn

[U56] PHP：命名参数
来源：http://xj.colortex.cn

f(a: 1, b: 2)
来源：http://yw.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://nx.panjiajie.cn

"值: {$a}"
来源：http://db.hnjuh.cn

[U58] PHP：数组三件套
来源：http://tq.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qd.hnjuh.cn

[U59] PHP：自定义排序
来源：http://tr.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pe.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://lh.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bd.gzmigu.cn

[U61] PHP：正则
来源：http://sk.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gp.nicolike.cn

[U62] PHP：日期对象
来源：http://lu.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ec.bjjhwx.cn

[U63] PHP：文件读写
来源：http://eh.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://se.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://gt.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://yj.9csxet.cn

[U65] PHP：会话
来源：http://ar.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mo.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://hs.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ay.shxzukj.cn

[U67] PHP：处理文件上传
来源：http://hg.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gv.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://sb.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xi.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://ee.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vf.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ul.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gy.nszjky.cn

[U71] PHP：抛出异常
来源：http://sn.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://yq.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://pp.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://un.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://hi.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://ip.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://lb.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://qa.shxzukj.cn

[U75] PHP：依赖注入
来源：http://lv.haigaiapp.cn

composer require psr/container
来源：http://yq.yuexingan06.cn

[U76] PHP：简单路由
来源：http://vl.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rr.huanxung.cn

[U77] PHP：模板渲染
来源：http://dh.gzmigu.cn

composer require twig/twig
来源：http://lk.chemitech.net.cn

[U78] PHP：单元测试
来源：http://jf.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://vs.newstarts.cn

[U79] PHP：静态分析
来源：http://gp.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://dz.newstarts.cn

[U80] PHP：代码规范修复
来源：http://jn.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://di.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://lb.521024.cn

npm init -y;  npm i express
来源：http://it.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://mt.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iw.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://xj.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xh.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://ga.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://av.nicolike.cn

[U85] JS：可选链
来源：http://ij.9csxet.cn

a?.b?.c
来源：http://bi.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://hx.jianghongdianzi.cn

a ?? b
来源：http://wp.panjiajie.cn

[U87] JS：解构默认值
来源：http://nt.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://ru.shxzskj.cn

[U88] JS：对象展开合并
来源：http://ax.chemitech.net.cn

{ ...a, ...b }
来源：http://jy.shxzskj.cn

[U89] JS：数组去重
来源：http://aq.hnjuh.cn

[...new Set(arr)]
来源：http://sb.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://hy.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://du.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://jh.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kq.newstarts.cn

[U92] JS：深拷贝
来源：http://ms.shxzukj.cn

structuredClone(obj)
来源：http://ng.hnjuh.cn

[U93] JS：模板字符串
来源：http://kp.nszjky.cn

`共 ${n} 条`
来源：http://ei.yuexingan06.cn

[U94] JS：箭头函数
来源：http://mn.bookmarksfly.cn

const double = x => x * 2;
来源：http://qp.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://up.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://gr.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://vd.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://js.asd995.cn

[U97] JS：并发请求
来源：http://sr.hahajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://wr.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bb.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://zn.newstarts.cn

el.addEventListener("click", e => {})
来源：http://oi.lnxyls.cn

[U100] JS：DOM 查询
来源：http://cp.shxzskj.cn

document.querySelector(".item")
来源：http://fl.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://la.nszjky.cn

el.classList.toggle("active")
来源：http://vq.szxytkj.cn

[U102] JS：本地存储
来源：http://er.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pt.bjjhwx.cn

[U103] JS：定时器
来源：http://bm.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ps.hahajie.cn

[U104] JS：防抖
来源：http://it.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aa.jianghongdianzi.cn

[U105] JS：节流
来源：http://lx.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wv.shxzskj.cn

[U106] JS：日期格式化
来源：http://rf.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ty.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://ve.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://me.shxzukj.cn

[U108] JS：随机整数
来源：http://if.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ef.9csxet.cn

[U109] JS：数组分组
来源：http://wm.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://ho.colortex.cn

[U110] JS：数组分块
来源：http://jx.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ed.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://ae.panjiajie.cn

new Map(Object.entries(obj))
来源：http://vp.colortex.cn

[U112] JS：字符串补位
来源：http://dw.newstarts.cn

"7".padStart(3, "0")
来源：http://ws.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://wv.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://rf.asd995.cn

[U114] JS：JSON 深比较
来源：http://dq.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ur.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://lp.jctech888.com.cn

crypto.randomUUID()
来源：http://xo.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://jz.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://lm.haigaiapp.cn

[U117] JS：单元测试
来源：http://vv.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://hd.lnxyls.cn

[U118] JS：开发服务器
来源：http://kl.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://gk.shxzukj.cn

[U119] JS：生产构建
来源：http://or.szxytkj.cn

npx vite build
来源：http://nu.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://xq.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://tl.asd995.cn

================================================================================
来源：http://zn.9csxet.cn

统计汇总
来源：http://lp.nszjky.cn

================================================================================
来源：http://jt.colortex.cn

按语言统计（条）：
来源：http://bw.521024.cn

Python ......... 252
来源：http://vd.lnxyls.cn

PHP ............ 252
来源：http://ij.haigaiapp.cn

JavaScript ..... 252
来源：http://mu.huanxung.cn

TypeScript ..... 212
来源：http://qs.asd995.cn

Java ........... 212
来源：http://ul.huixiangedu.cn

Go ............. 212
来源：http://xo.nszjky.cn

Ruby ........... 212
来源：http://jj.nicolike.cn

C# ............. 212
来源：http://mg.wgjwhj.cn

C .............. 30
来源：http://ls.haigaiapp.cn

C++ ............ 30
来源：http://ef.nszjky.cn

SQL ............ 90
来源：http://pn.nszjky.cn

Bash ........... 80
来源：http://nk.yuexingan06.cn

Kotlin ......... 15
来源：http://yu.wgjwhj.cn

Swift .......... 15
来源：http://rt.asd995.cn

Lua ............ 10
来源：http://ph.muxihuayi.cn

Perl ........... 10
来源：http://sm.lnxyls.cn

Scala .......... 10
来源：http://oy.newstarts.cn

------------------------------------
来源：http://yz.haigaiapp.cn

合计 ........... 2106 条
来源：http://mf.bjjhwx.cn

按章节统计：
来源：http://cv.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dj.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qn.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qc.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://td.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aj.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://as.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jh.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://te.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qk.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yp.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gi.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fj.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wr.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://de.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://km.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xh.hahajie.cn

Q SQL 专题                              90
来源：http://fu.bookmarksfly.cn

R Bash 专题                             80
来源：http://oq.colortex.cn

S C / C++ 专题                          60
来源：http://zj.huixiangedu.cn

T 其他语言补充                          60
来源：http://xd.521024.cn

U 高频实用片段                         120
来源：http://hi.szxytkj.cn

------------------------------------
来源：http://gw.gzmigu.cn

合计                                  2106 条
来源：http://cs.newstarts.cn

--------------------------------------------------------------------------------
来源：http://dh.yuexingan06.cn

使用提醒
来源：http://ox.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://vd.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rp.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://na.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mn.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ik.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wf.521024.cn

—— 文件结束 ——
来源：http://js.asd995.cn

================================================================================
来源：http://xj.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ux.newstarts.cn

Common Programming Examples Cheat Book
来源：http://wf.asd995.cn

================================================================================
来源：http://if.chemitech.net.cn

【收录内容】
来源：http://kv.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vz.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aj.shxzukj.cn

SQL · Bash · C · C++
来源：http://pn.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xx.szxytkj.cn

【使用说明】
来源：http://en.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ao.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hm.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fe.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kv.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://es.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bv.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qo.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zu.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ej.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://md.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tk.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ql.jctech888.com.cn

【文件统计】
来源：http://lk.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tp.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://xo.521024.cn

目  录
来源：http://aq.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://sw.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://on.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lc.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jd.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ax.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nk.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nz.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mg.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ds.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qh.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qe.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oj.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xe.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sk.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kp.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cc.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mw.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tp.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ix.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tf.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fp.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tl.yuntaijiaju.cn

================================================================================
来源：http://gg.yuntaijiaju.cn

A. 基础语法与类型
来源：http://wz.hahajie.cn

================================================================================
来源：http://zw.newstarts.cn

[A01] Hello World
来源：http://tj.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://ld.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://hb.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://pv.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ss.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://ed.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://rn.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://op.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vs.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://jh.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lo.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yc.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://as.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rl.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://jk.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://jd.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://ry.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rs.hahajie.cn

[A03] 常量定义
来源：http://os.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sy.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://nn.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ca.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://rc.asd995.cn

Java: static final double PI = 3.14159;
来源：http://av.asd995.cn

Go:   const PI = 3.14159
来源：http://dp.521024.cn


<!-- 参考信息 -->