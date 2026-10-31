代发 wailian999

[U23] Py：分块读取大文件
来源：http://hc.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://up.hahajie.cn

[U24] Py：路径操作
来源：http://ri.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qz.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://xa.shxzskj.cn

csv.DictReader(f)
来源：http://vk.nszjky.cn

[U26] Py：并发下载
来源：http://au.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gv.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://ln.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://cy.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://eh.jianghongdianzi.cn

UserId = int
来源：http://pq.lnxyls.cn

[U29] Py：属性校验
来源：http://fy.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://xu.yuntaijiaju.cn

[U30] Py：数据类
来源：http://kz.hahajie.cn

@dataclass(slots=True)
来源：http://ej.huixinmuqiang.cn

[U31] Py：单测
来源：http://hl.huanxung.cn

python -m pytest -q
来源：http://qy.huixiangedu.cn

[U32] Py：代码格式化
来源：http://qr.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://mz.521024.cn

[U33] Py：打包发布
来源：http://sj.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ai.szsharing.cn

[U34] Py：判断编码
来源：http://dx.bookmarksfly.cn

chardet.detect(raw)
来源：http://gv.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://ah.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.nicolike.cn

[U36] Py：定时任务
来源：http://sp.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://wr.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://zf.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://va.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://fb.9csxet.cn

Path(__file__).resolve().parent
来源：http://fn.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://fr.hahajie.cn

sys.stdout.isatty()
来源：http://vn.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://ds.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://oo.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://or.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hy.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://he.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tf.521024.cn

[U43] PHP：声明命名空间
来源：http://vz.panjiajie.cn

namespace App\Http;
来源：http://mw.newstarts.cn

[U44] PHP：开启严格类型
来源：http://my.yuexingan06.cn

declare(strict_types=1);
来源：http://ay.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ow.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://so.huanxung.cn

[U46] PHP：可空类型
来源：http://cp.shxzskj.cn

?string $name = null
来源：http://sk.szsharing.cn

[U47] PHP：联合类型
来源：http://hv.newstarts.cn

int|string $id
来源：http://qe.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://lj.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vd.newstarts.cn

[U49] PHP：只读属性
来源：http://ot.bjjhwx.cn

public readonly string $name
来源：http://hf.521024.cn

[U50] PHP：构造器属性提升
来源：http://yf.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://eq.haigaiapp.cn

[U51] PHP：数组解构
来源：http://ma.shxzskj.cn

[$a, $b] = $arr;
来源：http://jn.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://np.asd995.cn

$double = fn($x) => $x * 2;
来源：http://qb.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://kh.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://qe.gzmigu.cn

[U54] PHP：空安全调用
来源：http://ae.szxytkj.cn

$obj?->method()
来源：http://ms.colortex.cn

[U55] PHP：match 表达式
来源：http://sn.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://el.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://hd.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ch.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://jh.newstarts.cn

"值: {$a}"
来源：http://mr.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://cg.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sy.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ct.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mp.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://il.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uv.9csxet.cn

[U61] PHP：正则
来源：http://zy.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tu.521024.cn

[U62] PHP：日期对象
来源：http://ib.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pg.shxzskj.cn

[U63] PHP：文件读写
来源：http://gx.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lz.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://vg.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://nd.yuntaijiaju.cn

[U65] PHP：会话
来源：http://hj.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vl.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ho.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cc.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://ss.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oz.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://ic.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rp.asd995.cn

[U69] PHP：PDO 预处理
来源：http://up.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://au.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://kg.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ut.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://mn.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://pa.shxzskj.cn

[U72] PHP：写错误日志
来源：http://bm.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://gf.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://wu.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://za.huanxung.cn

[U74] PHP：读取环境变量
来源：http://bq.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://zh.szxytkj.cn

[U75] PHP：依赖注入
来源：http://pu.jianghongdianzi.cn

composer require psr/container
来源：http://dl.nicolike.cn

[U76] PHP：简单路由
来源：http://ng.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zo.lnxyls.cn

[U77] PHP：模板渲染
来源：http://ou.asd995.cn

composer require twig/twig
来源：http://fx.shxzukj.cn

[U78] PHP：单元测试
来源：http://df.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://vx.haigaiapp.cn

[U79] PHP：静态分析
来源：http://or.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://ss.nszjky.cn

[U80] PHP：代码规范修复
来源：http://kx.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fl.szxytkj.cn

[U81] JS：初始化项目
来源：http://ql.shxzukj.cn

npm init -y;  npm i express
来源：http://pd.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://kk.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lq.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://jx.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ag.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://bw.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cm.huanxung.cn

[U85] JS：可选链
来源：http://nn.asd995.cn

a?.b?.c
来源：http://mb.szsharing.cn

[U86] JS：空值合并
来源：http://du.yuexingan06.cn

a ?? b
来源：http://lb.hahajie.cn

[U87] JS：解构默认值
来源：http://ya.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://sx.newstarts.cn

[U88] JS：对象展开合并
来源：http://er.9csxet.cn

{ ...a, ...b }
来源：http://fh.nszjky.cn

[U89] JS：数组去重
来源：http://ge.521024.cn

[...new Set(arr)]
来源：http://oz.gzmigu.cn

[U90] JS：数字数组排序
来源：http://dh.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://tq.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://dm.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zf.hahajie.cn

[U92] JS：深拷贝
来源：http://in.bookmarksfly.cn

structuredClone(obj)
来源：http://cw.shtwfgs.cn

[U93] JS：模板字符串
来源：http://zj.shxzskj.cn

`共 ${n} 条`
来源：http://jc.newstarts.cn

[U94] JS：箭头函数
来源：http://lr.jianghongdianzi.cn

const double = x => x * 2;
来源：http://uj.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://ep.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://be.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://pf.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lb.muxihuayi.cn

[U97] JS：并发请求
来源：http://wb.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://rp.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://an.szxytkj.cn

[U99] JS：事件监听
来源：http://ee.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://dm.shxzskj.cn

[U100] JS：DOM 查询
来源：http://op.szxytkj.cn

document.querySelector(".item")
来源：http://bf.colortex.cn

[U101] JS：classList 操作
来源：http://cb.szxytkj.cn

el.classList.toggle("active")
来源：http://js.gzmigu.cn

[U102] JS：本地存储
来源：http://iq.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sx.hnjuh.cn

[U103] JS：定时器
来源：http://ut.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nh.nszjky.cn

[U104] JS：防抖
来源：http://ki.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zr.9csxet.cn

[U105] JS：节流
来源：http://ll.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pl.szxytkj.cn

[U106] JS：日期格式化
来源：http://mb.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zw.szxytkj.cn

[U107] JS：数字千分位
来源：http://tj.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cg.9csxet.cn

[U108] JS：随机整数
来源：http://oh.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kp.szsharing.cn

[U109] JS：数组分组
来源：http://oj.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://be.shtwfgs.cn

[U110] JS：数组分块
来源：http://bg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jd.hahajie.cn

[U111] JS：对象转 Map
来源：http://to.nicolike.cn

new Map(Object.entries(obj))
来源：http://iu.yuexingan06.cn

[U112] JS：字符串补位
来源：http://of.521024.cn

"7".padStart(3, "0")
来源：http://ds.asd995.cn

[U113] JS：正则替换全部
来源：http://na.colortex.cn

s.replaceAll("a", "b")
来源：http://jx.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://hb.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qu.hahajie.cn

[U115] JS：生成 UUID
来源：http://wt.wgjwhj.cn

crypto.randomUUID()
来源：http://fk.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://cg.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ud.panjiajie.cn

[U117] JS：单元测试
来源：http://ok.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://rr.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://lb.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://sj.haigaiapp.cn

[U119] JS：生产构建
来源：http://cj.hnjuh.cn

npx vite build
来源：http://tt.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://cx.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://wv.bookmarksfly.cn

================================================================================
来源：http://lq.haigaiapp.cn

统计汇总
来源：http://om.chemitech.net.cn

================================================================================
来源：http://tj.shtwfgs.cn

按语言统计（条）：
来源：http://sf.bookmarksfly.cn

Python ......... 252
来源：http://uv.gzmigu.cn

PHP ............ 252
来源：http://np.asd995.cn

JavaScript ..... 252
来源：http://ve.lnxyls.cn

TypeScript ..... 212
来源：http://au.szxytkj.cn

Java ........... 212
来源：http://fd.shxzskj.cn

Go ............. 212
来源：http://kp.haigaiapp.cn

Ruby ........... 212
来源：http://tv.nicolike.cn

C# ............. 212
来源：http://zp.bjjhwx.cn

C .............. 30
来源：http://ow.hnjuh.cn

C++ ............ 30
来源：http://wk.yuntaijiaju.cn

SQL ............ 90
来源：http://xq.newstarts.cn

Bash ........... 80
来源：http://yf.asd995.cn

Kotlin ......... 15
来源：http://ue.jianghongdianzi.cn

Swift .......... 15
来源：http://aw.asd995.cn

Lua ............ 10
来源：http://aj.asd995.cn

Perl ........... 10
来源：http://bn.panjiajie.cn

Scala .......... 10
来源：http://eq.huixinmuqiang.cn

------------------------------------
来源：http://vj.hahajie.cn

合计 ........... 2106 条
来源：http://ng.nicolike.cn

按章节统计：
来源：http://xe.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wa.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gs.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xv.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qj.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hg.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sv.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ai.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ch.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cu.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mq.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dk.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qt.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hh.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zb.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rp.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qd.asd995.cn

Q SQL 专题                              90
来源：http://bi.szsharing.cn

R Bash 专题                             80
来源：http://kx.9csxet.cn

S C / C++ 专题                          60
来源：http://hm.hnjuh.cn

T 其他语言补充                          60
来源：http://wz.gzmigu.cn

U 高频实用片段                         120
来源：http://sp.panjiajie.cn

------------------------------------
来源：http://nh.colortex.cn

合计                                  2106 条
来源：http://lt.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://sz.shxzukj.cn

使用提醒
来源：http://ew.colortex.cn

--------------------------------------------------------------------------------
来源：http://wj.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uj.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ni.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fu.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rj.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jt.huixiangedu.cn

—— 文件结束 ——
来源：http://cd.szsharing.cn

================================================================================
来源：http://vv.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://bp.szsharing.cn

Common Programming Examples Cheat Book
来源：http://qv.colortex.cn

================================================================================
来源：http://uq.lnxyls.cn

【收录内容】
来源：http://ud.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qi.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jv.shxzukj.cn

SQL · Bash · C · C++
来源：http://bb.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ob.nszjky.cn

【使用说明】
来源：http://uu.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://al.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rv.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vj.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tg.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ve.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dv.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ko.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vs.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ae.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vg.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qr.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ba.521024.cn

【文件统计】
来源：http://uj.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ux.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hf.hnjuh.cn

目  录
来源：http://vk.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ff.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hl.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bp.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tg.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oz.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jb.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://im.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kp.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://st.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nz.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wk.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bz.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ae.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zo.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gv.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oi.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://um.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ew.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ei.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vu.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tg.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rp.yuexingan06.cn


<!-- 参考信息 -->