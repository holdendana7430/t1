代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://rv.shxzukj.cn

[T55] Scala：集合过滤
来源：http://xn.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dc.wgjwhj.cn

[T56] Scala：样例类
来源：http://qo.lnxyls.cn

case class User(name: String, age: Int)
来源：http://nm.nszjky.cn

[T57] Scala：模式匹配
来源：http://iv.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ny.huanxung.cn

[T58] Scala：函数定义
来源：http://oi.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zy.jianghongdianzi.cn

[T59] Scala：循环
来源：http://om.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://ou.shtwfgs.cn

[T60] Scala：折叠
来源：http://uh.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gg.jianghongdianzi.cn

================================================================================
来源：http://fy.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zg.szsharing.cn

================================================================================
来源：http://zr.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://xn.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qe.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://eu.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bs.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://hj.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pp.9csxet.cn

[U04] Py：变量调试打印
来源：http://hn.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dj.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://nt.asd995.cn

list(dict.fromkeys(arr))
来源：http://vk.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://sq.asd995.cn

{**a, **b}
来源：http://xy.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://rw.colortex.cn

{v: k for k, v in d.items()}
来源：http://vs.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://gm.yuexingan06.cn

[y for x in nested for y in x]
来源：http://pz.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://yy.9csxet.cn

max(d, key=d.get)
来源：http://pq.colortex.cn

[U10] Py：按值排序字典
来源：http://vz.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pd.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://cd.colortex.cn

(x * 2 for x in arr)
来源：http://le.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://np.szsharing.cn

Counter(arr).most_common(3)
来源：http://ut.szsharing.cn

[U13] Py：固定长度队列
来源：http://kx.newstarts.cn

deque(maxlen=10)
来源：http://eu.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://ae.huanxung.cn

defaultdict(list)
来源：http://lr.yuexingan06.cn

[U15] Py：高精度计时
来源：http://ox.bjjhwx.cn

t = time.perf_counter()
来源：http://ig.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://rg.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dj.nicolike.cn

[U17] Py：初始化日志
来源：http://ft.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://kk.asd995.cn

[U18] Py：预编译正则
来源：http://un.colortex.cn

pat = re.compile(r"\d+")
来源：http://ro.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://sd.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nc.colortex.cn

[U20] Py：缓存函数结果
来源：http://ng.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://jm.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://ra.szxytkj.cn

@contextlib.contextmanager
来源：http://yp.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://my.colortex.cn

list(zip(*m))
来源：http://um.szsharing.cn

[U23] Py：分块读取大文件
来源：http://pn.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tt.9csxet.cn

[U24] Py：路径操作
来源：http://yk.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qh.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://to.shtwfgs.cn

csv.DictReader(f)
来源：http://ru.lnxyls.cn

[U26] Py：并发下载
来源：http://bc.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://an.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://gl.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://cq.shxzukj.cn

[U28] Py：类型别名
来源：http://eu.shxzskj.cn

UserId = int
来源：http://yh.colortex.cn

[U29] Py：属性校验
来源：http://dw.panjiajie.cn

@property 与 @x.setter 配合
来源：http://zl.shxzskj.cn

[U30] Py：数据类
来源：http://in.nszjky.cn

@dataclass(slots=True)
来源：http://xc.huixinmuqiang.cn

[U31] Py：单测
来源：http://wn.haigaiapp.cn

python -m pytest -q
来源：http://nj.hnjuh.cn

[U32] Py：代码格式化
来源：http://wu.nicolike.cn

ruff format . && ruff check --fix .
来源：http://yn.asd995.cn

[U33] Py：打包发布
来源：http://bq.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://br.lnxyls.cn

[U34] Py：判断编码
来源：http://ty.asd995.cn

chardet.detect(raw)
来源：http://yc.lnxyls.cn

[U35] Py：发送邮件
来源：http://ds.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zb.haigaiapp.cn

[U36] Py：定时任务
来源：http://da.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://ee.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ox.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iw.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ba.nicolike.cn

Path(__file__).resolve().parent
来源：http://oy.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://hk.521024.cn

sys.stdout.isatty()
来源：http://hj.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://le.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://zg.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://kl.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kz.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://lb.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://px.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://nx.gzmigu.cn

namespace App\Http;
来源：http://cv.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://jl.muxihuayi.cn

declare(strict_types=1);
来源：http://zf.bookmarksfly.cn

[U45] PHP：类型声明与返回类型
来源：http://ug.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cy.gzmigu.cn

[U46] PHP：可空类型
来源：http://ft.asd995.cn

?string $name = null
来源：http://hk.szxytkj.cn

[U47] PHP：联合类型
来源：http://jh.bjjhwx.cn

int|string $id
来源：http://es.szxytkj.cn

[U48] PHP：纯枚举
来源：http://bv.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yh.haigaiapp.cn

[U49] PHP：只读属性
来源：http://mh.newstarts.cn

public readonly string $name
来源：http://po.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://vs.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://xv.shxzukj.cn

[U51] PHP：数组解构
来源：http://nx.nicolike.cn

[$a, $b] = $arr;
来源：http://hw.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://qc.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://fw.szsharing.cn

[U53] PHP：空合并运算符
来源：http://fs.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://wb.colortex.cn

[U54] PHP：空安全调用
来源：http://dw.nicolike.cn

$obj?->method()
来源：http://rq.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ar.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ld.lnxyls.cn

[U56] PHP：命名参数
来源：http://nk.9csxet.cn

f(a: 1, b: 2)
来源：http://wu.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://ud.panjiajie.cn

"值: {$a}"
来源：http://qq.shxzukj.cn

[U58] PHP：数组三件套
来源：http://ci.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wy.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://lz.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dx.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://er.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bj.jianghongdianzi.cn

[U61] PHP：正则
来源：http://ra.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://to.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://lx.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xh.asd995.cn

[U63] PHP：文件读写
来源：http://gc.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ua.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://zg.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ck.shxzukj.cn

[U65] PHP：会话
来源：http://mh.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://si.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://pe.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ur.hahajie.cn

[U67] PHP：处理文件上传
来源：http://ye.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ib.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://wb.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ve.521024.cn

[U69] PHP：PDO 预处理
来源：http://qw.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nb.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ih.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qz.shxzukj.cn

[U71] PHP：抛出异常
来源：http://qr.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://ys.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://ao.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://aj.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://fx.521024.cn

parse_ini_file("config.ini", true)
来源：http://dy.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://te.colortex.cn

getenv("APP_ENV") ?: "production"
来源：http://wj.szsharing.cn

[U75] PHP：依赖注入
来源：http://fp.huixiangedu.cn

composer require psr/container
来源：http://jc.huanxung.cn

[U76] PHP：简单路由
来源：http://vs.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kv.hnjuh.cn

[U77] PHP：模板渲染
来源：http://fm.jctech888.com.cn

composer require twig/twig
来源：http://ca.hnjuh.cn

[U78] PHP：单元测试
来源：http://ml.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://hd.muxihuayi.cn

[U79] PHP：静态分析
来源：http://pf.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://oe.asd995.cn

[U80] PHP：代码规范修复
来源：http://gj.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pk.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://mf.newstarts.cn

npm init -y;  npm i express
来源：http://un.yuntaijiaju.cn

[U82] JS：package.json 脚本
来源：http://if.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ph.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://ng.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ds.9csxet.cn

[U84] JS：CommonJS 写法
来源：http://lk.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ai.colortex.cn

[U85] JS：可选链
来源：http://fk.asd995.cn

a?.b?.c
来源：http://iq.newstarts.cn

[U86] JS：空值合并
来源：http://pq.521024.cn

a ?? b
来源：http://dj.chemitech.net.cn

[U87] JS：解构默认值
来源：http://dm.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://tw.szxytkj.cn

[U88] JS：对象展开合并
来源：http://mj.gzmigu.cn

{ ...a, ...b }
来源：http://rx.yuexingan06.cn

[U89] JS：数组去重
来源：http://ej.bjjhwx.cn

[...new Set(arr)]
来源：http://wl.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ux.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://wb.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://hc.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zg.huanxung.cn

[U92] JS：深拷贝
来源：http://wg.hnjuh.cn

structuredClone(obj)
来源：http://bx.yuexingan06.cn

[U93] JS：模板字符串
来源：http://yv.asd995.cn

`共 ${n} 条`
来源：http://yc.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://gs.bjjhwx.cn

const double = x => x * 2;
来源：http://xt.asd995.cn

[U95] JS：Promise 包装
来源：http://iw.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://ix.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://gk.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iq.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://pr.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tx.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://ax.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dz.bjjhwx.cn

[U99] JS：事件监听
来源：http://dq.newstarts.cn

el.addEventListener("click", e => {})
来源：http://pg.521024.cn

[U100] JS：DOM 查询
来源：http://cc.nszjky.cn

document.querySelector(".item")
来源：http://ch.haigaiapp.cn

[U101] JS：classList 操作
来源：http://ld.szsharing.cn

el.classList.toggle("active")
来源：http://wl.jianghongdianzi.cn

[U102] JS：本地存储
来源：http://hl.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://js.gzmigu.cn

[U103] JS：定时器
来源：http://fo.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pg.colortex.cn

[U104] JS：防抖
来源：http://xr.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.shtwfgs.cn

[U105] JS：节流
来源：http://se.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iy.gzmigu.cn

[U106] JS：日期格式化
来源：http://gi.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ct.colortex.cn

[U107] JS：数字千分位
来源：http://hd.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xq.nszjky.cn

[U108] JS：随机整数
来源：http://qv.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aw.szsharing.cn

[U109] JS：数组分组
来源：http://fs.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://ns.bjjhwx.cn

[U110] JS：数组分块
来源：http://kw.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jc.asd995.cn

[U111] JS：对象转 Map
来源：http://ep.asd995.cn

new Map(Object.entries(obj))
来源：http://rc.colortex.cn

[U112] JS：字符串补位
来源：http://zx.shxzskj.cn

"7".padStart(3, "0")
来源：http://ea.szsharing.cn

[U113] JS：正则替换全部
来源：http://kw.colortex.cn

s.replaceAll("a", "b")
来源：http://op.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://jr.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://py.newstarts.cn

[U115] JS：生成 UUID
来源：http://eq.yuntaijiaju.cn

crypto.randomUUID()
来源：http://na.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://lf.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://ia.jctech888.com.cn

[U117] JS：单元测试
来源：http://lh.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://df.nicolike.cn

[U118] JS：开发服务器
来源：http://dz.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://bl.hnjuh.cn

[U119] JS：生产构建
来源：http://mh.szsharing.cn

npx vite build
来源：http://yn.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://sl.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://mm.newstarts.cn

================================================================================
来源：http://dg.wgjwhj.cn

统计汇总
来源：http://pr.asd995.cn

================================================================================
来源：http://cm.jianghongdianzi.cn

按语言统计（条）：
来源：http://dg.huixinmuqiang.cn

Python ......... 252
来源：http://wm.wgjwhj.cn

PHP ............ 252
来源：http://sj.yuntaijiaju.cn

JavaScript ..... 252
来源：http://bz.yuexingan06.cn

TypeScript ..... 212
来源：http://jt.muxihuayi.cn

Java ........... 212
来源：http://dt.hnjuh.cn

Go ............. 212
来源：http://sd.haigaiapp.cn

Ruby ........... 212
来源：http://mq.muxihuayi.cn

C# ............. 212
来源：http://dm.szxytkj.cn

C .............. 30
来源：http://gm.huixinmuqiang.cn

C++ ............ 30
来源：http://ei.shtwfgs.cn

SQL ............ 90
来源：http://lk.nszjky.cn

Bash ........... 80
来源：http://gd.521024.cn

Kotlin ......... 15
来源：http://uk.szxytkj.cn

Swift .......... 15
来源：http://kp.521024.cn

Lua ............ 10
来源：http://ih.asd995.cn

Perl ........... 10
来源：http://bu.asd995.cn

Scala .......... 10
来源：http://oq.haigaiapp.cn

------------------------------------
来源：http://qe.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://xj.chemitech.net.cn

按章节统计：
来源：http://rp.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jd.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mw.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ss.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ls.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qc.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qo.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qm.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zq.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yt.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sa.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pn.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vf.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rs.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bm.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qy.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ze.haigaiapp.cn

Q SQL 专题                              90
来源：http://lx.huixinmuqiang.cn

R Bash 专题                             80
来源：http://vd.panjiajie.cn

S C / C++ 专题                          60
来源：http://di.yuexingan06.cn

T 其他语言补充                          60
来源：http://hw.newstarts.cn


<!-- 参考信息 -->