代发 wailian999

[U17] Py：初始化日志
来源：http://zt.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://qw.hnjuh.cn

[U18] Py：预编译正则
来源：http://ee.colortex.cn

pat = re.compile(r"\d+")
来源：http://wk.nicolike.cn

[U19] Py：正则替换带回调
来源：http://ab.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://id.szsharing.cn

[U20] Py：缓存函数结果
来源：http://fm.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://xp.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://kl.huixiangedu.cn

@contextlib.contextmanager
来源：http://nl.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://la.huixinmuqiang.cn

list(zip(*m))
来源：http://el.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://mm.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ql.newstarts.cn

[U24] Py：路径操作
来源：http://bx.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ur.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://el.haigaiapp.cn

csv.DictReader(f)
来源：http://ys.szxytkj.cn

[U26] Py：并发下载
来源：http://ph.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vg.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://qc.muxihuayi.cn

aiohttp.ClientSession() 配合 async with
来源：http://aw.hnjuh.cn

[U28] Py：类型别名
来源：http://nw.gzmigu.cn

UserId = int
来源：http://ol.huanxung.cn

[U29] Py：属性校验
来源：http://lh.huanxung.cn

@property 与 @x.setter 配合
来源：http://bc.jctech888.com.cn

[U30] Py：数据类
来源：http://zv.shtwfgs.cn

@dataclass(slots=True)
来源：http://vp.nszjky.cn

[U31] Py：单测
来源：http://ex.wgjwhj.cn

python -m pytest -q
来源：http://kq.wgjwhj.cn

[U32] Py：代码格式化
来源：http://qr.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ny.wgjwhj.cn

[U33] Py：打包发布
来源：http://cl.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://tp.newstarts.cn

[U34] Py：判断编码
来源：http://ay.asd995.cn

chardet.detect(raw)
来源：http://ew.huixiangedu.cn

[U35] Py：发送邮件
来源：http://eb.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xv.asd995.cn

[U36] Py：定时任务
来源：http://zx.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://sy.hahajie.cn

[U37] Py：读写 Excel
来源：http://gv.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gy.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://wt.gzmigu.cn

Path(__file__).resolve().parent
来源：http://ck.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://hi.bookmarksfly.cn

sys.stdout.isatty()
来源：http://po.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://ex.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://dt.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://xb.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ia.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://mn.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iq.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://un.huixinmuqiang.cn

namespace App\Http;
来源：http://ak.nicolike.cn

[U44] PHP：开启严格类型
来源：http://hl.lnxyls.cn

declare(strict_types=1);
来源：http://dt.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://fo.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://le.lnxyls.cn

[U46] PHP：可空类型
来源：http://kb.haigaiapp.cn

?string $name = null
来源：http://xj.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://kx.yuntaijiaju.cn

int|string $id
来源：http://qv.nicolike.cn

[U48] PHP：纯枚举
来源：http://tj.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cp.shxzukj.cn

[U49] PHP：只读属性
来源：http://yt.bookmarksfly.cn

public readonly string $name
来源：http://qz.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://sw.9csxet.cn

public function __construct(private int $id) {}
来源：http://pf.szsharing.cn

[U51] PHP：数组解构
来源：http://lc.chemitech.net.cn

[$a, $b] = $arr;
来源：http://vz.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://ms.wgjwhj.cn

$double = fn($x) => $x * 2;
来源：http://cp.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://jy.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://he.asd995.cn

[U54] PHP：空安全调用
来源：http://ny.colortex.cn

$obj?->method()
来源：http://uq.asd995.cn

[U55] PHP：match 表达式
来源：http://np.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ee.shxzukj.cn

[U56] PHP：命名参数
来源：http://rz.asd995.cn

f(a: 1, b: 2)
来源：http://ax.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://sb.shtwfgs.cn

"值: {$a}"
来源：http://bz.lnxyls.cn

[U58] PHP：数组三件套
来源：http://pe.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ew.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://zi.colortex.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sa.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://qp.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lc.shxzukj.cn

[U61] PHP：正则
来源：http://xn.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ch.huanxung.cn

[U62] PHP：日期对象
来源：http://ix.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zn.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://zl.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dk.shxzskj.cn

[U64] PHP：目录遍历
来源：http://mk.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://zf.szsharing.cn

[U65] PHP：会话
来源：http://yh.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hw.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://pn.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ke.521024.cn

[U67] PHP：处理文件上传
来源：http://cd.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oh.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ek.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eo.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://nn.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dq.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://up.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ni.chemitech.net.cn

[U71] PHP：抛出异常
来源：http://tc.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://gl.hahajie.cn

[U72] PHP：写错误日志
来源：http://ds.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://de.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://lf.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://vh.haigaiapp.cn

[U74] PHP：读取环境变量
来源：http://ae.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://tz.hnjuh.cn

[U75] PHP：依赖注入
来源：http://bb.shxzukj.cn

composer require psr/container
来源：http://cs.szxytkj.cn

[U76] PHP：简单路由
来源：http://fw.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fu.gzmigu.cn

[U77] PHP：模板渲染
来源：http://jc.yuntaijiaju.cn

composer require twig/twig
来源：http://qs.bjjhwx.cn

[U78] PHP：单元测试
来源：http://uj.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://ef.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://fg.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://gh.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://zl.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kv.521024.cn

[U81] JS：初始化项目
来源：http://cj.huixiangedu.cn

npm init -y;  npm i express
来源：http://sb.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://ei.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qr.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://gb.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mp.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://zp.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gc.haigaiapp.cn

[U85] JS：可选链
来源：http://mw.shxzukj.cn

a?.b?.c
来源：http://yx.9csxet.cn

[U86] JS：空值合并
来源：http://th.asd995.cn

a ?? b
来源：http://te.newstarts.cn

[U87] JS：解构默认值
来源：http://ax.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://ct.shxzukj.cn

[U88] JS：对象展开合并
来源：http://ar.muxihuayi.cn

{ ...a, ...b }
来源：http://hu.gzmigu.cn

[U89] JS：数组去重
来源：http://ux.shxzukj.cn

[...new Set(arr)]
来源：http://ra.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://ew.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://jf.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://zz.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xd.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://wf.haigaiapp.cn

structuredClone(obj)
来源：http://rw.hnjuh.cn

[U93] JS：模板字符串
来源：http://bf.nszjky.cn

`共 ${n} 条`
来源：http://jx.huixiangedu.cn

[U94] JS：箭头函数
来源：http://mf.nicolike.cn

const double = x => x * 2;
来源：http://sy.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://mb.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://cc.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://na.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sl.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://kf.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lw.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://ir.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nz.shtwfgs.cn

[U99] JS：事件监听
来源：http://ut.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://xp.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://cl.nicolike.cn

document.querySelector(".item")
来源：http://wq.bjjhwx.cn

[U101] JS：classList 操作
来源：http://pm.jctech888.com.cn

el.classList.toggle("active")
来源：http://ka.huixiangedu.cn

[U102] JS：本地存储
来源：http://xs.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vg.asd995.cn

[U103] JS：定时器
来源：http://js.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tq.newstarts.cn

[U104] JS：防抖
来源：http://oa.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sq.hnjuh.cn

[U105] JS：节流
来源：http://hn.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sm.nszjky.cn

[U106] JS：日期格式化
来源：http://le.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rt.colortex.cn

[U107] JS：数字千分位
来源：http://gd.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ve.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://vi.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ts.hnjuh.cn

[U109] JS：数组分组
来源：http://tc.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://ds.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://qr.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nq.szxytkj.cn

[U111] JS：对象转 Map
来源：http://ry.colortex.cn

new Map(Object.entries(obj))
来源：http://mn.newstarts.cn

[U112] JS：字符串补位
来源：http://au.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://wz.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://br.bookmarksfly.cn

s.replaceAll("a", "b")
来源：http://df.szsharing.cn

[U114] JS：JSON 深比较
来源：http://hw.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jl.szsharing.cn

[U115] JS：生成 UUID
来源：http://ib.yuexingan06.cn

crypto.randomUUID()
来源：http://it.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://dg.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://jv.asd995.cn

[U117] JS：单元测试
来源：http://bk.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://pv.yuexingan06.cn

[U118] JS：开发服务器
来源：http://ab.newstarts.cn

npm i -D vite;  npx vite
来源：http://ax.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://wn.muxihuayi.cn

npx vite build
来源：http://ap.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ic.shtwfgs.cn

import.meta.env.VITE_API_URL
来源：http://lo.9csxet.cn

================================================================================
来源：http://nk.yuntaijiaju.cn

统计汇总
来源：http://yj.hahajie.cn

================================================================================
来源：http://fc.szsharing.cn

按语言统计（条）：
来源：http://oa.shtwfgs.cn

Python ......... 252
来源：http://vx.nszjky.cn

PHP ............ 252
来源：http://yf.muxihuayi.cn

JavaScript ..... 252
来源：http://nj.shxzukj.cn

TypeScript ..... 212
来源：http://kq.yuexingan06.cn

Java ........... 212
来源：http://mp.newstarts.cn

Go ............. 212
来源：http://ap.bookmarksfly.cn

Ruby ........... 212
来源：http://fr.shtwfgs.cn

C# ............. 212
来源：http://ed.jianghongdianzi.cn

C .............. 30
来源：http://rw.haigaiapp.cn

C++ ............ 30
来源：http://tt.shxzskj.cn

SQL ............ 90
来源：http://qy.szxytkj.cn

Bash ........... 80
来源：http://fy.panjiajie.cn

Kotlin ......... 15
来源：http://wz.nszjky.cn

Swift .......... 15
来源：http://ae.gzmigu.cn

Lua ............ 10
来源：http://qx.asd995.cn

Perl ........... 10
来源：http://ct.asd995.cn

Scala .......... 10
来源：http://fd.szxytkj.cn

------------------------------------
来源：http://cz.szsharing.cn

合计 ........... 2106 条
来源：http://rc.yuntaijiaju.cn

按章节统计：
来源：http://jh.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://di.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cf.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://md.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sf.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nb.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dn.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yr.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qd.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jl.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ih.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://av.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xc.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tv.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tn.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ru.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ed.shxzukj.cn

Q SQL 专题                              90
来源：http://wg.hnjuh.cn

R Bash 专题                             80
来源：http://ik.chemitech.net.cn

S C / C++ 专题                          60
来源：http://js.newstarts.cn

T 其他语言补充                          60
来源：http://hm.shxzukj.cn

U 高频实用片段                         120
来源：http://yf.jctech888.com.cn

------------------------------------
来源：http://yc.jianghongdianzi.cn

合计                                  2106 条
来源：http://tn.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://bh.gzmigu.cn

使用提醒
来源：http://cw.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ah.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xz.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tt.hahajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bx.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mo.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uc.bookmarksfly.cn

—— 文件结束 ——
来源：http://or.szxytkj.cn

================================================================================
来源：http://gt.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://kv.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://gw.shxzskj.cn

================================================================================
来源：http://wf.panjiajie.cn

【收录内容】
来源：http://en.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://al.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ch.muxihuayi.cn

SQL · Bash · C · C++
来源：http://ou.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://at.bookmarksfly.cn

【使用说明】
来源：http://we.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rg.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://au.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wp.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hv.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tl.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://db.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sq.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sa.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gd.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sr.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wb.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nr.muxihuayi.cn

【文件统计】
来源：http://yi.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bc.szsharing.cn

--------------------------------------------------------------------------------
来源：http://sf.yuntaijiaju.cn

目  录
来源：http://gi.asd995.cn

--------------------------------------------------------------------------------
来源：http://bk.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://en.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dz.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ub.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bd.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kz.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fz.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xv.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vv.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yf.nicolike.cn


<!-- 参考信息 -->