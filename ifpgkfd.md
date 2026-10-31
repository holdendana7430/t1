代发 wailian999

[U37] Py：读写 Excel
来源：http://sz.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ux.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://xk.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://vw.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ee.chemitech.net.cn

sys.stdout.isatty()
来源：http://me.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://ut.asd995.cn

print("err", file=sys.stderr)
来源：http://vm.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ay.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cr.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://ae.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ue.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://lu.huanxung.cn

namespace App\Http;
来源：http://rt.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://vu.shxzskj.cn

declare(strict_types=1);
来源：http://eo.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://pk.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pz.chemitech.net.cn

[U46] PHP：可空类型
来源：http://of.nicolike.cn

?string $name = null
来源：http://ye.hahajie.cn

[U47] PHP：联合类型
来源：http://gl.panjiajie.cn

int|string $id
来源：http://ce.panjiajie.cn

[U48] PHP：纯枚举
来源：http://yf.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tb.hnjuh.cn

[U49] PHP：只读属性
来源：http://gh.shtwfgs.cn

public readonly string $name
来源：http://ak.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://go.nicolike.cn

public function __construct(private int $id) {}
来源：http://er.szxytkj.cn

[U51] PHP：数组解构
来源：http://ls.newstarts.cn

[$a, $b] = $arr;
来源：http://gj.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://og.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://mh.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://jp.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://hg.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://sr.9csxet.cn

$obj?->method()
来源：http://kh.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://vj.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ch.haigaiapp.cn

[U56] PHP：命名参数
来源：http://rm.shtwfgs.cn

f(a: 1, b: 2)
来源：http://tq.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://br.wgjwhj.cn

"值: {$a}"
来源：http://fm.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://ve.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qg.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://va.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://qq.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eb.shtwfgs.cn

[U61] PHP：正则
来源：http://bq.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mr.shxzskj.cn

[U62] PHP：日期对象
来源：http://zu.shxzskj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hr.huanxung.cn

[U63] PHP：文件读写
来源：http://nw.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://md.hnjuh.cn

[U64] PHP：目录遍历
来源：http://tb.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://bl.hnjuh.cn

[U65] PHP：会话
来源：http://aj.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ws.asd995.cn

[U66] PHP：设置 Cookie
来源：http://br.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://co.asd995.cn

[U67] PHP：处理文件上传
来源：http://vc.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qs.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://lk.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ca.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://dw.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qu.asd995.cn

[U70] PHP：PDO 事务
来源：http://wi.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sr.shxzukj.cn

[U71] PHP：抛出异常
来源：http://um.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://cw.nszjky.cn

[U72] PHP：写错误日志
来源：http://xj.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://mi.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://ls.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ai.shxzukj.cn

[U74] PHP：读取环境变量
来源：http://hv.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://uo.hnjuh.cn

[U75] PHP：依赖注入
来源：http://yj.asd995.cn

composer require psr/container
来源：http://yf.9csxet.cn

[U76] PHP：简单路由
来源：http://fp.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qs.shxzukj.cn

[U77] PHP：模板渲染
来源：http://zx.bookmarksfly.cn

composer require twig/twig
来源：http://wj.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://jf.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://js.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ro.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://jg.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://wa.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://by.9csxet.cn

[U81] JS：初始化项目
来源：http://kt.jctech888.com.cn

npm init -y;  npm i express
来源：http://ww.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://pi.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hx.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://ga.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ju.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://tc.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nh.shxzukj.cn

[U85] JS：可选链
来源：http://ok.shxzukj.cn

a?.b?.c
来源：http://fn.huixiangedu.cn

[U86] JS：空值合并
来源：http://wr.panjiajie.cn

a ?? b
来源：http://xk.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://az.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://vp.newstarts.cn

[U88] JS：对象展开合并
来源：http://du.jianghongdianzi.cn

{ ...a, ...b }
来源：http://rv.colortex.cn

[U89] JS：数组去重
来源：http://ei.haigaiapp.cn

[...new Set(arr)]
来源：http://vo.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://vu.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://rq.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://md.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jr.gzmigu.cn

[U92] JS：深拷贝
来源：http://ox.shxzukj.cn

structuredClone(obj)
来源：http://hh.nicolike.cn

[U93] JS：模板字符串
来源：http://jk.bookmarksfly.cn

`共 ${n} 条`
来源：http://bh.colortex.cn

[U94] JS：箭头函数
来源：http://hh.nszjky.cn

const double = x => x * 2;
来源：http://js.colortex.cn

[U95] JS：Promise 包装
来源：http://ve.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://ic.szsharing.cn

[U96] JS：async/await 与异常
来源：http://rh.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qc.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://um.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://lw.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mp.bjjhwx.cn

[U99] JS：事件监听
来源：http://at.nszjky.cn

el.addEventListener("click", e => {})
来源：http://tm.szxytkj.cn

[U100] JS：DOM 查询
来源：http://oj.bjjhwx.cn

document.querySelector(".item")
来源：http://kn.szsharing.cn

[U101] JS：classList 操作
来源：http://lp.hahajie.cn

el.classList.toggle("active")
来源：http://xj.shtwfgs.cn

[U102] JS：本地存储
来源：http://se.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nm.bookmarksfly.cn

[U103] JS：定时器
来源：http://ih.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fq.panjiajie.cn

[U104] JS：防抖
来源：http://yc.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fu.shtwfgs.cn

[U105] JS：节流
来源：http://ea.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wj.asd995.cn

[U106] JS：日期格式化
来源：http://ms.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xc.wgjwhj.cn

[U107] JS：数字千分位
来源：http://ta.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.9csxet.cn

[U108] JS：随机整数
来源：http://rm.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uz.newstarts.cn

[U109] JS：数组分组
来源：http://ss.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://sj.muxihuayi.cn

[U110] JS：数组分块
来源：http://dl.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vb.colortex.cn

[U111] JS：对象转 Map
来源：http://zj.hahajie.cn

new Map(Object.entries(obj))
来源：http://sv.jctech888.com.cn

[U112] JS：字符串补位
来源：http://uh.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://jt.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://qj.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://jx.asd995.cn

[U114] JS：JSON 深比较
来源：http://im.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://st.colortex.cn

[U115] JS：生成 UUID
来源：http://ec.yuexingan06.cn

crypto.randomUUID()
来源：http://iz.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://zs.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://ax.asd995.cn

[U117] JS：单元测试
来源：http://me.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://sx.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://vz.szsharing.cn

npm i -D vite;  npx vite
来源：http://ct.jctech888.com.cn

[U119] JS：生产构建
来源：http://pe.huixiangedu.cn

npx vite build
来源：http://vz.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://cr.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://aj.colortex.cn

================================================================================
来源：http://qr.shxzukj.cn

统计汇总
来源：http://xj.huanxung.cn

================================================================================
来源：http://py.bjjhwx.cn

按语言统计（条）：
来源：http://rk.9csxet.cn

Python ......... 252
来源：http://gx.chemitech.net.cn

PHP ............ 252
来源：http://kk.szsharing.cn

JavaScript ..... 252
来源：http://uw.9csxet.cn

TypeScript ..... 212
来源：http://on.bjjhwx.cn

Java ........... 212
来源：http://co.yuntaijiaju.cn

Go ............. 212
来源：http://vc.yuexingan06.cn

Ruby ........... 212
来源：http://wb.gzmigu.cn

C# ............. 212
来源：http://go.shtwfgs.cn

C .............. 30
来源：http://rp.colortex.cn

C++ ............ 30
来源：http://ai.shtwfgs.cn

SQL ............ 90
来源：http://gn.lnxyls.cn

Bash ........... 80
来源：http://ff.haigaiapp.cn

Kotlin ......... 15
来源：http://zx.muxihuayi.cn

Swift .......... 15
来源：http://yx.huixiangedu.cn

Lua ............ 10
来源：http://sp.jctech888.com.cn

Perl ........... 10
来源：http://we.shxzskj.cn

Scala .......... 10
来源：http://rr.muxihuayi.cn

------------------------------------
来源：http://rj.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://nu.shxzukj.cn

按章节统计：
来源：http://ik.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lb.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://za.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rz.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rl.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kc.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ix.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ed.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wr.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ii.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lb.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mh.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wv.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uv.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ce.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pr.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qa.yuexingan06.cn

Q SQL 专题                              90
来源：http://kq.lnxyls.cn

R Bash 专题                             80
来源：http://md.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://af.newstarts.cn

T 其他语言补充                          60
来源：http://ze.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://it.521024.cn

------------------------------------
来源：http://of.jianghongdianzi.cn

合计                                  2106 条
来源：http://kc.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://xt.newstarts.cn

使用提醒
来源：http://gi.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dm.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hk.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wu.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lf.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vk.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fr.yuexingan06.cn

—— 文件结束 ——
来源：http://en.huixinmuqiang.cn

================================================================================
来源：http://en.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://yq.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://fd.jianghongdianzi.cn

================================================================================
来源：http://zv.szsharing.cn

【收录内容】
来源：http://fo.szxytkj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cr.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wr.jctech888.com.cn

SQL · Bash · C · C++
来源：http://xd.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xh.huanxung.cn

【使用说明】
来源：http://kb.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ck.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hd.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gg.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ny.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aw.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ny.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ii.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rj.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yl.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xh.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://an.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xj.panjiajie.cn

【文件统计】
来源：http://ap.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rs.huanxung.cn

--------------------------------------------------------------------------------
来源：http://vj.colortex.cn

目  录
来源：http://yh.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ct.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hf.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wn.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ei.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ou.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ia.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xo.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ma.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ts.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ev.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hk.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rv.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zk.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://za.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yg.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vs.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qs.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mo.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gv.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vc.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wc.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rt.gzmigu.cn

================================================================================
来源：http://ub.jctech888.com.cn

A. 基础语法与类型
来源：http://fo.bookmarksfly.cn

================================================================================
来源：http://ra.shxzskj.cn

[A01] Hello World
来源：http://gz.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://kw.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://pf.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://tg.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://us.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://xw.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://hg.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://hs.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ge.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://bd.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fz.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fw.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qo.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bf.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://py.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://me.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://cp.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ry.521024.cn

[A03] 常量定义
来源：http://oy.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ri.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://gh.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://jr.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://kj.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://zd.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://rs.shxzskj.cn


<!-- 参考信息 -->