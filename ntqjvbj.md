代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ja.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://cv.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nw.szsharing.cn

[T56] Scala：样例类
来源：http://pv.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ds.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://bj.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zx.lnxyls.cn

[T58] Scala：函数定义
来源：http://ul.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ds.szsharing.cn

[T59] Scala：循环
来源：http://xs.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://zv.jctech888.com.cn

[T60] Scala：折叠
来源：http://kn.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nn.huixiangedu.cn

================================================================================
来源：http://uc.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xp.lnxyls.cn

================================================================================
来源：http://gh.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://qe.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wr.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://bt.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pf.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://bp.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eu.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://fh.asd995.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bn.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://hc.nicolike.cn

list(dict.fromkeys(arr))
来源：http://dj.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://bi.panjiajie.cn

{**a, **b}
来源：http://ll.szsharing.cn

[U07] Py：反转字典键值
来源：http://pe.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://lw.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://kd.lnxyls.cn

[y for x in nested for y in x]
来源：http://gx.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://oy.jianghongdianzi.cn

max(d, key=d.get)
来源：http://iq.shxzskj.cn

[U10] Py：按值排序字典
来源：http://sr.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xs.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://md.asd995.cn

(x * 2 for x in arr)
来源：http://cl.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dk.szxytkj.cn

Counter(arr).most_common(3)
来源：http://lf.hnjuh.cn

[U13] Py：固定长度队列
来源：http://or.asd995.cn

deque(maxlen=10)
来源：http://he.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ni.shxzukj.cn

defaultdict(list)
来源：http://xr.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://ss.shxzskj.cn

t = time.perf_counter()
来源：http://ea.9csxet.cn

[U16] Py：命令行参数解析
来源：http://qf.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ze.szsharing.cn

[U17] Py：初始化日志
来源：http://yj.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://df.huixiangedu.cn

[U18] Py：预编译正则
来源：http://qh.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://sp.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://sc.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://df.nicolike.cn

[U20] Py：缓存函数结果
来源：http://no.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://hj.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://kj.colortex.cn

@contextlib.contextmanager
来源：http://wc.huanxung.cn

[U22] Py：矩阵转置
来源：http://it.huanxung.cn

list(zip(*m))
来源：http://dx.9csxet.cn

[U23] Py：分块读取大文件
来源：http://km.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ol.muxihuayi.cn

[U24] Py：路径操作
来源：http://na.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qy.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://lg.yuexingan06.cn

csv.DictReader(f)
来源：http://je.szxytkj.cn

[U26] Py：并发下载
来源：http://vp.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ll.nicolike.cn

[U27] Py：异步 HTTP
来源：http://fq.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://bp.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://ll.huanxung.cn

UserId = int
来源：http://oo.9csxet.cn

[U29] Py：属性校验
来源：http://lz.shxzukj.cn

@property 与 @x.setter 配合
来源：http://io.bjjhwx.cn

[U30] Py：数据类
来源：http://hx.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ph.haigaiapp.cn

[U31] Py：单测
来源：http://uf.newstarts.cn

python -m pytest -q
来源：http://bl.wgjwhj.cn

[U32] Py：代码格式化
来源：http://ar.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ul.gzmigu.cn

[U33] Py：打包发布
来源：http://sw.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://eq.nicolike.cn

[U34] Py：判断编码
来源：http://vy.bookmarksfly.cn

chardet.detect(raw)
来源：http://ka.lnxyls.cn

[U35] Py：发送邮件
来源：http://mt.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ao.jctech888.com.cn

[U36] Py：定时任务
来源：http://vg.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://hq.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ka.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ru.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://uj.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://pk.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://vk.chemitech.net.cn

sys.stdout.isatty()
来源：http://mv.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://qs.9csxet.cn

print("err", file=sys.stderr)
来源：http://gc.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://rp.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hd.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://id.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ws.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://fi.jianghongdianzi.cn

namespace App\Http;
来源：http://eb.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://rw.hnjuh.cn

declare(strict_types=1);
来源：http://oh.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://yg.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://hw.szxytkj.cn

?string $name = null
来源：http://lx.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://nl.shtwfgs.cn

int|string $id
来源：http://et.nicolike.cn

[U48] PHP：纯枚举
来源：http://od.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ic.521024.cn

[U49] PHP：只读属性
来源：http://bo.haigaiapp.cn

public readonly string $name
来源：http://cy.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://ym.panjiajie.cn

public function __construct(private int $id) {}
来源：http://gi.panjiajie.cn

[U51] PHP：数组解构
来源：http://wl.lnxyls.cn

[$a, $b] = $arr;
来源：http://sh.szsharing.cn

[U52] PHP：箭头函数
来源：http://yx.asd995.cn

$double = fn($x) => $x * 2;
来源：http://gc.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://al.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://xp.panjiajie.cn

[U54] PHP：空安全调用
来源：http://fb.hahajie.cn

$obj?->method()
来源：http://eq.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://cp.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tm.colortex.cn

[U56] PHP：命名参数
来源：http://zz.nicolike.cn

f(a: 1, b: 2)
来源：http://mg.huanxung.cn

[U57] PHP：字符串插值
来源：http://qy.shxzskj.cn

"值: {$a}"
来源：http://fx.szsharing.cn

[U58] PHP：数组三件套
来源：http://ei.521024.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fr.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://mw.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nh.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://fd.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gt.jianghongdianzi.cn

[U61] PHP：正则
来源：http://xs.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gh.szsharing.cn

[U62] PHP：日期对象
来源：http://re.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gc.muxihuayi.cn

[U63] PHP：文件读写
来源：http://rw.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://im.hnjuh.cn

[U64] PHP：目录遍历
来源：http://bt.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ti.wgjwhj.cn

[U65] PHP：会话
来源：http://pi.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://io.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://jf.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ju.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://wo.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://az.muxihuayi.cn

[U68] PHP：PDO 连接
来源：http://ia.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gt.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://sy.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mv.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://uy.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xh.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://fz.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://xe.hahajie.cn

[U72] PHP：写错误日志
来源：http://nk.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://qs.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://xv.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://qw.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://yc.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://se.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://rf.jctech888.com.cn

composer require psr/container
来源：http://rm.nicolike.cn

[U76] PHP：简单路由
来源：http://vz.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lj.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ve.jctech888.com.cn

composer require twig/twig
来源：http://zq.panjiajie.cn

[U78] PHP：单元测试
来源：http://wc.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://ga.wgjwhj.cn

[U79] PHP：静态分析
来源：http://yv.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://ms.colortex.cn

[U80] PHP：代码规范修复
来源：http://zf.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uy.9csxet.cn

[U81] JS：初始化项目
来源：http://og.muxihuayi.cn

npm init -y;  npm i express
来源：http://xq.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://ua.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ps.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://yb.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dn.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://qe.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fe.nszjky.cn

[U85] JS：可选链
来源：http://vr.shtwfgs.cn

a?.b?.c
来源：http://kq.muxihuayi.cn

[U86] JS：空值合并
来源：http://yi.jianghongdianzi.cn

a ?? b
来源：http://ne.huixiangedu.cn

[U87] JS：解构默认值
来源：http://cf.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://wd.asd995.cn

[U88] JS：对象展开合并
来源：http://as.shtwfgs.cn

{ ...a, ...b }
来源：http://iq.szxytkj.cn

[U89] JS：数组去重
来源：http://ve.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ot.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://nf.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://rd.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://sb.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mz.chemitech.net.cn

[U92] JS：深拷贝
来源：http://ag.bjjhwx.cn

structuredClone(obj)
来源：http://xy.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://mv.hahajie.cn

`共 ${n} 条`
来源：http://lg.newstarts.cn

[U94] JS：箭头函数
来源：http://yr.shtwfgs.cn

const double = x => x * 2;
来源：http://lm.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://qt.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://mk.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://yx.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gi.wgjwhj.cn

[U97] JS：并发请求
来源：http://xy.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ue.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://ao.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ov.hnjuh.cn

[U99] JS：事件监听
来源：http://yj.colortex.cn

el.addEventListener("click", e => {})
来源：http://wl.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://mp.nszjky.cn

document.querySelector(".item")
来源：http://my.haigaiapp.cn

[U101] JS：classList 操作
来源：http://bk.521024.cn

el.classList.toggle("active")
来源：http://ac.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://nq.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yr.szxytkj.cn

[U103] JS：定时器
来源：http://dc.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uv.huixiangedu.cn

[U104] JS：防抖
来源：http://xo.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ph.gzmigu.cn

[U105] JS：节流
来源：http://xi.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xz.nszjky.cn

[U106] JS：日期格式化
来源：http://hm.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dc.szxytkj.cn

[U107] JS：数字千分位
来源：http://is.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xp.szxytkj.cn

[U108] JS：随机整数
来源：http://rx.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qw.colortex.cn

[U109] JS：数组分组
来源：http://it.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://cj.nicolike.cn

[U110] JS：数组分块
来源：http://qm.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qk.hahajie.cn

[U111] JS：对象转 Map
来源：http://zt.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://zt.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ym.bjjhwx.cn

"7".padStart(3, "0")
来源：http://gi.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://wl.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://pz.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://mm.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lp.521024.cn

[U115] JS：生成 UUID
来源：http://ob.lnxyls.cn

crypto.randomUUID()
来源：http://kr.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://ji.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://wk.hahajie.cn

[U117] JS：单元测试
来源：http://id.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://bj.szxytkj.cn

[U118] JS：开发服务器
来源：http://gx.lnxyls.cn

npm i -D vite;  npx vite
来源：http://js.haigaiapp.cn

[U119] JS：生产构建
来源：http://lk.chemitech.net.cn

npx vite build
来源：http://ox.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ls.asd995.cn

import.meta.env.VITE_API_URL
来源：http://yc.hahajie.cn

================================================================================
来源：http://tx.shtwfgs.cn

统计汇总
来源：http://jd.asd995.cn

================================================================================
来源：http://ul.bjjhwx.cn

按语言统计（条）：
来源：http://ry.nicolike.cn

Python ......... 252
来源：http://gt.huixiangedu.cn

PHP ............ 252
来源：http://jx.huixinmuqiang.cn

JavaScript ..... 252
来源：http://fs.colortex.cn

TypeScript ..... 212
来源：http://ie.panjiajie.cn

Java ........... 212
来源：http://vg.nicolike.cn

Go ............. 212
来源：http://dt.colortex.cn

Ruby ........... 212
来源：http://mt.huixinmuqiang.cn

C# ............. 212
来源：http://gr.bookmarksfly.cn

C .............. 30
来源：http://ks.newstarts.cn

C++ ............ 30
来源：http://qq.huixiangedu.cn

SQL ............ 90
来源：http://cx.521024.cn

Bash ........... 80
来源：http://ez.yuexingan06.cn

Kotlin ......... 15
来源：http://mk.huixiangedu.cn

Swift .......... 15
来源：http://nf.jctech888.com.cn

Lua ............ 10
来源：http://sa.szxytkj.cn

Perl ........... 10
来源：http://wf.hnjuh.cn

Scala .......... 10
来源：http://ls.yuexingan06.cn

------------------------------------
来源：http://gz.chemitech.net.cn

合计 ........... 2106 条
来源：http://rv.bjjhwx.cn

按章节统计：
来源：http://mt.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ln.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qw.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yj.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fn.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://id.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sb.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ez.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sm.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zn.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cb.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ys.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fa.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bw.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://js.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ug.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iq.shxzskj.cn

Q SQL 专题                              90
来源：http://wi.521024.cn

R Bash 专题                             80
来源：http://jy.szsharing.cn

S C / C++ 专题                          60
来源：http://vb.newstarts.cn

T 其他语言补充                          60
来源：http://nr.gzmigu.cn


<!-- 参考信息 -->