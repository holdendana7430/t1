代发 wailian999

[U31] Py：单测
来源：http://uh.hnjuh.cn

python -m pytest -q
来源：http://we.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://zg.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://pz.huanxung.cn

[U33] Py：打包发布
来源：http://us.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://yu.muxihuayi.cn

[U34] Py：判断编码
来源：http://ep.nszjky.cn

chardet.detect(raw)
来源：http://pc.521024.cn

[U35] Py：发送邮件
来源：http://jo.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://om.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://lk.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://bi.muxihuayi.cn

[U37] Py：读写 Excel
来源：http://oo.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rl.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://hj.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://br.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ya.wgjwhj.cn

sys.stdout.isatty()
来源：http://cs.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://gz.hahajie.cn

print("err", file=sys.stderr)
来源：http://hg.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://kg.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sf.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://qa.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://to.huanxung.cn

[U43] PHP：声明命名空间
来源：http://dh.nszjky.cn

namespace App\Http;
来源：http://yu.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://be.huixinmuqiang.cn

declare(strict_types=1);
来源：http://eq.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://mh.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ls.bjjhwx.cn

[U46] PHP：可空类型
来源：http://wp.wgjwhj.cn

?string $name = null
来源：http://pq.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://vw.newstarts.cn

int|string $id
来源：http://jk.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://lz.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xd.szxytkj.cn

[U49] PHP：只读属性
来源：http://il.shxzukj.cn

public readonly string $name
来源：http://ip.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://la.lnxyls.cn

public function __construct(private int $id) {}
来源：http://in.chemitech.net.cn

[U51] PHP：数组解构
来源：http://ea.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://fg.shxzukj.cn

[U52] PHP：箭头函数
来源：http://dj.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://ls.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://yx.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://lf.shxzskj.cn

[U54] PHP：空安全调用
来源：http://oh.bjjhwx.cn

$obj?->method()
来源：http://lf.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://tk.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ft.hnjuh.cn

[U56] PHP：命名参数
来源：http://sz.shxzskj.cn

f(a: 1, b: 2)
来源：http://gk.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://vm.nicolike.cn

"值: {$a}"
来源：http://le.colortex.cn

[U58] PHP：数组三件套
来源：http://eg.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mv.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://rl.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vl.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://pn.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://an.nicolike.cn

[U61] PHP：正则
来源：http://hx.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ab.hahajie.cn

[U62] PHP：日期对象
来源：http://et.wgjwhj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uh.shxzskj.cn

[U63] PHP：文件读写
来源：http://lm.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://md.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://gz.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://em.szxytkj.cn

[U65] PHP：会话
来源：http://tp.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://er.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://de.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ti.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://fr.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://be.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://bh.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qw.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://hn.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wu.asd995.cn

[U70] PHP：PDO 事务
来源：http://ld.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oo.nszjky.cn

[U71] PHP：抛出异常
来源：http://nq.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://if.jctech888.com.cn

[U72] PHP：写错误日志
来源：http://ao.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://zu.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://lc.huixinmuqiang.cn

parse_ini_file("config.ini", true)
来源：http://iq.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://wj.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://sb.szxytkj.cn

[U75] PHP：依赖注入
来源：http://gv.huanxung.cn

composer require psr/container
来源：http://yb.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ue.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cc.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://mw.chemitech.net.cn

composer require twig/twig
来源：http://qg.wgjwhj.cn

[U78] PHP：单元测试
来源：http://qu.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://rm.szsharing.cn

[U79] PHP：静态分析
来源：http://wg.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://rs.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://xu.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tx.hahajie.cn

[U81] JS：初始化项目
来源：http://ur.huanxung.cn

npm init -y;  npm i express
来源：http://qr.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://ir.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wl.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://rp.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zr.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://tj.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rd.haigaiapp.cn

[U85] JS：可选链
来源：http://lh.yuexingan06.cn

a?.b?.c
来源：http://km.nicolike.cn

[U86] JS：空值合并
来源：http://pf.szsharing.cn

a ?? b
来源：http://rx.shtwfgs.cn

[U87] JS：解构默认值
来源：http://vb.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://hu.szxytkj.cn

[U88] JS：对象展开合并
来源：http://ij.szsharing.cn

{ ...a, ...b }
来源：http://xm.bjjhwx.cn

[U89] JS：数组去重
来源：http://hi.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ky.hnjuh.cn

[U90] JS：数字数组排序
来源：http://wb.szsharing.cn

[...arr].sort((a, b) => a - b)
来源：http://kc.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://he.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wp.newstarts.cn

[U92] JS：深拷贝
来源：http://pu.shxzukj.cn

structuredClone(obj)
来源：http://xu.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://sz.gzmigu.cn

`共 ${n} 条`
来源：http://zp.szxytkj.cn

[U94] JS：箭头函数
来源：http://gx.jctech888.com.cn

const double = x => x * 2;
来源：http://kh.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://oi.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://rj.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://hj.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hk.nszjky.cn

[U97] JS：并发请求
来源：http://ba.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mg.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://nb.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wc.gzmigu.cn

[U99] JS：事件监听
来源：http://uk.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://tl.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://ez.szsharing.cn

document.querySelector(".item")
来源：http://ae.lnxyls.cn

[U101] JS：classList 操作
来源：http://kh.nicolike.cn

el.classList.toggle("active")
来源：http://op.szsharing.cn

[U102] JS：本地存储
来源：http://te.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dz.jctech888.com.cn

[U103] JS：定时器
来源：http://kj.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fz.shtwfgs.cn

[U104] JS：防抖
来源：http://ds.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tw.newstarts.cn

[U105] JS：节流
来源：http://ax.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ve.hnjuh.cn

[U106] JS：日期格式化
来源：http://nl.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gl.jctech888.com.cn

[U107] JS：数字千分位
来源：http://gj.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ld.lnxyls.cn

[U108] JS：随机整数
来源：http://jt.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ux.huanxung.cn

[U109] JS：数组分组
来源：http://ac.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://uz.yuexingan06.cn

[U110] JS：数组分块
来源：http://tc.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lf.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://lz.gzmigu.cn

new Map(Object.entries(obj))
来源：http://iy.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ra.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://xc.shxzukj.cn

[U113] JS：正则替换全部
来源：http://oi.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://ab.asd995.cn

[U114] JS：JSON 深比较
来源：http://aw.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tz.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://oo.newstarts.cn

crypto.randomUUID()
来源：http://yy.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://rq.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://kn.9csxet.cn

[U117] JS：单元测试
来源：http://zj.colortex.cn

npm i -D vitest;  npx vitest
来源：http://rj.shxzukj.cn

[U118] JS：开发服务器
来源：http://fc.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://ui.nszjky.cn

[U119] JS：生产构建
来源：http://ju.yuntaijiaju.cn

npx vite build
来源：http://yn.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://rg.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://bu.chemitech.net.cn

================================================================================
来源：http://ke.wgjwhj.cn

统计汇总
来源：http://kx.hahajie.cn

================================================================================
来源：http://ua.wgjwhj.cn

按语言统计（条）：
来源：http://eg.szsharing.cn

Python ......... 252
来源：http://zi.asd995.cn

PHP ............ 252
来源：http://ky.huanxung.cn

JavaScript ..... 252
来源：http://fl.521024.cn

TypeScript ..... 212
来源：http://er.9csxet.cn

Java ........... 212
来源：http://ky.hnjuh.cn

Go ............. 212
来源：http://kl.asd995.cn

Ruby ........... 212
来源：http://cc.huixinmuqiang.cn

C# ............. 212
来源：http://li.shxzukj.cn

C .............. 30
来源：http://bd.wgjwhj.cn

C++ ............ 30
来源：http://bu.bjjhwx.cn

SQL ............ 90
来源：http://fo.nszjky.cn

Bash ........... 80
来源：http://dq.wgjwhj.cn

Kotlin ......... 15
来源：http://ii.szxytkj.cn

Swift .......... 15
来源：http://ik.bjjhwx.cn

Lua ............ 10
来源：http://ce.panjiajie.cn

Perl ........... 10
来源：http://ua.nicolike.cn

Scala .......... 10
来源：http://dg.wgjwhj.cn

------------------------------------
来源：http://gk.shtwfgs.cn

合计 ........... 2106 条
来源：http://oo.huanxung.cn

按章节统计：
来源：http://cm.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bs.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wh.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ng.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pq.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zw.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ou.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bu.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cd.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ky.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uz.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://go.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ec.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sk.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ow.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pv.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rc.szxytkj.cn

Q SQL 专题                              90
来源：http://zs.nszjky.cn

R Bash 专题                             80
来源：http://fc.9csxet.cn

S C / C++ 专题                          60
来源：http://ix.jctech888.com.cn

T 其他语言补充                          60
来源：http://dc.jctech888.com.cn

U 高频实用片段                         120
来源：http://mr.gzmigu.cn

------------------------------------
来源：http://ph.gzmigu.cn

合计                                  2106 条
来源：http://vo.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://im.521024.cn

使用提醒
来源：http://cx.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ko.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qg.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zw.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jf.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fr.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zf.hahajie.cn

—— 文件结束 ——
来源：http://vl.lnxyls.cn

================================================================================
来源：http://hp.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://fp.newstarts.cn

Common Programming Examples Cheat Book
来源：http://et.muxihuayi.cn

================================================================================
来源：http://ov.nicolike.cn

【收录内容】
来源：http://sx.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zp.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rh.szsharing.cn

SQL · Bash · C · C++
来源：http://kq.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ra.jianghongdianzi.cn

【使用说明】
来源：http://rl.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://og.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hu.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vp.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ha.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ar.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ox.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wt.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bt.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ds.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ls.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ht.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zz.asd995.cn

【文件统计】
来源：http://vp.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://de.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://nq.lnxyls.cn

目  录
来源：http://uu.szsharing.cn

--------------------------------------------------------------------------------
来源：http://qo.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tq.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yi.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tm.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xk.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zq.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fv.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gc.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kr.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zp.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://os.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lt.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ch.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dx.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://en.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ph.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://of.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lj.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oj.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://un.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aq.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ke.colortex.cn

================================================================================
来源：http://sf.huanxung.cn

A. 基础语法与类型
来源：http://iz.shxzukj.cn

================================================================================
来源：http://xd.yuntaijiaju.cn

[A01] Hello World
来源：http://hv.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://nq.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://dt.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://yt.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aa.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://uo.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://sr.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://bq.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lz.panjiajie.cn

[A02] 变量声明与赋值
来源：http://yf.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vo.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kn.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qw.haigaiapp.cn


<!-- 参考信息 -->