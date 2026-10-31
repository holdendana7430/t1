代发 wailian999

[U35] Py：发送邮件
来源：http://xg.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fm.nicolike.cn

[U36] Py：定时任务
来源：http://lw.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://jc.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://fe.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ko.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://yw.nszjky.cn

Path(__file__).resolve().parent
来源：http://bi.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://rw.lnxyls.cn

sys.stdout.isatty()
来源：http://xs.9csxet.cn

[U40] Py：打印到标准错误
来源：http://gx.szsharing.cn

print("err", file=sys.stderr)
来源：http://tt.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://sp.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fe.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://pd.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kh.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://mm.asd995.cn

namespace App\Http;
来源：http://jk.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://gf.jianghongdianzi.cn

declare(strict_types=1);
来源：http://wt.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://sn.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://if.521024.cn

[U46] PHP：可空类型
来源：http://no.huanxung.cn

?string $name = null
来源：http://ji.szsharing.cn

[U47] PHP：联合类型
来源：http://ms.shxzskj.cn

int|string $id
来源：http://tv.asd995.cn

[U48] PHP：纯枚举
来源：http://vv.shxzukj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jc.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ni.nicolike.cn

public readonly string $name
来源：http://oo.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://jv.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://xj.huanxung.cn

[U51] PHP：数组解构
来源：http://lt.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://ml.9csxet.cn

[U52] PHP：箭头函数
来源：http://il.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://wo.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://xe.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://fd.colortex.cn

[U54] PHP：空安全调用
来源：http://en.bookmarksfly.cn

$obj?->method()
来源：http://ju.szxytkj.cn

[U55] PHP：match 表达式
来源：http://zx.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yv.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://un.521024.cn

f(a: 1, b: 2)
来源：http://gg.521024.cn

[U57] PHP：字符串插值
来源：http://kr.asd995.cn

"值: {$a}"
来源：http://tv.asd995.cn

[U58] PHP：数组三件套
来源：http://fk.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://do.newstarts.cn

[U59] PHP：自定义排序
来源：http://vv.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tn.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://pe.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nc.colortex.cn

[U61] PHP：正则
来源：http://ri.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gm.panjiajie.cn

[U62] PHP：日期对象
来源：http://dk.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vf.colortex.cn

[U63] PHP：文件读写
来源：http://rb.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xq.hahajie.cn

[U64] PHP：目录遍历
来源：http://va.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://gp.szsharing.cn

[U65] PHP：会话
来源：http://hn.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jk.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://sr.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ls.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://ut.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fo.hahajie.cn

[U68] PHP：PDO 连接
来源：http://pu.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ed.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://te.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sd.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://ng.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pv.hnjuh.cn

[U71] PHP：抛出异常
来源：http://vj.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://wh.lnxyls.cn

[U72] PHP：写错误日志
来源：http://fw.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://mg.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://te.asd995.cn

parse_ini_file("config.ini", true)
来源：http://vb.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://jy.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://lu.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://at.huixiangedu.cn

composer require psr/container
来源：http://er.nicolike.cn

[U76] PHP：简单路由
来源：http://nv.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eh.shxzukj.cn

[U77] PHP：模板渲染
来源：http://yq.wgjwhj.cn

composer require twig/twig
来源：http://de.hahajie.cn

[U78] PHP：单元测试
来源：http://eb.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://do.wgjwhj.cn

[U79] PHP：静态分析
来源：http://co.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://ji.huanxung.cn

[U80] PHP：代码规范修复
来源：http://mh.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xe.panjiajie.cn

[U81] JS：初始化项目
来源：http://sj.szxytkj.cn

npm init -y;  npm i express
来源：http://df.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://oz.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ba.521024.cn

[U83] JS：ES Module 导入导出
来源：http://nk.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zv.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://fn.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yx.szsharing.cn

[U85] JS：可选链
来源：http://jb.jctech888.com.cn

a?.b?.c
来源：http://er.521024.cn

[U86] JS：空值合并
来源：http://sv.colortex.cn

a ?? b
来源：http://zp.nicolike.cn

[U87] JS：解构默认值
来源：http://yr.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://hp.huanxung.cn

[U88] JS：对象展开合并
来源：http://ha.newstarts.cn

{ ...a, ...b }
来源：http://zt.panjiajie.cn

[U89] JS：数组去重
来源：http://zo.hnjuh.cn

[...new Set(arr)]
来源：http://bg.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ws.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://fb.nszjky.cn

[U91] JS：对象键值遍历
来源：http://ct.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xl.shtwfgs.cn

[U92] JS：深拷贝
来源：http://dl.jctech888.com.cn

structuredClone(obj)
来源：http://xe.muxihuayi.cn

[U93] JS：模板字符串
来源：http://pa.shtwfgs.cn

`共 ${n} 条`
来源：http://ws.asd995.cn

[U94] JS：箭头函数
来源：http://ps.wgjwhj.cn

const double = x => x * 2;
来源：http://qq.panjiajie.cn

[U95] JS：Promise 包装
来源：http://eg.asd995.cn

new Promise((resolve, reject) => {})
来源：http://au.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ee.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ch.chemitech.net.cn

[U97] JS：并发请求
来源：http://gz.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tn.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://wm.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jd.shtwfgs.cn

[U99] JS：事件监听
来源：http://ga.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://iu.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://bw.shxzskj.cn

document.querySelector(".item")
来源：http://tu.lnxyls.cn

[U101] JS：classList 操作
来源：http://ik.newstarts.cn

el.classList.toggle("active")
来源：http://nk.nicolike.cn

[U102] JS：本地存储
来源：http://wb.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rv.jctech888.com.cn

[U103] JS：定时器
来源：http://cq.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://om.nszjky.cn

[U104] JS：防抖
来源：http://nd.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tn.shtwfgs.cn

[U105] JS：节流
来源：http://ck.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gn.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://dk.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ya.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://fx.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uw.gzmigu.cn

[U108] JS：随机整数
来源：http://gs.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yg.nicolike.cn

[U109] JS：数组分组
来源：http://iq.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://yf.521024.cn

[U110] JS：数组分块
来源：http://oo.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lj.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://my.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://hx.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://yb.muxihuayi.cn

"7".padStart(3, "0")
来源：http://oy.lnxyls.cn

[U113] JS：正则替换全部
来源：http://va.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://ed.nicolike.cn

[U114] JS：JSON 深比较
来源：http://pn.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ji.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://cw.colortex.cn

crypto.randomUUID()
来源：http://xi.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://tq.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://qq.szxytkj.cn

[U117] JS：单元测试
来源：http://ie.521024.cn

npm i -D vitest;  npx vitest
来源：http://mk.huixiangedu.cn

[U118] JS：开发服务器
来源：http://xm.hnjuh.cn

npm i -D vite;  npx vite
来源：http://bz.shxzukj.cn

[U119] JS：生产构建
来源：http://jm.szxytkj.cn

npx vite build
来源：http://oc.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://vz.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://by.nszjky.cn

================================================================================
来源：http://vu.nszjky.cn

统计汇总
来源：http://bj.521024.cn

================================================================================
来源：http://cp.panjiajie.cn

按语言统计（条）：
来源：http://dv.huixinmuqiang.cn

Python ......... 252
来源：http://yk.szsharing.cn

PHP ............ 252
来源：http://lq.gzmigu.cn

JavaScript ..... 252
来源：http://sm.jctech888.com.cn

TypeScript ..... 212
来源：http://ka.chemitech.net.cn

Java ........... 212
来源：http://fy.haigaiapp.cn

Go ............. 212
来源：http://uc.yuntaijiaju.cn

Ruby ........... 212
来源：http://hi.huanxung.cn

C# ............. 212
来源：http://cq.gzmigu.cn

C .............. 30
来源：http://hj.yuntaijiaju.cn

C++ ............ 30
来源：http://fi.nicolike.cn

SQL ............ 90
来源：http://fp.haigaiapp.cn

Bash ........... 80
来源：http://js.hahajie.cn

Kotlin ......... 15
来源：http://rk.nszjky.cn

Swift .......... 15
来源：http://go.lnxyls.cn

Lua ............ 10
来源：http://iv.9csxet.cn

Perl ........... 10
来源：http://pi.szsharing.cn

Scala .......... 10
来源：http://lv.szsharing.cn

------------------------------------
来源：http://jf.asd995.cn

合计 ........... 2106 条
来源：http://ky.shxzukj.cn

按章节统计：
来源：http://rq.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oz.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://da.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ly.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cq.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xo.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ss.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iy.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eb.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yg.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gj.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qz.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kt.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://if.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fn.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ti.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lq.yuexingan06.cn

Q SQL 专题                              90
来源：http://fh.colortex.cn

R Bash 专题                             80
来源：http://ge.hnjuh.cn

S C / C++ 专题                          60
来源：http://jf.shxzukj.cn

T 其他语言补充                          60
来源：http://fd.shxzskj.cn

U 高频实用片段                         120
来源：http://mv.huixiangedu.cn

------------------------------------
来源：http://pg.asd995.cn

合计                                  2106 条
来源：http://lp.colortex.cn

--------------------------------------------------------------------------------
来源：http://mp.szsharing.cn

使用提醒
来源：http://zz.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://mw.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ax.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wa.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yh.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vu.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ry.nicolike.cn

—— 文件结束 ——
来源：http://cy.shxzukj.cn

================================================================================
来源：http://jw.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://ui.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://zj.jianghongdianzi.cn

================================================================================
来源：http://pd.newstarts.cn

【收录内容】
来源：http://yl.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sw.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ap.szsharing.cn

SQL · Bash · C · C++
来源：http://py.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ko.haigaiapp.cn

【使用说明】
来源：http://hb.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fv.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zj.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cz.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wt.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://um.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xf.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hb.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vp.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uu.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qt.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qa.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lp.yuexingan06.cn

【文件统计】
来源：http://od.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ho.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ym.muxihuayi.cn

目  录
来源：http://vk.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://tp.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mk.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ro.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hj.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gp.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://an.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kz.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rd.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ix.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vj.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ac.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gx.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://as.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nv.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vo.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xn.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sq.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rj.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vr.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cj.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gp.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cx.huanxung.cn

================================================================================
来源：http://sl.muxihuayi.cn

A. 基础语法与类型
来源：http://bt.haigaiapp.cn

================================================================================
来源：http://pb.lnxyls.cn

[A01] Hello World
来源：http://xc.huanxung.cn

Py:   print("Hello, World!")
来源：http://is.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://ip.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://ur.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wf.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://ei.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://lk.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://br.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gt.panjiajie.cn

[A02] 变量声明与赋值
来源：http://kn.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gm.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tl.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dr.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vl.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://kn.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://ce.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://zi.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bq.jianghongdianzi.cn

[A03] 常量定义
来源：http://jm.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mf.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://jn.muxihuayi.cn


<!-- 参考信息 -->