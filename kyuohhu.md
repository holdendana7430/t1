代发 wailian999

[U17] Py：初始化日志
来源：http://yo.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://xt.shxzukj.cn

[U18] Py：预编译正则
来源：http://gz.asd995.cn

pat = re.compile(r"\d+")
来源：http://hb.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://ac.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iy.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://hw.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ro.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://da.jctech888.com.cn

@contextlib.contextmanager
来源：http://uz.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://jq.newstarts.cn

list(zip(*m))
来源：http://ka.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://ag.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://td.asd995.cn

[U24] Py：路径操作
来源：http://ab.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ca.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://ea.jctech888.com.cn

csv.DictReader(f)
来源：http://vs.haigaiapp.cn

[U26] Py：并发下载
来源：http://qc.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pb.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://cz.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://xz.panjiajie.cn

[U28] Py：类型别名
来源：http://xm.hahajie.cn

UserId = int
来源：http://ci.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://nh.nszjky.cn

@property 与 @x.setter 配合
来源：http://mt.shxzskj.cn

[U30] Py：数据类
来源：http://pz.huixiangedu.cn

@dataclass(slots=True)
来源：http://oz.gzmigu.cn

[U31] Py：单测
来源：http://xx.bookmarksfly.cn

python -m pytest -q
来源：http://la.huanxung.cn

[U32] Py：代码格式化
来源：http://kd.nszjky.cn

ruff format . && ruff check --fix .
来源：http://wn.haigaiapp.cn

[U33] Py：打包发布
来源：http://gx.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://cg.asd995.cn

[U34] Py：判断编码
来源：http://bc.haigaiapp.cn

chardet.detect(raw)
来源：http://oi.gzmigu.cn

[U35] Py：发送邮件
来源：http://xz.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fd.panjiajie.cn

[U36] Py：定时任务
来源：http://np.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://xj.lnxyls.cn

[U37] Py：读写 Excel
来源：http://dh.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lr.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://ed.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://zn.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://ga.huanxung.cn

sys.stdout.isatty()
来源：http://gr.521024.cn

[U40] Py：打印到标准错误
来源：http://oe.panjiajie.cn

print("err", file=sys.stderr)
来源：http://qn.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://jv.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ed.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://qh.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ji.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://yl.muxihuayi.cn

namespace App\Http;
来源：http://yn.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://hh.asd995.cn

declare(strict_types=1);
来源：http://tl.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://ia.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.nszjky.cn

[U46] PHP：可空类型
来源：http://od.bjjhwx.cn

?string $name = null
来源：http://lc.9csxet.cn

[U47] PHP：联合类型
来源：http://hu.nszjky.cn

int|string $id
来源：http://bk.huanxung.cn

[U48] PHP：纯枚举
来源：http://ie.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bh.jctech888.com.cn

[U49] PHP：只读属性
来源：http://yb.nicolike.cn

public readonly string $name
来源：http://ae.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://yi.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://fo.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ct.bjjhwx.cn

[$a, $b] = $arr;
来源：http://vx.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://cl.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://yk.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://lu.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://lc.lnxyls.cn

[U54] PHP：空安全调用
来源：http://oy.hahajie.cn

$obj?->method()
来源：http://gp.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://wn.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lr.nszjky.cn

[U56] PHP：命名参数
来源：http://jr.muxihuayi.cn

f(a: 1, b: 2)
来源：http://vj.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://hb.bookmarksfly.cn

"值: {$a}"
来源：http://lj.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://uq.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ln.nszjky.cn

[U59] PHP：自定义排序
来源：http://ob.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ge.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://ks.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yv.newstarts.cn

[U61] PHP：正则
来源：http://lo.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cb.9csxet.cn

[U62] PHP：日期对象
来源：http://zb.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rt.muxihuayi.cn

[U63] PHP：文件读写
来源：http://zu.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qg.newstarts.cn

[U64] PHP：目录遍历
来源：http://em.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://to.521024.cn

[U65] PHP：会话
来源：http://ri.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dj.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://ic.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sj.szsharing.cn

[U67] PHP：处理文件上传
来源：http://zf.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rm.huanxung.cn

[U68] PHP：PDO 连接
来源：http://kc.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ts.hnjuh.cn

[U69] PHP：PDO 预处理
来源：http://rz.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wy.521024.cn

[U70] PHP：PDO 事务
来源：http://kk.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yz.lnxyls.cn

[U71] PHP：抛出异常
来源：http://ir.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://tc.newstarts.cn

[U72] PHP：写错误日志
来源：http://dn.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://tw.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://lz.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://fd.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://fv.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://nb.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://tx.hnjuh.cn

composer require psr/container
来源：http://fg.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://gz.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iq.shxzukj.cn

[U77] PHP：模板渲染
来源：http://oa.haigaiapp.cn

composer require twig/twig
来源：http://vf.huanxung.cn

[U78] PHP：单元测试
来源：http://up.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://wh.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ig.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://oz.colortex.cn

[U80] PHP：代码规范修复
来源：http://va.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hb.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://bo.shxzukj.cn

npm init -y;  npm i express
来源：http://as.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://fv.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yy.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://ao.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yh.colortex.cn

[U84] JS：CommonJS 写法
来源：http://fw.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rj.shtwfgs.cn

[U85] JS：可选链
来源：http://ds.hnjuh.cn

a?.b?.c
来源：http://kd.gzmigu.cn

[U86] JS：空值合并
来源：http://is.hahajie.cn

a ?? b
来源：http://ix.asd995.cn

[U87] JS：解构默认值
来源：http://ai.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://mh.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://bj.nszjky.cn

{ ...a, ...b }
来源：http://ci.huixiangedu.cn

[U89] JS：数组去重
来源：http://rv.nicolike.cn

[...new Set(arr)]
来源：http://ea.gzmigu.cn

[U90] JS：数字数组排序
来源：http://zr.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://xp.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://zh.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ul.wgjwhj.cn

[U92] JS：深拷贝
来源：http://rr.chemitech.net.cn

structuredClone(obj)
来源：http://yv.shtwfgs.cn

[U93] JS：模板字符串
来源：http://yn.huixiangedu.cn

`共 ${n} 条`
来源：http://cm.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://hg.shxzukj.cn

const double = x => x * 2;
来源：http://ku.9csxet.cn

[U95] JS：Promise 包装
来源：http://zc.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://si.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://xr.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dz.gzmigu.cn

[U97] JS：并发请求
来源：http://bx.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zg.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://av.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pk.shxzskj.cn

[U99] JS：事件监听
来源：http://ox.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://wn.shxzskj.cn

[U100] JS：DOM 查询
来源：http://an.haigaiapp.cn

document.querySelector(".item")
来源：http://qe.bjjhwx.cn

[U101] JS：classList 操作
来源：http://kb.wgjwhj.cn

el.classList.toggle("active")
来源：http://me.gzmigu.cn

[U102] JS：本地存储
来源：http://da.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hb.huixinmuqiang.cn

[U103] JS：定时器
来源：http://jr.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zr.huixinmuqiang.cn

[U104] JS：防抖
来源：http://op.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ge.yuexingan06.cn

[U105] JS：节流
来源：http://fy.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fu.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://cq.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bc.nicolike.cn

[U107] JS：数字千分位
来源：http://hm.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mu.huixiangedu.cn

[U108] JS：随机整数
来源：http://uo.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bl.521024.cn

[U109] JS：数组分组
来源：http://eb.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://xu.colortex.cn

[U110] JS：数组分块
来源：http://lx.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cs.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://vi.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://ji.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://rm.huixiangedu.cn

"7".padStart(3, "0")
来源：http://bc.gzmigu.cn

[U113] JS：正则替换全部
来源：http://nd.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://wh.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://ct.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qz.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://nh.jctech888.com.cn

crypto.randomUUID()
来源：http://ot.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://ac.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://dy.colortex.cn

[U117] JS：单元测试
来源：http://pv.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://dj.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://rl.9csxet.cn

npm i -D vite;  npx vite
来源：http://xz.asd995.cn

[U119] JS：生产构建
来源：http://yu.shtwfgs.cn

npx vite build
来源：http://tc.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ug.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://mc.panjiajie.cn

================================================================================
来源：http://ho.jianghongdianzi.cn

统计汇总
来源：http://ep.bjjhwx.cn

================================================================================
来源：http://rq.huixinmuqiang.cn

按语言统计（条）：
来源：http://ki.yuntaijiaju.cn

Python ......... 252
来源：http://oh.hnjuh.cn

PHP ............ 252
来源：http://ps.gzmigu.cn

JavaScript ..... 252
来源：http://gz.nicolike.cn

TypeScript ..... 212
来源：http://br.yuntaijiaju.cn

Java ........... 212
来源：http://no.shxzskj.cn

Go ............. 212
来源：http://tj.bookmarksfly.cn

Ruby ........... 212
来源：http://cq.huanxung.cn

C# ............. 212
来源：http://iy.hahajie.cn

C .............. 30
来源：http://zx.szxytkj.cn

C++ ............ 30
来源：http://pw.bookmarksfly.cn

SQL ............ 90
来源：http://zl.newstarts.cn

Bash ........... 80
来源：http://wt.huanxung.cn

Kotlin ......... 15
来源：http://jy.jianghongdianzi.cn

Swift .......... 15
来源：http://as.521024.cn

Lua ............ 10
来源：http://nu.hahajie.cn

Perl ........... 10
来源：http://au.521024.cn

Scala .......... 10
来源：http://wu.huanxung.cn

------------------------------------
来源：http://mk.nszjky.cn

合计 ........... 2106 条
来源：http://ea.shtwfgs.cn

按章节统计：
来源：http://kk.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ya.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jm.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fh.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://co.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oy.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ba.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xc.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ki.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bu.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mg.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qi.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ld.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qk.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vu.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cz.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ys.jctech888.com.cn

Q SQL 专题                              90
来源：http://jj.muxihuayi.cn

R Bash 专题                             80
来源：http://ff.huixiangedu.cn

S C / C++ 专题                          60
来源：http://qk.nicolike.cn

T 其他语言补充                          60
来源：http://eh.yuexingan06.cn

U 高频实用片段                         120
来源：http://hr.colortex.cn

------------------------------------
来源：http://xo.9csxet.cn

合计                                  2106 条
来源：http://yb.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://zz.lnxyls.cn

使用提醒
来源：http://ty.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://kw.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ca.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nj.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vw.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dj.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ea.9csxet.cn

—— 文件结束 ——
来源：http://ir.hahajie.cn

================================================================================
来源：http://vz.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://bh.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://mu.hahajie.cn

【收录内容】
来源：http://qb.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nj.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tv.colortex.cn

SQL · Bash · C · C++
来源：http://xf.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sq.9csxet.cn

【使用说明】
来源：http://jc.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ow.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cd.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qg.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wx.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://av.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jl.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bt.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oq.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uf.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rr.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://um.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fx.szxytkj.cn

【文件统计】
来源：http://yh.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ks.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ip.jianghongdianzi.cn

目  录
来源：http://or.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ge.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ad.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ej.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dw.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ok.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aq.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://if.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hh.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ly.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ak.shxzukj.cn


<!-- 参考信息 -->