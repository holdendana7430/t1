代发 wailian999

[U37] Py：读写 Excel
来源：http://uc.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ym.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://el.shxzskj.cn

Path(__file__).resolve().parent
来源：http://ih.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://kg.nszjky.cn

sys.stdout.isatty()
来源：http://zf.nszjky.cn

[U40] Py：打印到标准错误
来源：http://tc.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://tc.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://so.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gu.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://hr.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vc.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://da.huixiangedu.cn

namespace App\Http;
来源：http://nf.szsharing.cn

[U44] PHP：开启严格类型
来源：http://ub.bookmarksfly.cn

declare(strict_types=1);
来源：http://ig.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://pc.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.asd995.cn

[U46] PHP：可空类型
来源：http://fv.huixiangedu.cn

?string $name = null
来源：http://kl.521024.cn

[U47] PHP：联合类型
来源：http://uv.wgjwhj.cn

int|string $id
来源：http://bl.nszjky.cn

[U48] PHP：纯枚举
来源：http://us.bookmarksfly.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lo.jctech888.com.cn

[U49] PHP：只读属性
来源：http://lt.lnxyls.cn

public readonly string $name
来源：http://qo.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://vz.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://aq.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://ud.chemitech.net.cn

[$a, $b] = $arr;
来源：http://nz.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://yn.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://rt.huanxung.cn

[U53] PHP：空合并运算符
来源：http://jo.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://bq.nszjky.cn

[U54] PHP：空安全调用
来源：http://ys.nszjky.cn

$obj?->method()
来源：http://em.szsharing.cn

[U55] PHP：match 表达式
来源：http://kq.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qi.huixiangedu.cn

[U56] PHP：命名参数
来源：http://pr.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://bp.hahajie.cn

[U57] PHP：字符串插值
来源：http://wg.muxihuayi.cn

"值: {$a}"
来源：http://dx.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://wb.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ow.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://sj.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yl.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://ud.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wp.chemitech.net.cn

[U61] PHP：正则
来源：http://kq.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wk.521024.cn

[U62] PHP：日期对象
来源：http://mh.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://et.yuexingan06.cn

[U63] PHP：文件读写
来源：http://ap.huixinmuqiang.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://co.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://ml.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kz.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ck.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lh.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://pc.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tp.hahajie.cn

[U67] PHP：处理文件上传
来源：http://gl.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://we.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://df.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cg.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://vj.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fx.newstarts.cn

[U70] PHP：PDO 事务
来源：http://dw.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bi.gzmigu.cn

[U71] PHP：抛出异常
来源：http://rg.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://zo.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://yi.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://pg.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://df.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://vc.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://qr.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://sl.huanxung.cn

[U75] PHP：依赖注入
来源：http://lx.shtwfgs.cn

composer require psr/container
来源：http://gi.shtwfgs.cn

[U76] PHP：简单路由
来源：http://qn.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bf.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ly.hnjuh.cn

composer require twig/twig
来源：http://uw.nicolike.cn

[U78] PHP：单元测试
来源：http://pw.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://cl.nicolike.cn

[U79] PHP：静态分析
来源：http://de.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ox.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://uk.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qu.huanxung.cn

[U81] JS：初始化项目
来源：http://iq.huanxung.cn

npm init -y;  npm i express
来源：http://rl.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://fz.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xo.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://ga.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ta.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://pd.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wf.shtwfgs.cn

[U85] JS：可选链
来源：http://op.yuexingan06.cn

a?.b?.c
来源：http://yy.hnjuh.cn

[U86] JS：空值合并
来源：http://dk.nicolike.cn

a ?? b
来源：http://yl.wgjwhj.cn

[U87] JS：解构默认值
来源：http://dq.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://ya.panjiajie.cn

[U88] JS：对象展开合并
来源：http://gv.shxzskj.cn

{ ...a, ...b }
来源：http://sa.colortex.cn

[U89] JS：数组去重
来源：http://ue.9csxet.cn

[...new Set(arr)]
来源：http://dv.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://xv.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://rv.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://sn.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ba.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://no.9csxet.cn

structuredClone(obj)
来源：http://om.yuexingan06.cn

[U93] JS：模板字符串
来源：http://xa.haigaiapp.cn

`共 ${n} 条`
来源：http://ce.521024.cn

[U94] JS：箭头函数
来源：http://gt.szsharing.cn

const double = x => x * 2;
来源：http://hs.shxzukj.cn

[U95] JS：Promise 包装
来源：http://la.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://vb.521024.cn

[U96] JS：async/await 与异常
来源：http://qc.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cx.wgjwhj.cn

[U97] JS：并发请求
来源：http://lt.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://xu.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ja.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://qo.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://fv.panjiajie.cn

[U100] JS：DOM 查询
来源：http://rf.chemitech.net.cn

document.querySelector(".item")
来源：http://ig.muxihuayi.cn

[U101] JS：classList 操作
来源：http://gb.521024.cn

el.classList.toggle("active")
来源：http://sv.shxzskj.cn

[U102] JS：本地存储
来源：http://rn.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vn.bjjhwx.cn

[U103] JS：定时器
来源：http://ea.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sk.521024.cn

[U104] JS：防抖
来源：http://kc.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ef.yuntaijiaju.cn

[U105] JS：节流
来源：http://kk.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vf.huanxung.cn

[U106] JS：日期格式化
来源：http://yn.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sa.panjiajie.cn

[U107] JS：数字千分位
来源：http://zi.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://af.521024.cn

[U108] JS：随机整数
来源：http://ql.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xl.hnjuh.cn

[U109] JS：数组分组
来源：http://wk.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://jf.chemitech.net.cn

[U110] JS：数组分块
来源：http://jj.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gh.newstarts.cn

[U111] JS：对象转 Map
来源：http://vf.newstarts.cn

new Map(Object.entries(obj))
来源：http://xn.newstarts.cn

[U112] JS：字符串补位
来源：http://ey.haigaiapp.cn

"7".padStart(3, "0")
来源：http://pl.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://ek.szxytkj.cn

s.replaceAll("a", "b")
来源：http://vq.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://iv.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://io.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://te.chemitech.net.cn

crypto.randomUUID()
来源：http://bm.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://bf.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://us.bjjhwx.cn

[U117] JS：单元测试
来源：http://wj.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://ps.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://sa.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://pi.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://gi.panjiajie.cn

npx vite build
来源：http://ht.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ux.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://tn.hahajie.cn

================================================================================
来源：http://jw.521024.cn

统计汇总
来源：http://xf.nszjky.cn

================================================================================
来源：http://bj.wgjwhj.cn

按语言统计（条）：
来源：http://eo.9csxet.cn

Python ......... 252
来源：http://un.huixinmuqiang.cn

PHP ............ 252
来源：http://gh.jctech888.com.cn

JavaScript ..... 252
来源：http://iw.hahajie.cn

TypeScript ..... 212
来源：http://qs.gzmigu.cn

Java ........... 212
来源：http://zd.9csxet.cn

Go ............. 212
来源：http://dq.huixinmuqiang.cn

Ruby ........... 212
来源：http://ql.shxzskj.cn

C# ............. 212
来源：http://tc.hahajie.cn

C .............. 30
来源：http://qb.newstarts.cn

C++ ............ 30
来源：http://ps.gzmigu.cn

SQL ............ 90
来源：http://qj.chemitech.net.cn

Bash ........... 80
来源：http://bs.yuexingan06.cn

Kotlin ......... 15
来源：http://dr.chemitech.net.cn

Swift .......... 15
来源：http://nx.szsharing.cn

Lua ............ 10
来源：http://wd.bookmarksfly.cn

Perl ........... 10
来源：http://ah.panjiajie.cn

Scala .......... 10
来源：http://jt.521024.cn

------------------------------------
来源：http://nw.newstarts.cn

合计 ........... 2106 条
来源：http://sb.9csxet.cn

按章节统计：
来源：http://lp.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sd.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cz.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fy.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ik.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pu.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mx.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://if.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nw.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wt.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cr.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ty.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://th.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dm.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fk.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bb.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://os.muxihuayi.cn

Q SQL 专题                              90
来源：http://we.nicolike.cn

R Bash 专题                             80
来源：http://bx.shtwfgs.cn

S C / C++ 专题                          60
来源：http://iv.huanxung.cn

T 其他语言补充                          60
来源：http://wt.bjjhwx.cn

U 高频实用片段                         120
来源：http://ti.jctech888.com.cn

------------------------------------
来源：http://kn.nszjky.cn

合计                                  2106 条
来源：http://ru.521024.cn

--------------------------------------------------------------------------------
来源：http://sl.shxzukj.cn

使用提醒
来源：http://ss.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ga.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ra.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bi.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xg.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eq.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://co.yuntaijiaju.cn

—— 文件结束 ——
来源：http://jk.nicolike.cn

================================================================================
来源：http://yl.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://tc.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://ml.colortex.cn

================================================================================
来源：http://fz.szxytkj.cn

【收录内容】
来源：http://xs.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sq.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pc.newstarts.cn

SQL · Bash · C · C++
来源：http://va.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jc.haigaiapp.cn

【使用说明】
来源：http://tf.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://us.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://na.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ys.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fp.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vo.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iv.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rx.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sv.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hv.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ej.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ws.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xk.jctech888.com.cn

【文件统计】
来源：http://pp.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://or.nicolike.cn

--------------------------------------------------------------------------------
来源：http://de.shxzskj.cn

目  录
来源：http://xx.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://wq.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xx.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xd.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vh.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wp.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ng.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zb.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zb.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fn.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://do.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eg.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zn.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bb.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vh.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tt.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lm.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mk.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fo.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xv.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rz.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rj.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dt.shxzskj.cn

================================================================================
来源：http://zj.newstarts.cn

A. 基础语法与类型
来源：http://yy.huanxung.cn

================================================================================
来源：http://hp.asd995.cn

[A01] Hello World
来源：http://sk.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://kt.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://vh.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://hl.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aa.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://vu.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://ej.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://te.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xc.szsharing.cn

[A02] 变量声明与赋值
来源：http://ig.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ji.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ox.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yg.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bq.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://ep.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://rl.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://lo.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://er.nicolike.cn

[A03] 常量定义
来源：http://ss.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tc.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://ry.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://nx.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://sg.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://jc.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://ou.szsharing.cn


<!-- 参考信息 -->