代发 wailian999

[U23] Py：分块读取大文件
来源：http://zr.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nr.gzmigu.cn

[U24] Py：路径操作
来源：http://yg.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nm.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://wq.jctech888.com.cn

csv.DictReader(f)
来源：http://bi.huixiangedu.cn

[U26] Py：并发下载
来源：http://od.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zc.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://ng.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://dy.huixiangedu.cn

[U28] Py：类型别名
来源：http://xl.chemitech.net.cn

UserId = int
来源：http://mk.9csxet.cn

[U29] Py：属性校验
来源：http://zm.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://vp.asd995.cn

[U30] Py：数据类
来源：http://my.gzmigu.cn

@dataclass(slots=True)
来源：http://hv.hahajie.cn

[U31] Py：单测
来源：http://sp.jianghongdianzi.cn

python -m pytest -q
来源：http://ng.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://zq.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://sg.muxihuayi.cn

[U33] Py：打包发布
来源：http://pj.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://fi.bjjhwx.cn

[U34] Py：判断编码
来源：http://zn.newstarts.cn

chardet.detect(raw)
来源：http://lo.shtwfgs.cn

[U35] Py：发送邮件
来源：http://be.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gz.chemitech.net.cn

[U36] Py：定时任务
来源：http://pl.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://wp.huanxung.cn

[U37] Py：读写 Excel
来源：http://he.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uv.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://cz.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://fr.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://bq.shtwfgs.cn

sys.stdout.isatty()
来源：http://xc.huanxung.cn

[U40] Py：打印到标准错误
来源：http://sl.newstarts.cn

print("err", file=sys.stderr)
来源：http://ba.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://kn.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kn.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://we.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oh.colortex.cn

[U43] PHP：声明命名空间
来源：http://dz.wgjwhj.cn

namespace App\Http;
来源：http://ra.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://nz.colortex.cn

declare(strict_types=1);
来源：http://yy.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://lz.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qv.shxzukj.cn

[U46] PHP：可空类型
来源：http://ko.colortex.cn

?string $name = null
来源：http://if.asd995.cn

[U47] PHP：联合类型
来源：http://kc.shxzskj.cn

int|string $id
来源：http://od.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://xg.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rd.huanxung.cn

[U49] PHP：只读属性
来源：http://at.huixiangedu.cn

public readonly string $name
来源：http://iv.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://oj.szsharing.cn

public function __construct(private int $id) {}
来源：http://uz.shxzskj.cn

[U51] PHP：数组解构
来源：http://cm.bookmarksfly.cn

[$a, $b] = $arr;
来源：http://cr.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://au.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://bt.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://mc.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://iy.asd995.cn

[U54] PHP：空安全调用
来源：http://uy.huanxung.cn

$obj?->method()
来源：http://jo.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://sf.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qw.yuexingan06.cn

[U56] PHP：命名参数
来源：http://sc.hahajie.cn

f(a: 1, b: 2)
来源：http://qj.9csxet.cn

[U57] PHP：字符串插值
来源：http://ch.haigaiapp.cn

"值: {$a}"
来源：http://dq.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://es.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ub.shxzukj.cn

[U59] PHP：自定义排序
来源：http://gr.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qc.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://mn.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kh.gzmigu.cn

[U61] PHP：正则
来源：http://vn.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dn.jctech888.com.cn

[U62] PHP：日期对象
来源：http://cs.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pt.newstarts.cn

[U63] PHP：文件读写
来源：http://lo.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lg.9csxet.cn

[U64] PHP：目录遍历
来源：http://ln.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://bk.szsharing.cn

[U65] PHP：会话
来源：http://hb.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ej.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://wy.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pw.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://df.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uk.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://nk.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rs.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://ne.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lu.huanxung.cn

[U70] PHP：PDO 事务
来源：http://td.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ne.nicolike.cn

[U71] PHP：抛出异常
来源：http://df.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://ir.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://jq.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://xv.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://zs.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://lk.chemitech.net.cn

[U74] PHP：读取环境变量
来源：http://yi.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://hz.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://qf.szxytkj.cn

composer require psr/container
来源：http://hg.newstarts.cn

[U76] PHP：简单路由
来源：http://eh.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vg.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://xg.9csxet.cn

composer require twig/twig
来源：http://ym.nicolike.cn

[U78] PHP：单元测试
来源：http://sv.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://bg.gzmigu.cn

[U79] PHP：静态分析
来源：http://xn.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://hr.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://er.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fo.hahajie.cn

[U81] JS：初始化项目
来源：http://bc.newstarts.cn

npm init -y;  npm i express
来源：http://sq.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://ga.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vx.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://nh.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dk.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://bk.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hq.lnxyls.cn

[U85] JS：可选链
来源：http://me.haigaiapp.cn

a?.b?.c
来源：http://rl.lnxyls.cn

[U86] JS：空值合并
来源：http://en.newstarts.cn

a ?? b
来源：http://vv.gzmigu.cn

[U87] JS：解构默认值
来源：http://rr.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://bf.nszjky.cn

[U88] JS：对象展开合并
来源：http://fa.shxzskj.cn

{ ...a, ...b }
来源：http://eu.gzmigu.cn

[U89] JS：数组去重
来源：http://sd.521024.cn

[...new Set(arr)]
来源：http://ks.hnjuh.cn

[U90] JS：数字数组排序
来源：http://eu.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://sa.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://hj.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://an.lnxyls.cn

[U92] JS：深拷贝
来源：http://ns.bjjhwx.cn

structuredClone(obj)
来源：http://ch.huanxung.cn

[U93] JS：模板字符串
来源：http://mm.nicolike.cn

`共 ${n} 条`
来源：http://so.chemitech.net.cn

[U94] JS：箭头函数
来源：http://fc.asd995.cn

const double = x => x * 2;
来源：http://se.colortex.cn

[U95] JS：Promise 包装
来源：http://jk.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://fi.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://hs.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fq.shxzukj.cn

[U97] JS：并发请求
来源：http://cu.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ey.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://lt.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zf.huanxung.cn

[U99] JS：事件监听
来源：http://nv.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://er.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://fn.yuexingan06.cn

document.querySelector(".item")
来源：http://wo.shtwfgs.cn

[U101] JS：classList 操作
来源：http://rj.yuntaijiaju.cn

el.classList.toggle("active")
来源：http://rz.colortex.cn

[U102] JS：本地存储
来源：http://oc.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cx.nicolike.cn

[U103] JS：定时器
来源：http://hz.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ze.jctech888.com.cn

[U104] JS：防抖
来源：http://we.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.wgjwhj.cn

[U105] JS：节流
来源：http://yg.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kn.9csxet.cn

[U106] JS：日期格式化
来源：http://hk.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ml.szxytkj.cn

[U107] JS：数字千分位
来源：http://oh.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jt.shxzskj.cn

[U108] JS：随机整数
来源：http://nw.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qy.bookmarksfly.cn

[U109] JS：数组分组
来源：http://zp.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://fr.521024.cn

[U110] JS：数组分块
来源：http://gc.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cu.newstarts.cn

[U111] JS：对象转 Map
来源：http://nn.newstarts.cn

new Map(Object.entries(obj))
来源：http://pq.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://rx.haigaiapp.cn

"7".padStart(3, "0")
来源：http://eq.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://ge.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://im.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://oh.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yt.asd995.cn

[U115] JS：生成 UUID
来源：http://gw.jianghongdianzi.cn

crypto.randomUUID()
来源：http://hi.yuntaijiaju.cn

[U116] JS：类型检查（JSDoc）
来源：http://fl.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://lx.huixiangedu.cn

[U117] JS：单元测试
来源：http://ig.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://kq.shxzskj.cn

[U118] JS：开发服务器
来源：http://xc.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://rj.hnjuh.cn

[U119] JS：生产构建
来源：http://fe.haigaiapp.cn

npx vite build
来源：http://er.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://fr.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://mv.yuntaijiaju.cn

================================================================================
来源：http://wi.wgjwhj.cn

统计汇总
来源：http://zf.bookmarksfly.cn

================================================================================
来源：http://ue.huixiangedu.cn

按语言统计（条）：
来源：http://ua.colortex.cn

Python ......... 252
来源：http://rt.yuntaijiaju.cn

PHP ............ 252
来源：http://mr.gzmigu.cn

JavaScript ..... 252
来源：http://va.bjjhwx.cn

TypeScript ..... 212
来源：http://df.colortex.cn

Java ........... 212
来源：http://rd.nicolike.cn

Go ............. 212
来源：http://mc.nicolike.cn

Ruby ........... 212
来源：http://ic.colortex.cn

C# ............. 212
来源：http://du.hahajie.cn

C .............. 30
来源：http://bt.bookmarksfly.cn

C++ ............ 30
来源：http://be.yuntaijiaju.cn

SQL ............ 90
来源：http://dw.panjiajie.cn

Bash ........... 80
来源：http://wj.9csxet.cn

Kotlin ......... 15
来源：http://jz.jctech888.com.cn

Swift .......... 15
来源：http://gf.bookmarksfly.cn

Lua ............ 10
来源：http://my.szsharing.cn

Perl ........... 10
来源：http://aa.nszjky.cn

Scala .......... 10
来源：http://oo.shxzskj.cn

------------------------------------
来源：http://ao.chemitech.net.cn

合计 ........... 2106 条
来源：http://az.jianghongdianzi.cn

按章节统计：
来源：http://jg.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kz.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qw.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wk.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lc.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cx.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vn.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ve.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fg.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mi.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xd.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qd.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ui.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ad.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ao.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tw.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ng.shxzskj.cn

Q SQL 专题                              90
来源：http://cp.521024.cn

R Bash 专题                             80
来源：http://py.shxzskj.cn

S C / C++ 专题                          60
来源：http://rv.colortex.cn

T 其他语言补充                          60
来源：http://fd.lnxyls.cn

U 高频实用片段                         120
来源：http://mv.chemitech.net.cn

------------------------------------
来源：http://ua.hahajie.cn

合计                                  2106 条
来源：http://ji.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://az.hahajie.cn

使用提醒
来源：http://dy.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://wx.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bm.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qv.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dk.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ny.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sk.colortex.cn

—— 文件结束 ——
来源：http://ck.shtwfgs.cn

================================================================================
来源：http://xx.hnjuh.cn

程序语言常见例子速查手册（2024 版）
来源：http://kh.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://kn.shxzskj.cn

================================================================================
来源：http://xp.huixiangedu.cn

【收录内容】
来源：http://pk.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wq.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bc.colortex.cn

SQL · Bash · C · C++
来源：http://vh.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://to.huixinmuqiang.cn

【使用说明】
来源：http://sv.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pk.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dw.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lk.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ap.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bf.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ih.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tz.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oh.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cq.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qo.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mr.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vc.yuexingan06.cn

【文件统计】
来源：http://pw.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hl.nszjky.cn

--------------------------------------------------------------------------------
来源：http://dd.shxzskj.cn

目  录
来源：http://mm.colortex.cn

--------------------------------------------------------------------------------
来源：http://mn.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yz.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ux.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qi.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://up.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yq.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rf.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ew.nicolike.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qx.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oi.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://md.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://od.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fp.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://no.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pw.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://so.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cz.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kf.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vp.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fq.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ho.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tb.chemitech.net.cn


<!-- 参考信息 -->