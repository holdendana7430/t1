代发 wailian999

[U13] Py：固定长度队列
来源：http://ua.nszjky.cn

deque(maxlen=10)
来源：http://ji.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://ec.huixinmuqiang.cn

defaultdict(list)
来源：http://bw.asd995.cn

[U15] Py：高精度计时
来源：http://pn.bookmarksfly.cn

t = time.perf_counter()
来源：http://hw.huanxung.cn

[U16] Py：命令行参数解析
来源：http://rn.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fj.wgjwhj.cn

[U17] Py：初始化日志
来源：http://we.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ld.shtwfgs.cn

[U18] Py：预编译正则
来源：http://il.9csxet.cn

pat = re.compile(r"\d+")
来源：http://ji.521024.cn

[U19] Py：正则替换带回调
来源：http://fr.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uw.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://ad.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://al.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://ze.yuexingan06.cn

@contextlib.contextmanager
来源：http://md.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://jo.hnjuh.cn

list(zip(*m))
来源：http://mb.huanxung.cn

[U23] Py：分块读取大文件
来源：http://nz.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qd.asd995.cn

[U24] Py：路径操作
来源：http://sz.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yr.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://tg.huanxung.cn

csv.DictReader(f)
来源：http://hp.hahajie.cn

[U26] Py：并发下载
来源：http://so.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ic.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://rq.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://jw.bookmarksfly.cn

[U28] Py：类型别名
来源：http://nf.huixinmuqiang.cn

UserId = int
来源：http://gc.newstarts.cn

[U29] Py：属性校验
来源：http://ut.colortex.cn

@property 与 @x.setter 配合
来源：http://ei.newstarts.cn

[U30] Py：数据类
来源：http://zi.jctech888.com.cn

@dataclass(slots=True)
来源：http://gt.yuntaijiaju.cn

[U31] Py：单测
来源：http://wb.shxzskj.cn

python -m pytest -q
来源：http://rq.colortex.cn

[U32] Py：代码格式化
来源：http://fh.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://pj.shxzukj.cn

[U33] Py：打包发布
来源：http://lz.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://om.lnxyls.cn

[U34] Py：判断编码
来源：http://ci.521024.cn

chardet.detect(raw)
来源：http://hz.shtwfgs.cn

[U35] Py：发送邮件
来源：http://my.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ho.jctech888.com.cn

[U36] Py：定时任务
来源：http://tm.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://bo.9csxet.cn

[U37] Py：读写 Excel
来源：http://dz.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mf.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://hg.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://da.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://qb.521024.cn

sys.stdout.isatty()
来源：http://xa.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://vo.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://vb.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://ft.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://md.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://ds.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ax.asd995.cn

[U43] PHP：声明命名空间
来源：http://bb.jianghongdianzi.cn

namespace App\Http;
来源：http://hr.bjjhwx.cn

[U44] PHP：开启严格类型
来源：http://cj.huixiangedu.cn

declare(strict_types=1);
来源：http://oc.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://fq.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.gzmigu.cn

[U46] PHP：可空类型
来源：http://aw.szxytkj.cn

?string $name = null
来源：http://ze.colortex.cn

[U47] PHP：联合类型
来源：http://kx.szsharing.cn

int|string $id
来源：http://bf.shxzskj.cn

[U48] PHP：纯枚举
来源：http://wc.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sk.yuexingan06.cn

[U49] PHP：只读属性
来源：http://pf.szsharing.cn

public readonly string $name
来源：http://md.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://zo.9csxet.cn

public function __construct(private int $id) {}
来源：http://ws.nszjky.cn

[U51] PHP：数组解构
来源：http://dw.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://zi.shxzskj.cn

[U52] PHP：箭头函数
来源：http://fc.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://lh.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://wl.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://tg.gzmigu.cn

[U54] PHP：空安全调用
来源：http://oo.muxihuayi.cn

$obj?->method()
来源：http://mv.521024.cn

[U55] PHP：match 表达式
来源：http://xm.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ps.shxzukj.cn

[U56] PHP：命名参数
来源：http://qi.gzmigu.cn

f(a: 1, b: 2)
来源：http://ax.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://zq.hahajie.cn

"值: {$a}"
来源：http://xx.huanxung.cn

[U58] PHP：数组三件套
来源：http://zk.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pp.nszjky.cn

[U59] PHP：自定义排序
来源：http://or.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oa.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://pe.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ln.gzmigu.cn

[U61] PHP：正则
来源：http://yl.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ul.asd995.cn

[U62] PHP：日期对象
来源：http://xz.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xe.wgjwhj.cn

[U63] PHP：文件读写
来源：http://ez.haigaiapp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fl.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://gm.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://so.haigaiapp.cn

[U65] PHP：会话
来源：http://lf.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xw.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://kp.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sh.colortex.cn

[U67] PHP：处理文件上传
来源：http://ca.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://li.nszjky.cn

[U68] PHP：PDO 连接
来源：http://ya.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lt.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://tc.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://en.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://pp.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fs.nicolike.cn

[U71] PHP：抛出异常
来源：http://jt.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://lb.521024.cn

[U72] PHP：写错误日志
来源：http://fh.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://zi.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://lu.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://te.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://hq.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://gm.9csxet.cn

[U75] PHP：依赖注入
来源：http://nu.huixinmuqiang.cn

composer require psr/container
来源：http://yr.shtwfgs.cn

[U76] PHP：简单路由
来源：http://lp.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cv.szsharing.cn

[U77] PHP：模板渲染
来源：http://vj.shtwfgs.cn

composer require twig/twig
来源：http://do.nicolike.cn

[U78] PHP：单元测试
来源：http://yu.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://av.gzmigu.cn

[U79] PHP：静态分析
来源：http://im.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://lc.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://ps.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ao.nicolike.cn

[U81] JS：初始化项目
来源：http://ky.bookmarksfly.cn

npm init -y;  npm i express
来源：http://al.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://vt.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wm.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ky.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://px.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://rh.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ro.shxzskj.cn

[U85] JS：可选链
来源：http://ps.shxzskj.cn

a?.b?.c
来源：http://dq.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://vv.newstarts.cn

a ?? b
来源：http://xy.muxihuayi.cn

[U87] JS：解构默认值
来源：http://dg.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://nh.shxzskj.cn

[U88] JS：对象展开合并
来源：http://gm.shtwfgs.cn

{ ...a, ...b }
来源：http://fp.huanxung.cn

[U89] JS：数组去重
来源：http://zx.muxihuayi.cn

[...new Set(arr)]
来源：http://rq.szsharing.cn

[U90] JS：数字数组排序
来源：http://gh.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://ex.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://pk.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cr.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://yn.panjiajie.cn

structuredClone(obj)
来源：http://ku.muxihuayi.cn

[U93] JS：模板字符串
来源：http://jm.shxzukj.cn

`共 ${n} 条`
来源：http://gs.panjiajie.cn

[U94] JS：箭头函数
来源：http://dn.panjiajie.cn

const double = x => x * 2;
来源：http://yf.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://os.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://yf.colortex.cn

[U96] JS：async/await 与异常
来源：http://as.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mx.9csxet.cn

[U97] JS：并发请求
来源：http://at.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jm.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ac.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pl.chemitech.net.cn

[U99] JS：事件监听
来源：http://bb.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://pi.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://hr.jctech888.com.cn

document.querySelector(".item")
来源：http://qo.hnjuh.cn

[U101] JS：classList 操作
来源：http://xe.yuexingan06.cn

el.classList.toggle("active")
来源：http://yb.nszjky.cn

[U102] JS：本地存储
来源：http://nf.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://of.gzmigu.cn

[U103] JS：定时器
来源：http://pj.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zm.asd995.cn

[U104] JS：防抖
来源：http://of.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pi.521024.cn

[U105] JS：节流
来源：http://wr.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ww.bjjhwx.cn

[U106] JS：日期格式化
来源：http://kf.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wb.muxihuayi.cn

[U107] JS：数字千分位
来源：http://kj.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hb.hnjuh.cn

[U108] JS：随机整数
来源：http://mj.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iw.521024.cn

[U109] JS：数组分组
来源：http://eg.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://qx.asd995.cn

[U110] JS：数组分块
来源：http://sr.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xa.shxzskj.cn

[U111] JS：对象转 Map
来源：http://vo.szsharing.cn

new Map(Object.entries(obj))
来源：http://nn.newstarts.cn

[U112] JS：字符串补位
来源：http://ss.wgjwhj.cn

"7".padStart(3, "0")
来源：http://tq.9csxet.cn

[U113] JS：正则替换全部
来源：http://nf.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://lb.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://at.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ij.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://bb.haigaiapp.cn

crypto.randomUUID()
来源：http://cq.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://lh.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://rp.newstarts.cn

[U117] JS：单元测试
来源：http://oi.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://br.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://lm.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://zw.9csxet.cn

[U119] JS：生产构建
来源：http://oo.asd995.cn

npx vite build
来源：http://hj.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ke.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://rk.nicolike.cn

================================================================================
来源：http://qb.newstarts.cn

统计汇总
来源：http://wc.yuntaijiaju.cn

================================================================================
来源：http://xn.colortex.cn

按语言统计（条）：
来源：http://up.panjiajie.cn

Python ......... 252
来源：http://jr.huanxung.cn

PHP ............ 252
来源：http://jf.bookmarksfly.cn

JavaScript ..... 252
来源：http://od.521024.cn

TypeScript ..... 212
来源：http://dc.nicolike.cn

Java ........... 212
来源：http://ls.jctech888.com.cn

Go ............. 212
来源：http://gr.szsharing.cn

Ruby ........... 212
来源：http://wt.wgjwhj.cn

C# ............. 212
来源：http://gs.panjiajie.cn

C .............. 30
来源：http://xq.shxzskj.cn

C++ ............ 30
来源：http://te.hahajie.cn

SQL ............ 90
来源：http://hd.gzmigu.cn

Bash ........... 80
来源：http://vz.huixiangedu.cn

Kotlin ......... 15
来源：http://fj.chemitech.net.cn

Swift .......... 15
来源：http://zz.yuntaijiaju.cn

Lua ............ 10
来源：http://pm.newstarts.cn

Perl ........... 10
来源：http://ei.szxytkj.cn

Scala .......... 10
来源：http://nz.hahajie.cn

------------------------------------
来源：http://yv.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://rk.bjjhwx.cn

按章节统计：
来源：http://so.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://if.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://av.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nx.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://li.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lt.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gf.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nz.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vj.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ht.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dw.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wk.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ed.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ux.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cw.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oz.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lh.9csxet.cn

Q SQL 专题                              90
来源：http://el.shxzukj.cn

R Bash 专题                             80
来源：http://by.shtwfgs.cn

S C / C++ 专题                          60
来源：http://tn.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://ee.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://dj.yuntaijiaju.cn

------------------------------------
来源：http://up.nszjky.cn

合计                                  2106 条
来源：http://jv.hahajie.cn

--------------------------------------------------------------------------------
来源：http://mc.chemitech.net.cn

使用提醒
来源：http://sv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://rs.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://av.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ve.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ue.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mx.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fi.haigaiapp.cn

—— 文件结束 ——
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://tn.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://zg.nicolike.cn

Common Programming Examples Cheat Book
来源：http://uj.nicolike.cn

================================================================================
来源：http://wb.haigaiapp.cn

【收录内容】
来源：http://re.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bz.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nc.521024.cn

SQL · Bash · C · C++
来源：http://ry.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yf.lnxyls.cn

【使用说明】
来源：http://ef.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hr.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pa.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hb.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ib.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qf.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ws.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hy.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bi.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jh.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gj.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iw.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://js.hnjuh.cn

【文件统计】
来源：http://zw.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uq.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ii.colortex.cn

目  录
来源：http://ag.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://aw.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gt.shxzskj.cn


<!-- 参考信息 -->