代发 wailian999

[U33] Py：打包发布
来源：http://pd.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://sy.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://ce.bookmarksfly.cn

chardet.detect(raw)
来源：http://mk.hnjuh.cn

[U35] Py：发送邮件
来源：http://yp.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ix.panjiajie.cn

[U36] Py：定时任务
来源：http://po.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://ol.asd995.cn

[U37] Py：读写 Excel
来源：http://gb.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://le.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://wq.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://kn.521024.cn

[U39] Py：判断是否在交互环境
来源：http://xc.panjiajie.cn

sys.stdout.isatty()
来源：http://mt.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ui.gzmigu.cn

print("err", file=sys.stderr)
来源：http://kr.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ps.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bc.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://eb.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gd.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://lt.bjjhwx.cn

namespace App\Http;
来源：http://qr.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://rj.yuexingan06.cn

declare(strict_types=1);
来源：http://we.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://lt.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ty.521024.cn

[U46] PHP：可空类型
来源：http://qh.hahajie.cn

?string $name = null
来源：http://mb.lnxyls.cn

[U47] PHP：联合类型
来源：http://fi.szsharing.cn

int|string $id
来源：http://fu.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://ik.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qx.asd995.cn

[U49] PHP：只读属性
来源：http://za.panjiajie.cn

public readonly string $name
来源：http://zw.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://dp.9csxet.cn

public function __construct(private int $id) {}
来源：http://uz.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ip.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://sa.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://ii.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://yx.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://xb.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://cf.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://zf.colortex.cn

$obj?->method()
来源：http://mh.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://mp.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hw.shxzukj.cn

[U56] PHP：命名参数
来源：http://kb.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ll.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://ts.colortex.cn

"值: {$a}"
来源：http://cf.9csxet.cn

[U58] PHP：数组三件套
来源：http://ib.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gu.shxzukj.cn

[U59] PHP：自定义排序
来源：http://rj.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oe.colortex.cn

[U60] PHP：JSON 编解码
来源：http://pk.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://om.9csxet.cn

[U61] PHP：正则
来源：http://km.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rg.huanxung.cn

[U62] PHP：日期对象
来源：http://lq.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vu.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://fm.wgjwhj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bj.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://sp.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ci.jianghongdianzi.cn

[U65] PHP：会话
来源：http://cq.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ho.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://ys.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wr.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://qb.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://su.asd995.cn

[U68] PHP：PDO 连接
来源：http://lc.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vb.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://zl.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gh.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://wi.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qv.hnjuh.cn

[U71] PHP：抛出异常
来源：http://wu.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://gz.panjiajie.cn

[U72] PHP：写错误日志
来源：http://mb.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://cj.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://ge.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://al.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://ex.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://sp.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://jg.panjiajie.cn

composer require psr/container
来源：http://ec.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://bb.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ft.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://on.jctech888.com.cn

composer require twig/twig
来源：http://ry.chemitech.net.cn

[U78] PHP：单元测试
来源：http://uu.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://mf.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://ud.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://bg.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://ek.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aa.bjjhwx.cn

[U81] JS：初始化项目
来源：http://xm.nicolike.cn

npm init -y;  npm i express
来源：http://en.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://nt.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bp.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://kz.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mu.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://ty.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://po.huixinmuqiang.cn

[U85] JS：可选链
来源：http://av.wgjwhj.cn

a?.b?.c
来源：http://bq.lnxyls.cn

[U86] JS：空值合并
来源：http://te.shxzukj.cn

a ?? b
来源：http://io.9csxet.cn

[U87] JS：解构默认值
来源：http://zf.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://jn.szsharing.cn

[U88] JS：对象展开合并
来源：http://fr.colortex.cn

{ ...a, ...b }
来源：http://se.shtwfgs.cn

[U89] JS：数组去重
来源：http://bj.yuexingan06.cn

[...new Set(arr)]
来源：http://fy.nicolike.cn

[U90] JS：数字数组排序
来源：http://gi.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://mh.newstarts.cn

[U91] JS：对象键值遍历
来源：http://dx.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ye.hahajie.cn

[U92] JS：深拷贝
来源：http://yj.nszjky.cn

structuredClone(obj)
来源：http://ib.colortex.cn

[U93] JS：模板字符串
来源：http://ay.chemitech.net.cn

`共 ${n} 条`
来源：http://yb.colortex.cn

[U94] JS：箭头函数
来源：http://up.lnxyls.cn

const double = x => x * 2;
来源：http://sv.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://hi.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://ve.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ed.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ol.muxihuayi.cn

[U97] JS：并发请求
来源：http://ja.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cc.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://ne.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sh.asd995.cn

[U99] JS：事件监听
来源：http://bc.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://zg.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://ap.hnjuh.cn

document.querySelector(".item")
来源：http://gi.hahajie.cn

[U101] JS：classList 操作
来源：http://dw.shxzskj.cn

el.classList.toggle("active")
来源：http://dm.yuexingan06.cn

[U102] JS：本地存储
来源：http://rb.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://as.jianghongdianzi.cn

[U103] JS：定时器
来源：http://ei.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cl.shxzukj.cn

[U104] JS：防抖
来源：http://pt.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eb.shxzskj.cn

[U105] JS：节流
来源：http://lo.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wd.huixiangedu.cn

[U106] JS：日期格式化
来源：http://rd.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ev.newstarts.cn

[U107] JS：数字千分位
来源：http://qv.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lt.wgjwhj.cn

[U108] JS：随机整数
来源：http://oh.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xr.chemitech.net.cn

[U109] JS：数组分组
来源：http://xq.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://bu.szsharing.cn

[U110] JS：数组分块
来源：http://uh.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sd.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://or.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ww.hnjuh.cn

[U112] JS：字符串补位
来源：http://at.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://sy.nicolike.cn

[U113] JS：正则替换全部
来源：http://it.shxzskj.cn

s.replaceAll("a", "b")
来源：http://an.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://qc.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dp.hahajie.cn

[U115] JS：生成 UUID
来源：http://tf.bookmarksfly.cn

crypto.randomUUID()
来源：http://dj.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://bt.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://xn.huixiangedu.cn

[U117] JS：单元测试
来源：http://cz.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://iz.huixiangedu.cn

[U118] JS：开发服务器
来源：http://zw.nicolike.cn

npm i -D vite;  npx vite
来源：http://kx.huixiangedu.cn

[U119] JS：生产构建
来源：http://wd.jianghongdianzi.cn

npx vite build
来源：http://bk.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://cm.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://iy.shxzukj.cn

================================================================================
来源：http://jn.newstarts.cn

统计汇总
来源：http://rk.chemitech.net.cn

================================================================================
来源：http://ls.jctech888.com.cn

按语言统计（条）：
来源：http://wu.hahajie.cn

Python ......... 252
来源：http://qy.gzmigu.cn

PHP ............ 252
来源：http://gg.wgjwhj.cn

JavaScript ..... 252
来源：http://sb.521024.cn

TypeScript ..... 212
来源：http://ak.szsharing.cn

Java ........... 212
来源：http://nu.huanxung.cn

Go ............. 212
来源：http://ab.hnjuh.cn

Ruby ........... 212
来源：http://gn.jctech888.com.cn

C# ............. 212
来源：http://au.hnjuh.cn

C .............. 30
来源：http://ky.haigaiapp.cn

C++ ............ 30
来源：http://rt.muxihuayi.cn

SQL ............ 90
来源：http://bd.hnjuh.cn

Bash ........... 80
来源：http://wj.haigaiapp.cn

Kotlin ......... 15
来源：http://wn.9csxet.cn

Swift .......... 15
来源：http://jd.newstarts.cn

Lua ............ 10
来源：http://zt.panjiajie.cn

Perl ........... 10
来源：http://vx.shxzukj.cn

Scala .......... 10
来源：http://wc.huixinmuqiang.cn

------------------------------------
来源：http://by.9csxet.cn

合计 ........... 2106 条
来源：http://aa.haigaiapp.cn

按章节统计：
来源：http://xr.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://te.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uz.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uj.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bk.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gc.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yf.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jb.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sx.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ly.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fz.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ge.wgjwhj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zn.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bd.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qx.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ul.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fx.huixiangedu.cn

Q SQL 专题                              90
来源：http://ij.huixinmuqiang.cn

R Bash 专题                             80
来源：http://kc.muxihuayi.cn

S C / C++ 专题                          60
来源：http://if.bjjhwx.cn

T 其他语言补充                          60
来源：http://vp.bookmarksfly.cn

U 高频实用片段                         120
来源：http://qh.shtwfgs.cn

------------------------------------
来源：http://me.521024.cn

合计                                  2106 条
来源：http://pp.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ge.bjjhwx.cn

使用提醒
来源：http://af.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ke.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jz.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fo.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ov.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qu.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vn.colortex.cn

—— 文件结束 ——
来源：http://am.nszjky.cn

================================================================================
来源：http://ch.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://hy.szsharing.cn

Common Programming Examples Cheat Book
来源：http://hu.chemitech.net.cn

================================================================================
来源：http://ht.yuexingan06.cn

【收录内容】
来源：http://yv.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bl.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ll.shtwfgs.cn

SQL · Bash · C · C++
来源：http://ne.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uz.hnjuh.cn

【使用说明】
来源：http://rj.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ry.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rk.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jo.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xu.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mu.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zs.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lm.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aw.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rr.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wp.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ww.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lw.yuntaijiaju.cn

【文件统计】
来源：http://dl.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bf.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://fn.gzmigu.cn

目  录
来源：http://kk.hahajie.cn

--------------------------------------------------------------------------------
来源：http://im.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lm.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lu.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gn.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://to.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://id.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gg.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://le.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hq.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kb.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zh.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yq.hnjuh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wo.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sw.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rk.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rl.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vy.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ei.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ex.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kt.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hk.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fb.9csxet.cn

================================================================================
来源：http://cm.szsharing.cn

A. 基础语法与类型
来源：http://aq.yuntaijiaju.cn

================================================================================
来源：http://hr.gzmigu.cn

[A01] Hello World
来源：http://hj.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://jf.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://ry.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://os.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nl.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://yx.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://zp.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://zi.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zk.shxzskj.cn

[A02] 变量声明与赋值
来源：http://gj.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pi.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dg.asd995.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vh.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yi.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://dn.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://lv.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://kd.bjjhwx.cn


<!-- 参考信息 -->