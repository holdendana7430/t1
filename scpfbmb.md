代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://zg.521024.cn

@contextlib.contextmanager
来源：http://wo.colortex.cn

[U22] Py：矩阵转置
来源：http://yb.bjjhwx.cn

list(zip(*m))
来源：http://vu.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://bd.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nz.wgjwhj.cn

[U24] Py：路径操作
来源：http://zo.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xu.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://pu.yuntaijiaju.cn

csv.DictReader(f)
来源：http://xg.bjjhwx.cn

[U26] Py：并发下载
来源：http://xt.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ti.newstarts.cn

[U27] Py：异步 HTTP
来源：http://mz.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ec.asd995.cn

[U28] Py：类型别名
来源：http://fl.yuexingan06.cn

UserId = int
来源：http://jk.bookmarksfly.cn

[U29] Py：属性校验
来源：http://bz.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://lb.panjiajie.cn

[U30] Py：数据类
来源：http://sa.bookmarksfly.cn

@dataclass(slots=True)
来源：http://yk.nszjky.cn

[U31] Py：单测
来源：http://zn.newstarts.cn

python -m pytest -q
来源：http://ue.szxytkj.cn

[U32] Py：代码格式化
来源：http://jy.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://nl.hnjuh.cn

[U33] Py：打包发布
来源：http://zw.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://oh.szxytkj.cn

[U34] Py：判断编码
来源：http://hl.panjiajie.cn

chardet.detect(raw)
来源：http://vt.newstarts.cn

[U35] Py：发送邮件
来源：http://ss.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ui.yuexingan06.cn

[U36] Py：定时任务
来源：http://po.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://nv.colortex.cn

[U37] Py：读写 Excel
来源：http://zf.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jp.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://dn.shxzskj.cn

Path(__file__).resolve().parent
来源：http://yy.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://dp.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://qu.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://aw.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://bq.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://oj.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jt.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://ks.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zj.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ka.shxzukj.cn

namespace App\Http;
来源：http://jj.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://oo.chemitech.net.cn

declare(strict_types=1);
来源：http://gc.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://dk.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.haigaiapp.cn

[U46] PHP：可空类型
来源：http://ph.yuntaijiaju.cn

?string $name = null
来源：http://rh.9csxet.cn

[U47] PHP：联合类型
来源：http://lh.muxihuayi.cn

int|string $id
来源：http://hg.szxytkj.cn

[U48] PHP：纯枚举
来源：http://mv.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vw.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://cn.lnxyls.cn

public readonly string $name
来源：http://ov.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://zt.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://od.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://wi.hahajie.cn

[$a, $b] = $arr;
来源：http://pu.jianghongdianzi.cn

[U52] PHP：箭头函数
来源：http://nq.521024.cn

$double = fn($x) => $x * 2;
来源：http://vk.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://fx.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://gt.9csxet.cn

[U54] PHP：空安全调用
来源：http://oq.haigaiapp.cn

$obj?->method()
来源：http://wl.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://lq.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qw.shxzskj.cn

[U56] PHP：命名参数
来源：http://sc.hahajie.cn

f(a: 1, b: 2)
来源：http://mp.colortex.cn

[U57] PHP：字符串插值
来源：http://gf.newstarts.cn

"值: {$a}"
来源：http://qy.9csxet.cn

[U58] PHP：数组三件套
来源：http://pf.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://no.gzmigu.cn

[U59] PHP：自定义排序
来源：http://wu.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sk.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://jg.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fm.yuntaijiaju.cn

[U61] PHP：正则
来源：http://xw.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yq.muxihuayi.cn

[U62] PHP：日期对象
来源：http://la.nszjky.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://au.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://sj.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wz.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://lj.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://cm.newstarts.cn

[U65] PHP：会话
来源：http://oh.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yp.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://wu.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lz.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://xk.panjiajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hy.nicolike.cn

[U68] PHP：PDO 连接
来源：http://sc.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sb.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://wi.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gx.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://ga.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mh.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://ci.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://gn.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://yf.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://lg.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://rk.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://cw.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://oq.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://cw.panjiajie.cn

[U75] PHP：依赖注入
来源：http://tr.yuexingan06.cn

composer require psr/container
来源：http://vg.jctech888.com.cn

[U76] PHP：简单路由
来源：http://wr.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eb.nicolike.cn

[U77] PHP：模板渲染
来源：http://vw.shxzukj.cn

composer require twig/twig
来源：http://vc.hnjuh.cn

[U78] PHP：单元测试
来源：http://pi.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://ou.yuexingan06.cn

[U79] PHP：静态分析
来源：http://pd.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://sx.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://sd.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://on.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://ln.huixiangedu.cn

npm init -y;  npm i express
来源：http://sp.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ns.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tv.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://gp.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://md.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://zu.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oq.huixinmuqiang.cn

[U85] JS：可选链
来源：http://mw.szxytkj.cn

a?.b?.c
来源：http://bc.shxzskj.cn

[U86] JS：空值合并
来源：http://ax.colortex.cn

a ?? b
来源：http://jd.521024.cn

[U87] JS：解构默认值
来源：http://qh.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://rk.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://zc.chemitech.net.cn

{ ...a, ...b }
来源：http://mg.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://bb.gzmigu.cn

[...new Set(arr)]
来源：http://yn.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://hc.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://jl.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://kl.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mb.hnjuh.cn

[U92] JS：深拷贝
来源：http://ov.nicolike.cn

structuredClone(obj)
来源：http://zu.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ir.colortex.cn

`共 ${n} 条`
来源：http://nh.wgjwhj.cn

[U94] JS：箭头函数
来源：http://xo.9csxet.cn

const double = x => x * 2;
来源：http://zb.lnxyls.cn

[U95] JS：Promise 包装
来源：http://qt.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://ut.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://wu.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ui.chemitech.net.cn

[U97] JS：并发请求
来源：http://vu.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kv.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://fl.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kv.nszjky.cn

[U99] JS：事件监听
来源：http://sa.huanxung.cn

el.addEventListener("click", e => {})
来源：http://bq.szxytkj.cn

[U100] JS：DOM 查询
来源：http://hb.chemitech.net.cn

document.querySelector(".item")
来源：http://ft.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://zw.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://sa.asd995.cn

[U102] JS：本地存储
来源：http://zt.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qh.newstarts.cn

[U103] JS：定时器
来源：http://yf.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://es.szsharing.cn

[U104] JS：防抖
来源：http://jv.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fb.bookmarksfly.cn

[U105] JS：节流
来源：http://rr.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vi.szsharing.cn

[U106] JS：日期格式化
来源：http://bt.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://he.chemitech.net.cn

[U107] JS：数字千分位
来源：http://kr.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rg.bookmarksfly.cn

[U108] JS：随机整数
来源：http://nk.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ca.asd995.cn

[U109] JS：数组分组
来源：http://mz.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://up.panjiajie.cn

[U110] JS：数组分块
来源：http://vz.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aw.szxytkj.cn

[U111] JS：对象转 Map
来源：http://no.asd995.cn

new Map(Object.entries(obj))
来源：http://xe.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://tf.hnjuh.cn

"7".padStart(3, "0")
来源：http://lr.colortex.cn

[U113] JS：正则替换全部
来源：http://ue.szxytkj.cn

s.replaceAll("a", "b")
来源：http://ph.colortex.cn

[U114] JS：JSON 深比较
来源：http://ge.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wv.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://qj.bookmarksfly.cn

crypto.randomUUID()
来源：http://rg.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://iy.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://rj.muxihuayi.cn

[U117] JS：单元测试
来源：http://wv.521024.cn

npm i -D vitest;  npx vitest
来源：http://zi.hahajie.cn

[U118] JS：开发服务器
来源：http://ja.colortex.cn

npm i -D vite;  npx vite
来源：http://cy.newstarts.cn

[U119] JS：生产构建
来源：http://jj.huanxung.cn

npx vite build
来源：http://hi.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rp.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://sb.gzmigu.cn

================================================================================
来源：http://pe.bjjhwx.cn

统计汇总
来源：http://og.shtwfgs.cn

================================================================================
来源：http://pa.colortex.cn

按语言统计（条）：
来源：http://fn.shtwfgs.cn

Python ......... 252
来源：http://vs.yuntaijiaju.cn

PHP ............ 252
来源：http://jd.huixiangedu.cn

JavaScript ..... 252
来源：http://hl.nszjky.cn

TypeScript ..... 212
来源：http://fw.huanxung.cn

Java ........... 212
来源：http://dc.huanxung.cn

Go ............. 212
来源：http://yt.hnjuh.cn

Ruby ........... 212
来源：http://um.haigaiapp.cn

C# ............. 212
来源：http://my.9csxet.cn

C .............. 30
来源：http://xg.jctech888.com.cn

C++ ............ 30
来源：http://nl.bjjhwx.cn

SQL ............ 90
来源：http://ec.asd995.cn

Bash ........... 80
来源：http://zx.hnjuh.cn

Kotlin ......... 15
来源：http://ok.huanxung.cn

Swift .......... 15
来源：http://zs.521024.cn

Lua ............ 10
来源：http://db.szsharing.cn

Perl ........... 10
来源：http://lx.szsharing.cn

Scala .......... 10
来源：http://uv.asd995.cn

------------------------------------
来源：http://ie.nicolike.cn

合计 ........... 2106 条
来源：http://mq.gzmigu.cn

按章节统计：
来源：http://cy.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yj.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qe.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ki.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ev.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pb.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://no.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oi.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zn.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lf.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kw.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qc.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oe.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fv.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gd.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zo.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ra.shxzskj.cn

Q SQL 专题                              90
来源：http://gt.colortex.cn

R Bash 专题                             80
来源：http://im.huixiangedu.cn

S C / C++ 专题                          60
来源：http://eb.asd995.cn

T 其他语言补充                          60
来源：http://be.szxytkj.cn

U 高频实用片段                         120
来源：http://gi.9csxet.cn

------------------------------------
来源：http://yy.huixinmuqiang.cn

合计                                  2106 条
来源：http://on.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://xf.colortex.cn

使用提醒
来源：http://wi.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://pw.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ms.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gv.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lu.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dp.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zj.yuexingan06.cn

—— 文件结束 ——
来源：http://pv.szsharing.cn

================================================================================
来源：http://cw.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://qj.newstarts.cn

Common Programming Examples Cheat Book
来源：http://sc.nszjky.cn

================================================================================
来源：http://hr.asd995.cn

【收录内容】
来源：http://bh.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fi.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jf.hahajie.cn

SQL · Bash · C · C++
来源：http://ui.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uh.shxzskj.cn

【使用说明】
来源：http://hg.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://et.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ns.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jg.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ap.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wq.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ce.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fr.jctech888.com.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ba.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vq.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nw.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qn.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fi.muxihuayi.cn

【文件统计】
来源：http://od.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fg.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://sa.colortex.cn

目  录
来源：http://pe.huanxung.cn

--------------------------------------------------------------------------------
来源：http://fc.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eo.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iw.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jo.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tk.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cx.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ua.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pn.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fc.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://we.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vg.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ci.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pf.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qv.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ey.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ss.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aj.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vg.bookmarksfly.cn


<!-- 参考信息 -->