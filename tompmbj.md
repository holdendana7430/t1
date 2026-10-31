代发 wailian999

[U17] Py：初始化日志
来源：http://ed.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://it.huanxung.cn

[U18] Py：预编译正则
来源：http://ye.huanxung.cn

pat = re.compile(r"\d+")
来源：http://hy.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://di.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kd.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://on.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://qz.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://bu.szsharing.cn

@contextlib.contextmanager
来源：http://gj.521024.cn

[U22] Py：矩阵转置
来源：http://pr.huixiangedu.cn

list(zip(*m))
来源：http://fx.asd995.cn

[U23] Py：分块读取大文件
来源：http://qr.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vw.wgjwhj.cn

[U24] Py：路径操作
来源：http://ff.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wm.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://gm.nicolike.cn

csv.DictReader(f)
来源：http://he.bookmarksfly.cn

[U26] Py：并发下载
来源：http://kk.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mw.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://ni.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://zr.nszjky.cn

[U28] Py：类型别名
来源：http://ur.chemitech.net.cn

UserId = int
来源：http://xn.panjiajie.cn

[U29] Py：属性校验
来源：http://ot.szxytkj.cn

@property 与 @x.setter 配合
来源：http://ao.szsharing.cn

[U30] Py：数据类
来源：http://av.hnjuh.cn

@dataclass(slots=True)
来源：http://zu.nszjky.cn

[U31] Py：单测
来源：http://cg.asd995.cn

python -m pytest -q
来源：http://yb.521024.cn

[U32] Py：代码格式化
来源：http://jy.asd995.cn

ruff format . && ruff check --fix .
来源：http://pp.nicolike.cn

[U33] Py：打包发布
来源：http://ym.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://wn.haigaiapp.cn

[U34] Py：判断编码
来源：http://wy.jianghongdianzi.cn

chardet.detect(raw)
来源：http://gm.newstarts.cn

[U35] Py：发送邮件
来源：http://by.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zc.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://gh.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ki.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://uf.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ha.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://hd.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ks.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://mh.huixiangedu.cn

sys.stdout.isatty()
来源：http://qh.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://px.shxzskj.cn

print("err", file=sys.stderr)
来源：http://tp.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://jn.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qk.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ow.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dx.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://nn.9csxet.cn

namespace App\Http;
来源：http://uk.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://cj.gzmigu.cn

declare(strict_types=1);
来源：http://mn.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://my.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.asd995.cn

[U46] PHP：可空类型
来源：http://dc.nszjky.cn

?string $name = null
来源：http://pb.wgjwhj.cn

[U47] PHP：联合类型
来源：http://rw.huixiangedu.cn

int|string $id
来源：http://th.hnjuh.cn

[U48] PHP：纯枚举
来源：http://fa.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sc.panjiajie.cn

[U49] PHP：只读属性
来源：http://vb.jctech888.com.cn

public readonly string $name
来源：http://ot.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://zq.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://zb.jctech888.com.cn

[U51] PHP：数组解构
来源：http://cj.haigaiapp.cn

[$a, $b] = $arr;
来源：http://mm.521024.cn

[U52] PHP：箭头函数
来源：http://wz.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://jc.asd995.cn

[U53] PHP：空合并运算符
来源：http://yo.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://as.nszjky.cn

[U54] PHP：空安全调用
来源：http://xu.lnxyls.cn

$obj?->method()
来源：http://fc.nicolike.cn

[U55] PHP：match 表达式
来源：http://wd.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xq.huanxung.cn

[U56] PHP：命名参数
来源：http://kt.huixiangedu.cn

f(a: 1, b: 2)
来源：http://di.asd995.cn

[U57] PHP：字符串插值
来源：http://ue.521024.cn

"值: {$a}"
来源：http://nv.colortex.cn

[U58] PHP：数组三件套
来源：http://gf.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ir.hahajie.cn

[U59] PHP：自定义排序
来源：http://jt.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lz.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://oa.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ud.panjiajie.cn

[U61] PHP：正则
来源：http://xg.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xe.521024.cn

[U62] PHP：日期对象
来源：http://dy.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wj.szsharing.cn

[U63] PHP：文件读写
来源：http://gr.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vm.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://jj.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://nu.bookmarksfly.cn

[U65] PHP：会话
来源：http://eu.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pb.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://bf.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xx.9csxet.cn

[U67] PHP：处理文件上传
来源：http://go.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dm.hahajie.cn

[U68] PHP：PDO 连接
来源：http://hm.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fk.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://cz.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nk.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://bm.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ky.colortex.cn

[U71] PHP：抛出异常
来源：http://oz.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://dy.colortex.cn

[U72] PHP：写错误日志
来源：http://sv.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://ce.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://le.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://ms.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://wh.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://mp.szsharing.cn

[U75] PHP：依赖注入
来源：http://qu.colortex.cn

composer require psr/container
来源：http://hd.szxytkj.cn

[U76] PHP：简单路由
来源：http://ob.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kl.asd995.cn

[U77] PHP：模板渲染
来源：http://qk.yuexingan06.cn

composer require twig/twig
来源：http://ak.chemitech.net.cn

[U78] PHP：单元测试
来源：http://qv.521024.cn

composer require --dev phpunit/phpunit
来源：http://fj.hnjuh.cn

[U79] PHP：静态分析
来源：http://vs.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://ta.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://qx.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wl.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://pm.521024.cn

npm init -y;  npm i express
来源：http://kc.newstarts.cn

[U82] JS：package.json 脚本
来源：http://oe.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oj.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ak.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://op.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://uj.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ht.shxzukj.cn

[U85] JS：可选链
来源：http://pw.yuntaijiaju.cn

a?.b?.c
来源：http://gq.nszjky.cn

[U86] JS：空值合并
来源：http://vz.jctech888.com.cn

a ?? b
来源：http://gz.shxzukj.cn

[U87] JS：解构默认值
来源：http://eo.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://dd.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://qu.lnxyls.cn

{ ...a, ...b }
来源：http://ps.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://vr.chemitech.net.cn

[...new Set(arr)]
来源：http://xr.colortex.cn

[U90] JS：数字数组排序
来源：http://dt.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://rc.huanxung.cn

[U91] JS：对象键值遍历
来源：http://qf.jianghongdianzi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eh.shtwfgs.cn

[U92] JS：深拷贝
来源：http://we.bookmarksfly.cn

structuredClone(obj)
来源：http://jl.521024.cn

[U93] JS：模板字符串
来源：http://bm.hahajie.cn

`共 ${n} 条`
来源：http://cv.haigaiapp.cn

[U94] JS：箭头函数
来源：http://bx.shxzskj.cn

const double = x => x * 2;
来源：http://eo.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://sc.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://bv.nicolike.cn

[U96] JS：async/await 与异常
来源：http://hy.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bi.521024.cn

[U97] JS：并发请求
来源：http://hp.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iv.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ra.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://if.yuexingan06.cn

[U99] JS：事件监听
来源：http://bq.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://sq.521024.cn

[U100] JS：DOM 查询
来源：http://fe.szsharing.cn

document.querySelector(".item")
来源：http://mi.lnxyls.cn

[U101] JS：classList 操作
来源：http://zp.asd995.cn

el.classList.toggle("active")
来源：http://fa.szxytkj.cn

[U102] JS：本地存储
来源：http://lz.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ri.muxihuayi.cn

[U103] JS：定时器
来源：http://vb.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ur.yuntaijiaju.cn

[U104] JS：防抖
来源：http://cc.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.yuntaijiaju.cn

[U105] JS：节流
来源：http://yo.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dm.hnjuh.cn

[U106] JS：日期格式化
来源：http://gy.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jf.muxihuayi.cn

[U107] JS：数字千分位
来源：http://ng.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pu.jctech888.com.cn

[U108] JS：随机整数
来源：http://zk.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kb.nicolike.cn

[U109] JS：数组分组
来源：http://wn.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://bn.shtwfgs.cn

[U110] JS：数组分块
来源：http://lj.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hy.shxzukj.cn

[U111] JS：对象转 Map
来源：http://hr.hahajie.cn

new Map(Object.entries(obj))
来源：http://kg.szsharing.cn

[U112] JS：字符串补位
来源：http://zj.lnxyls.cn

"7".padStart(3, "0")
来源：http://py.colortex.cn

[U113] JS：正则替换全部
来源：http://ci.hahajie.cn

s.replaceAll("a", "b")
来源：http://jq.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://ad.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eo.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://oq.nicolike.cn

crypto.randomUUID()
来源：http://hz.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://mj.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://ke.shtwfgs.cn

[U117] JS：单元测试
来源：http://tm.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://uy.colortex.cn

[U118] JS：开发服务器
来源：http://bm.colortex.cn

npm i -D vite;  npx vite
来源：http://uc.szxytkj.cn

[U119] JS：生产构建
来源：http://qo.bjjhwx.cn

npx vite build
来源：http://xx.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://zl.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://pr.chemitech.net.cn

================================================================================
来源：http://zy.bookmarksfly.cn

统计汇总
来源：http://ut.9csxet.cn

================================================================================
来源：http://st.asd995.cn

按语言统计（条）：
来源：http://kj.asd995.cn

Python ......... 252
来源：http://uj.jianghongdianzi.cn

PHP ............ 252
来源：http://ae.shxzskj.cn

JavaScript ..... 252
来源：http://ra.chemitech.net.cn

TypeScript ..... 212
来源：http://yu.huanxung.cn

Java ........... 212
来源：http://fm.chemitech.net.cn

Go ............. 212
来源：http://yk.lnxyls.cn

Ruby ........... 212
来源：http://rt.nszjky.cn

C# ............. 212
来源：http://bf.bookmarksfly.cn

C .............. 30
来源：http://vg.panjiajie.cn

C++ ............ 30
来源：http://hl.colortex.cn

SQL ............ 90
来源：http://eb.panjiajie.cn

Bash ........... 80
来源：http://mh.521024.cn

Kotlin ......... 15
来源：http://be.jianghongdianzi.cn

Swift .......... 15
来源：http://hu.bjjhwx.cn

Lua ............ 10
来源：http://yd.hnjuh.cn

Perl ........... 10
来源：http://zb.bookmarksfly.cn

Scala .......... 10
来源：http://tj.szsharing.cn

------------------------------------
来源：http://ku.asd995.cn

合计 ........... 2106 条
来源：http://rm.jianghongdianzi.cn

按章节统计：
来源：http://al.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mr.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zc.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ma.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cg.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hj.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zr.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gz.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ov.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xw.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://so.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dy.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nk.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gx.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lz.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://up.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eb.huixiangedu.cn

Q SQL 专题                              90
来源：http://vi.szxytkj.cn

R Bash 专题                             80
来源：http://gv.gzmigu.cn

S C / C++ 专题                          60
来源：http://ch.huixiangedu.cn

T 其他语言补充                          60
来源：http://mq.bookmarksfly.cn

U 高频实用片段                         120
来源：http://fu.jianghongdianzi.cn

------------------------------------
来源：http://nj.huanxung.cn

合计                                  2106 条
来源：http://mx.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ce.jctech888.com.cn

使用提醒
来源：http://cz.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://pj.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hl.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nx.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xb.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sp.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dg.newstarts.cn

—— 文件结束 ——
来源：http://te.muxihuayi.cn

================================================================================
来源：http://wh.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://gu.hahajie.cn

Common Programming Examples Cheat Book
来源：http://uy.lnxyls.cn

================================================================================
来源：http://dm.shxzukj.cn

【收录内容】
来源：http://bc.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pj.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xz.yuexingan06.cn

SQL · Bash · C · C++
来源：http://vl.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mk.yuntaijiaju.cn

【使用说明】
来源：http://pu.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hl.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ea.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cc.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vv.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://of.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bk.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qd.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tv.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://om.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://on.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zb.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aj.huixiangedu.cn

【文件统计】
来源：http://jd.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qk.hahajie.cn

--------------------------------------------------------------------------------
来源：http://bn.lnxyls.cn

目  录
来源：http://bg.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ku.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wk.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pp.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vb.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ln.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qx.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gr.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bn.521024.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://px.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://el.bjjhwx.cn


<!-- 参考信息 -->