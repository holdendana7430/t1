代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://zb.lnxyls.cn

[T59] Scala：循环
来源：http://iy.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ah.lnxyls.cn

[T60] Scala：折叠
来源：http://hz.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vu.hnjuh.cn

================================================================================
来源：http://kd.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lu.jianghongdianzi.cn

================================================================================
来源：http://pd.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://xz.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vi.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://bb.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://at.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://om.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bt.huanxung.cn

[U04] Py：变量调试打印
来源：http://uc.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://py.nszjky.cn

[U05] Py：列表去重且保序
来源：http://gt.nszjky.cn

list(dict.fromkeys(arr))
来源：http://ol.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://iv.chemitech.net.cn

{**a, **b}
来源：http://cr.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://ft.newstarts.cn

{v: k for k, v in d.items()}
来源：http://vr.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://bd.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://jn.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://sp.szxytkj.cn

max(d, key=d.get)
来源：http://ah.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://wy.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fr.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://mh.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://sq.huixinmuqiang.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hd.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://wf.gzmigu.cn

[U13] Py：固定长度队列
来源：http://qa.jctech888.com.cn

deque(maxlen=10)
来源：http://qf.nicolike.cn

[U14] Py：分组收集到列表
来源：http://dy.yuntaijiaju.cn

defaultdict(list)
来源：http://eb.huanxung.cn

[U15] Py：高精度计时
来源：http://ng.yuntaijiaju.cn

t = time.perf_counter()
来源：http://ay.hahajie.cn

[U16] Py：命令行参数解析
来源：http://wf.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lv.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://rp.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://dv.nicolike.cn

[U18] Py：预编译正则
来源：http://rf.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://pe.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://ym.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wi.newstarts.cn

[U20] Py：缓存函数结果
来源：http://kh.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://ms.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://rv.shxzukj.cn

@contextlib.contextmanager
来源：http://mx.szsharing.cn

[U22] Py：矩阵转置
来源：http://ki.lnxyls.cn

list(zip(*m))
来源：http://ac.nszjky.cn

[U23] Py：分块读取大文件
来源：http://is.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hk.jctech888.com.cn

[U24] Py：路径操作
来源：http://os.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tm.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://ls.haigaiapp.cn

csv.DictReader(f)
来源：http://zc.huanxung.cn

[U26] Py：并发下载
来源：http://qt.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tn.newstarts.cn

[U27] Py：异步 HTTP
来源：http://xk.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://xx.lnxyls.cn

[U28] Py：类型别名
来源：http://yc.huixiangedu.cn

UserId = int
来源：http://pp.chemitech.net.cn

[U29] Py：属性校验
来源：http://cl.gzmigu.cn

@property 与 @x.setter 配合
来源：http://yc.9csxet.cn

[U30] Py：数据类
来源：http://jr.nicolike.cn

@dataclass(slots=True)
来源：http://xn.panjiajie.cn

[U31] Py：单测
来源：http://ha.9csxet.cn

python -m pytest -q
来源：http://zv.chemitech.net.cn

[U32] Py：代码格式化
来源：http://cl.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://wk.9csxet.cn

[U33] Py：打包发布
来源：http://em.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://lg.szxytkj.cn

[U34] Py：判断编码
来源：http://pz.szsharing.cn

chardet.detect(raw)
来源：http://lo.shxzskj.cn

[U35] Py：发送邮件
来源：http://cz.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://go.bjjhwx.cn

[U36] Py：定时任务
来源：http://io.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://yg.panjiajie.cn

[U37] Py：读写 Excel
来源：http://jf.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fc.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://px.asd995.cn

Path(__file__).resolve().parent
来源：http://kj.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://fv.muxihuayi.cn

sys.stdout.isatty()
来源：http://ba.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://ux.colortex.cn

print("err", file=sys.stderr)
来源：http://gq.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://lj.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yj.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://he.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xn.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://ji.szxytkj.cn

namespace App\Http;
来源：http://yu.9csxet.cn

[U44] PHP：开启严格类型
来源：http://xi.bjjhwx.cn

declare(strict_types=1);
来源：http://gg.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://au.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.huixiangedu.cn

[U46] PHP：可空类型
来源：http://ly.yuntaijiaju.cn

?string $name = null
来源：http://sw.gzmigu.cn

[U47] PHP：联合类型
来源：http://ad.colortex.cn

int|string $id
来源：http://ks.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://cu.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cl.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://ex.haigaiapp.cn

public readonly string $name
来源：http://ag.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://lj.asd995.cn

public function __construct(private int $id) {}
来源：http://aw.jctech888.com.cn

[U51] PHP：数组解构
来源：http://hk.gzmigu.cn

[$a, $b] = $arr;
来源：http://lb.lnxyls.cn

[U52] PHP：箭头函数
来源：http://rr.asd995.cn

$double = fn($x) => $x * 2;
来源：http://xt.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://it.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://fv.nicolike.cn

[U54] PHP：空安全调用
来源：http://bx.muxihuayi.cn

$obj?->method()
来源：http://pd.shxzukj.cn

[U55] PHP：match 表达式
来源：http://tu.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hf.hnjuh.cn

[U56] PHP：命名参数
来源：http://uo.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://gf.szxytkj.cn

[U57] PHP：字符串插值
来源：http://gl.hahajie.cn

"值: {$a}"
来源：http://cb.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://gz.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cc.huanxung.cn

[U59] PHP：自定义排序
来源：http://xi.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hx.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://az.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ui.muxihuayi.cn

[U61] PHP：正则
来源：http://iq.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ps.muxihuayi.cn

[U62] PHP：日期对象
来源：http://xz.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gn.gzmigu.cn

[U63] PHP：文件读写
来源：http://po.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pe.nszjky.cn

[U64] PHP：目录遍历
来源：http://gs.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://jn.shtwfgs.cn

[U65] PHP：会话
来源：http://oe.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ju.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://zo.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hb.szsharing.cn

[U67] PHP：处理文件上传
来源：http://gc.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jz.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://tx.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eu.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://pk.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ld.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://jb.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mz.huanxung.cn

[U71] PHP：抛出异常
来源：http://ny.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://xg.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://fx.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://nd.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://xu.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://kv.szsharing.cn

[U74] PHP：读取环境变量
来源：http://la.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://vz.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://wp.jctech888.com.cn

composer require psr/container
来源：http://ke.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://ow.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ie.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://nm.9csxet.cn

composer require twig/twig
来源：http://yu.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://kd.asd995.cn

composer require --dev phpunit/phpunit
来源：http://hc.yuexingan06.cn

[U79] PHP：静态分析
来源：http://ju.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://nc.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://xd.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sp.521024.cn

[U81] JS：初始化项目
来源：http://tt.szsharing.cn

npm init -y;  npm i express
来源：http://tz.huanxung.cn

[U82] JS：package.json 脚本
来源：http://sm.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xn.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ln.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eq.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://cz.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zk.szsharing.cn

[U85] JS：可选链
来源：http://ny.jctech888.com.cn

a?.b?.c
来源：http://ks.hnjuh.cn

[U86] JS：空值合并
来源：http://sn.szsharing.cn

a ?? b
来源：http://xp.haigaiapp.cn

[U87] JS：解构默认值
来源：http://kt.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://fs.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://ac.gzmigu.cn

{ ...a, ...b }
来源：http://qt.nicolike.cn

[U89] JS：数组去重
来源：http://nl.chemitech.net.cn

[...new Set(arr)]
来源：http://nj.shxzukj.cn

[U90] JS：数字数组排序
来源：http://cq.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://vz.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://rq.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kz.chemitech.net.cn

[U92] JS：深拷贝
来源：http://jl.newstarts.cn

structuredClone(obj)
来源：http://ye.521024.cn

[U93] JS：模板字符串
来源：http://sa.nszjky.cn

`共 ${n} 条`
来源：http://vc.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ob.asd995.cn

const double = x => x * 2;
来源：http://tv.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://tc.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://kq.newstarts.cn

[U96] JS：async/await 与异常
来源：http://za.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ze.jctech888.com.cn

[U97] JS：并发请求
来源：http://aw.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ze.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://fw.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oo.chemitech.net.cn

[U99] JS：事件监听
来源：http://gm.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://fu.newstarts.cn

[U100] JS：DOM 查询
来源：http://wd.huixiangedu.cn

document.querySelector(".item")
来源：http://lj.szsharing.cn

[U101] JS：classList 操作
来源：http://gk.jctech888.com.cn

el.classList.toggle("active")
来源：http://tw.bjjhwx.cn

[U102] JS：本地存储
来源：http://vk.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ic.9csxet.cn

[U103] JS：定时器
来源：http://bf.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fp.shxzukj.cn

[U104] JS：防抖
来源：http://gl.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zh.lnxyls.cn

[U105] JS：节流
来源：http://se.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://he.gzmigu.cn

[U106] JS：日期格式化
来源：http://jr.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://we.shxzukj.cn

[U107] JS：数字千分位
来源：http://yc.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lo.shxzskj.cn

[U108] JS：随机整数
来源：http://ol.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://az.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://tl.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://wc.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://hn.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jk.shxzskj.cn

[U111] JS：对象转 Map
来源：http://mt.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://qh.lnxyls.cn

[U112] JS：字符串补位
来源：http://ov.yuexingan06.cn

"7".padStart(3, "0")
来源：http://gl.lnxyls.cn

[U113] JS：正则替换全部
来源：http://wr.nszjky.cn

s.replaceAll("a", "b")
来源：http://jj.newstarts.cn

[U114] JS：JSON 深比较
来源：http://gm.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mn.szxytkj.cn

[U115] JS：生成 UUID
来源：http://uu.nszjky.cn

crypto.randomUUID()
来源：http://sg.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://fa.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://pb.wgjwhj.cn

[U117] JS：单元测试
来源：http://ou.521024.cn

npm i -D vitest;  npx vitest
来源：http://hu.chemitech.net.cn

[U118] JS：开发服务器
来源：http://ci.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://vv.bjjhwx.cn

[U119] JS：生产构建
来源：http://tm.bookmarksfly.cn

npx vite build
来源：http://kn.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://xe.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://xz.nszjky.cn

================================================================================
来源：http://qs.hnjuh.cn

统计汇总
来源：http://jy.shtwfgs.cn

================================================================================
来源：http://kl.colortex.cn

按语言统计（条）：
来源：http://pr.jianghongdianzi.cn

Python ......... 252
来源：http://jf.szsharing.cn

PHP ............ 252
来源：http://bl.newstarts.cn

JavaScript ..... 252
来源：http://vs.nicolike.cn

TypeScript ..... 212
来源：http://di.yuexingan06.cn

Java ........... 212
来源：http://vj.bjjhwx.cn

Go ............. 212
来源：http://wv.lnxyls.cn

Ruby ........... 212
来源：http://rs.hnjuh.cn

C# ............. 212
来源：http://oe.wgjwhj.cn

C .............. 30
来源：http://hs.newstarts.cn

C++ ............ 30
来源：http://ku.hahajie.cn

SQL ............ 90
来源：http://gp.bookmarksfly.cn

Bash ........... 80
来源：http://ss.szsharing.cn

Kotlin ......... 15
来源：http://om.muxihuayi.cn

Swift .......... 15
来源：http://ad.jianghongdianzi.cn

Lua ............ 10
来源：http://pp.haigaiapp.cn

Perl ........... 10
来源：http://kh.nszjky.cn

Scala .......... 10
来源：http://rc.muxihuayi.cn

------------------------------------
来源：http://ci.lnxyls.cn

合计 ........... 2106 条
来源：http://xg.haigaiapp.cn

按章节统计：
来源：http://gr.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kq.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sy.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tv.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://if.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xg.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ps.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rb.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ff.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://of.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lz.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://on.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hh.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wi.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gz.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pe.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kz.lnxyls.cn

Q SQL 专题                              90
来源：http://aw.haigaiapp.cn

R Bash 专题                             80
来源：http://ae.hnjuh.cn

S C / C++ 专题                          60
来源：http://zm.jctech888.com.cn

T 其他语言补充                          60
来源：http://ze.chemitech.net.cn

U 高频实用片段                         120
来源：http://yt.jctech888.com.cn

------------------------------------
来源：http://sg.yuntaijiaju.cn

合计                                  2106 条
来源：http://zd.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://vi.szsharing.cn

使用提醒
来源：http://fw.hahajie.cn

--------------------------------------------------------------------------------
来源：http://qh.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mt.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ks.gzmigu.cn


<!-- 参考信息 -->