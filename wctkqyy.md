代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://of.9csxet.cn

@contextlib.contextmanager
来源：http://sf.nszjky.cn

[U22] Py：矩阵转置
来源：http://mg.chemitech.net.cn

list(zip(*m))
来源：http://pb.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://bj.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ku.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://kd.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zz.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://wv.asd995.cn

csv.DictReader(f)
来源：http://gt.shxzskj.cn

[U26] Py：并发下载
来源：http://pj.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ib.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://vl.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://om.bookmarksfly.cn

[U28] Py：类型别名
来源：http://bp.shxzskj.cn

UserId = int
来源：http://nn.521024.cn

[U29] Py：属性校验
来源：http://vj.hnjuh.cn

@property 与 @x.setter 配合
来源：http://oh.haigaiapp.cn

[U30] Py：数据类
来源：http://hv.asd995.cn

@dataclass(slots=True)
来源：http://hg.haigaiapp.cn

[U31] Py：单测
来源：http://cq.szsharing.cn

python -m pytest -q
来源：http://zz.hnjuh.cn

[U32] Py：代码格式化
来源：http://jx.9csxet.cn

ruff format . && ruff check --fix .
来源：http://hc.muxihuayi.cn

[U33] Py：打包发布
来源：http://cx.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://oz.newstarts.cn

[U34] Py：判断编码
来源：http://bj.hahajie.cn

chardet.detect(raw)
来源：http://rs.szxytkj.cn

[U35] Py：发送邮件
来源：http://zr.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://do.lnxyls.cn

[U36] Py：定时任务
来源：http://ql.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://wj.nicolike.cn

[U37] Py：读写 Excel
来源：http://xo.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kw.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://kx.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://gx.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://hx.nicolike.cn

sys.stdout.isatty()
来源：http://mf.szsharing.cn

[U40] Py：打印到标准错误
来源：http://oe.lnxyls.cn

print("err", file=sys.stderr)
来源：http://af.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://ma.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wm.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://gi.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pt.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://ab.shxzukj.cn

namespace App\Http;
来源：http://sk.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://es.huixiangedu.cn

declare(strict_types=1);
来源：http://cy.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://ku.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dz.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://gj.lnxyls.cn

?string $name = null
来源：http://lj.huixiangedu.cn

[U47] PHP：联合类型
来源：http://yu.gzmigu.cn

int|string $id
来源：http://re.shxzskj.cn

[U48] PHP：纯枚举
来源：http://lx.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://he.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://ri.bookmarksfly.cn

public readonly string $name
来源：http://fe.colortex.cn

[U50] PHP：构造器属性提升
来源：http://qg.huanxung.cn

public function __construct(private int $id) {}
来源：http://vy.521024.cn

[U51] PHP：数组解构
来源：http://se.nszjky.cn

[$a, $b] = $arr;
来源：http://ws.521024.cn

[U52] PHP：箭头函数
来源：http://tz.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ut.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://zf.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://im.lnxyls.cn

[U54] PHP：空安全调用
来源：http://tv.bjjhwx.cn

$obj?->method()
来源：http://xt.hahajie.cn

[U55] PHP：match 表达式
来源：http://si.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ud.huixinmuqiang.cn

[U56] PHP：命名参数
来源：http://zq.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://xw.colortex.cn

[U57] PHP：字符串插值
来源：http://ar.yuexingan06.cn

"值: {$a}"
来源：http://ir.9csxet.cn

[U58] PHP：数组三件套
来源：http://cj.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lg.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://dt.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tg.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://df.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yd.shtwfgs.cn

[U61] PHP：正则
来源：http://xz.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ug.szsharing.cn

[U62] PHP：日期对象
来源：http://nz.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nj.hnjuh.cn

[U63] PHP：文件读写
来源：http://qw.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gg.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://fc.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ts.asd995.cn

[U65] PHP：会话
来源：http://rm.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pm.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://zo.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://di.szsharing.cn

[U67] PHP：处理文件上传
来源：http://xg.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eq.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://ns.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lu.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://nj.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sx.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://qy.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ng.hahajie.cn

[U71] PHP：抛出异常
来源：http://ux.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://dt.asd995.cn

[U72] PHP：写错误日志
来源：http://eb.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://ox.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://yc.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://gl.nicolike.cn

[U74] PHP：读取环境变量
来源：http://mx.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://hp.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://sg.hnjuh.cn

composer require psr/container
来源：http://vf.szsharing.cn

[U76] PHP：简单路由
来源：http://gl.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gr.yuexingan06.cn

[U77] PHP：模板渲染
来源：http://xd.nszjky.cn

composer require twig/twig
来源：http://ic.shxzskj.cn

[U78] PHP：单元测试
来源：http://eg.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://mo.hnjuh.cn

[U79] PHP：静态分析
来源：http://sx.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://um.newstarts.cn

[U80] PHP：代码规范修复
来源：http://yl.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ot.huanxung.cn

[U81] JS：初始化项目
来源：http://bu.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://vn.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://fg.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://si.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ri.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ff.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://rc.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oj.huixinmuqiang.cn

[U85] JS：可选链
来源：http://qb.chemitech.net.cn

a?.b?.c
来源：http://uq.jctech888.com.cn

[U86] JS：空值合并
来源：http://ie.szxytkj.cn

a ?? b
来源：http://yu.huixiangedu.cn

[U87] JS：解构默认值
来源：http://ts.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://uv.szxytkj.cn

[U88] JS：对象展开合并
来源：http://oi.shxzskj.cn

{ ...a, ...b }
来源：http://sm.muxihuayi.cn

[U89] JS：数组去重
来源：http://wf.yuntaijiaju.cn

[...new Set(arr)]
来源：http://kz.szsharing.cn

[U90] JS：数字数组排序
来源：http://iz.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://kl.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://pd.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jp.shxzskj.cn

[U92] JS：深拷贝
来源：http://tk.gzmigu.cn

structuredClone(obj)
来源：http://su.lnxyls.cn

[U93] JS：模板字符串
来源：http://gj.huanxung.cn

`共 ${n} 条`
来源：http://lt.lnxyls.cn

[U94] JS：箭头函数
来源：http://ww.nszjky.cn

const double = x => x * 2;
来源：http://qi.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://sj.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://fz.huanxung.cn

[U96] JS：async/await 与异常
来源：http://rv.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xa.newstarts.cn

[U97] JS：并发请求
来源：http://tt.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yt.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://ij.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ty.huanxung.cn

[U99] JS：事件监听
来源：http://vd.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://lx.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://gs.bjjhwx.cn

document.querySelector(".item")
来源：http://ns.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ze.hahajie.cn

el.classList.toggle("active")
来源：http://iq.shxzskj.cn

[U102] JS：本地存储
来源：http://ma.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://li.hnjuh.cn

[U103] JS：定时器
来源：http://jg.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bh.nszjky.cn

[U104] JS：防抖
来源：http://hx.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gz.szxytkj.cn

[U105] JS：节流
来源：http://oy.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oj.haigaiapp.cn

[U106] JS：日期格式化
来源：http://fr.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://is.nszjky.cn

[U107] JS：数字千分位
来源：http://zr.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zg.chemitech.net.cn

[U108] JS：随机整数
来源：http://xg.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.hahajie.cn

[U109] JS：数组分组
来源：http://ov.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://jf.9csxet.cn

[U110] JS：数组分块
来源：http://ut.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yk.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://bw.asd995.cn

new Map(Object.entries(obj))
来源：http://ak.nszjky.cn

[U112] JS：字符串补位
来源：http://lw.9csxet.cn

"7".padStart(3, "0")
来源：http://vj.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://br.gzmigu.cn

s.replaceAll("a", "b")
来源：http://iz.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://we.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ll.panjiajie.cn

[U115] JS：生成 UUID
来源：http://do.bookmarksfly.cn

crypto.randomUUID()
来源：http://bz.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://uv.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://lp.szsharing.cn

[U117] JS：单元测试
来源：http://ps.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://ny.521024.cn

[U118] JS：开发服务器
来源：http://er.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://ed.bookmarksfly.cn

[U119] JS：生产构建
来源：http://ma.nicolike.cn

npx vite build
来源：http://ki.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ln.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://am.9csxet.cn

================================================================================
来源：http://vg.shxzukj.cn

统计汇总
来源：http://vw.shxzskj.cn

================================================================================
来源：http://nd.huanxung.cn

按语言统计（条）：
来源：http://xu.jctech888.com.cn

Python ......... 252
来源：http://vr.jianghongdianzi.cn

PHP ............ 252
来源：http://of.szxytkj.cn

JavaScript ..... 252
来源：http://ud.nicolike.cn

TypeScript ..... 212
来源：http://ay.huanxung.cn

Java ........... 212
来源：http://yq.colortex.cn

Go ............. 212
来源：http://sv.newstarts.cn

Ruby ........... 212
来源：http://rm.shtwfgs.cn

C# ............. 212
来源：http://fz.nicolike.cn

C .............. 30
来源：http://bv.asd995.cn

C++ ............ 30
来源：http://ji.wgjwhj.cn

SQL ............ 90
来源：http://bp.shxzukj.cn

Bash ........... 80
来源：http://jb.yuntaijiaju.cn

Kotlin ......... 15
来源：http://vr.shxzskj.cn

Swift .......... 15
来源：http://cb.asd995.cn

Lua ............ 10
来源：http://au.lnxyls.cn

Perl ........... 10
来源：http://uv.panjiajie.cn

Scala .......... 10
来源：http://pm.chemitech.net.cn

------------------------------------
来源：http://bx.gzmigu.cn

合计 ........... 2106 条
来源：http://os.chemitech.net.cn

按章节统计：
来源：http://dp.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://se.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kk.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://av.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pk.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ki.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oa.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sg.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://no.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ab.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mh.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uh.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://na.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ma.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vx.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qa.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://va.hnjuh.cn

Q SQL 专题                              90
来源：http://vb.nicolike.cn

R Bash 专题                             80
来源：http://yv.521024.cn

S C / C++ 专题                          60
来源：http://zo.huanxung.cn

T 其他语言补充                          60
来源：http://aj.colortex.cn

U 高频实用片段                         120
来源：http://ng.chemitech.net.cn

------------------------------------
来源：http://gb.bjjhwx.cn

合计                                  2106 条
来源：http://lu.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://ks.asd995.cn

使用提醒
来源：http://ud.521024.cn

--------------------------------------------------------------------------------
来源：http://ch.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zc.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eg.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cl.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mf.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eo.huanxung.cn

—— 文件结束 ——
来源：http://lw.szsharing.cn

================================================================================
来源：http://sy.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://zi.huanxung.cn

Common Programming Examples Cheat Book
来源：http://ji.muxihuayi.cn

================================================================================
来源：http://dz.shxzukj.cn

【收录内容】
来源：http://kz.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nj.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hq.hahajie.cn

SQL · Bash · C · C++
来源：http://vq.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qt.nicolike.cn

【使用说明】
来源：http://ax.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ff.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kn.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ua.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sm.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mj.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ft.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://za.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://db.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fh.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ff.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zs.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ii.asd995.cn

【文件统计】
来源：http://rv.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ed.newstarts.cn

--------------------------------------------------------------------------------
来源：http://lh.bookmarksfly.cn

目  录
来源：http://zl.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://oz.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tk.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sn.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ng.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ou.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://al.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zb.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://un.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hw.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://th.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lw.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://le.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jq.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ct.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sj.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lq.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bu.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tg.521024.cn


<!-- 参考信息 -->