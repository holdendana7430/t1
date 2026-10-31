代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://di.nszjky.cn

[T51] Scala：Hello World
来源：http://rj.bjjhwx.cn

println("Hello")
来源：http://im.9csxet.cn

[T52] Scala：变量
来源：http://ur.shxzukj.cn

val a = 1;  var b = 2
来源：http://kx.panjiajie.cn

[T53] Scala：字符串插值
来源：http://ev.hahajie.cn

s"值: $b"
来源：http://ak.asd995.cn

[T54] Scala：集合映射
来源：http://au.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://xc.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://id.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lr.bjjhwx.cn

[T56] Scala：样例类
来源：http://rf.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://ex.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://yv.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uc.nszjky.cn

[T58] Scala：函数定义
来源：http://ec.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pn.huixiangedu.cn

[T59] Scala：循环
来源：http://op.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ch.asd995.cn

[T60] Scala：折叠
来源：http://qs.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xz.huixiangedu.cn

================================================================================
来源：http://ag.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mi.haigaiapp.cn

================================================================================
来源：http://ig.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://mx.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yo.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://pd.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hg.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://az.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nn.panjiajie.cn

[U04] Py：变量调试打印
来源：http://zu.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iy.huanxung.cn

[U05] Py：列表去重且保序
来源：http://ap.521024.cn

list(dict.fromkeys(arr))
来源：http://uw.nicolike.cn

[U06] Py：合并两个字典
来源：http://ee.wgjwhj.cn

{**a, **b}
来源：http://wi.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://to.asd995.cn

{v: k for k, v in d.items()}
来源：http://ow.shxzskj.cn

[U08] Py：展平二维列表
来源：http://wc.hnjuh.cn

[y for x in nested for y in x]
来源：http://uh.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://fm.yuntaijiaju.cn

max(d, key=d.get)
来源：http://us.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://to.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bx.nicolike.cn

[U11] Py：生成器表达式
来源：http://ss.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://fw.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cg.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://qq.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://hd.nszjky.cn

deque(maxlen=10)
来源：http://fq.521024.cn

[U14] Py：分组收集到列表
来源：http://pl.chemitech.net.cn

defaultdict(list)
来源：http://aw.521024.cn

[U15] Py：高精度计时
来源：http://ck.szxytkj.cn

t = time.perf_counter()
来源：http://kt.hahajie.cn

[U16] Py：命令行参数解析
来源：http://du.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://as.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://ma.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://bk.shtwfgs.cn

[U18] Py：预编译正则
来源：http://tl.newstarts.cn

pat = re.compile(r"\d+")
来源：http://ax.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://gz.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kn.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://no.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://no.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://ub.yuexingan06.cn

@contextlib.contextmanager
来源：http://bg.9csxet.cn

[U22] Py：矩阵转置
来源：http://uf.wgjwhj.cn

list(zip(*m))
来源：http://dc.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://zf.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wx.huixiangedu.cn

[U24] Py：路径操作
来源：http://eo.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ia.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://nd.shxzukj.cn

csv.DictReader(f)
来源：http://kn.huanxung.cn

[U26] Py：并发下载
来源：http://je.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cc.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://zl.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://hr.hahajie.cn

[U28] Py：类型别名
来源：http://gx.shtwfgs.cn

UserId = int
来源：http://wo.hahajie.cn

[U29] Py：属性校验
来源：http://gk.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://yp.lnxyls.cn

[U30] Py：数据类
来源：http://vw.shxzskj.cn

@dataclass(slots=True)
来源：http://xs.szxytkj.cn

[U31] Py：单测
来源：http://nh.szsharing.cn

python -m pytest -q
来源：http://ty.hnjuh.cn

[U32] Py：代码格式化
来源：http://as.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://dn.lnxyls.cn

[U33] Py：打包发布
来源：http://eh.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://qn.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://ph.muxihuayi.cn

chardet.detect(raw)
来源：http://gp.9csxet.cn

[U35] Py：发送邮件
来源：http://nw.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bf.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://dl.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://oy.nicolike.cn

[U37] Py：读写 Excel
来源：http://mp.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yd.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://bc.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://pj.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://dl.shtwfgs.cn

sys.stdout.isatty()
来源：http://uw.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://rn.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://wo.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://wp.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ye.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://aq.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cg.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://vy.huixiangedu.cn

namespace App\Http;
来源：http://cw.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://za.muxihuayi.cn

declare(strict_types=1);
来源：http://mh.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://si.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.shxzukj.cn

[U46] PHP：可空类型
来源：http://hi.shxzskj.cn

?string $name = null
来源：http://lr.newstarts.cn

[U47] PHP：联合类型
来源：http://fz.szxytkj.cn

int|string $id
来源：http://nr.hahajie.cn

[U48] PHP：纯枚举
来源：http://hi.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kz.wgjwhj.cn

[U49] PHP：只读属性
来源：http://lp.nszjky.cn

public readonly string $name
来源：http://sa.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://ei.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://sx.wgjwhj.cn

[U51] PHP：数组解构
来源：http://ev.jctech888.com.cn

[$a, $b] = $arr;
来源：http://jn.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://ca.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://wv.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://dn.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://gd.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://hz.muxihuayi.cn

$obj?->method()
来源：http://tr.nicolike.cn

[U55] PHP：match 表达式
来源：http://og.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jq.hahajie.cn

[U56] PHP：命名参数
来源：http://ic.huixiangedu.cn

f(a: 1, b: 2)
来源：http://am.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://tg.hahajie.cn

"值: {$a}"
来源：http://bb.szxytkj.cn

[U58] PHP：数组三件套
来源：http://pg.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://td.szxytkj.cn

[U59] PHP：自定义排序
来源：http://ys.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jg.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://sm.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tj.newstarts.cn

[U61] PHP：正则
来源：http://gz.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ti.huixinmuqiang.cn

[U62] PHP：日期对象
来源：http://oo.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://td.9csxet.cn

[U63] PHP：文件读写
来源：http://sg.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fs.521024.cn

[U64] PHP：目录遍历
来源：http://sp.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://nt.jctech888.com.cn

[U65] PHP：会话
来源：http://sf.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rz.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://jc.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ba.huanxung.cn

[U67] PHP：处理文件上传
来源：http://mt.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pm.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://fk.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nu.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://vq.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aj.szsharing.cn

[U70] PHP：PDO 事务
来源：http://jn.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ud.shxzskj.cn

[U71] PHP：抛出异常
来源：http://qn.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://is.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://hv.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://zx.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://ym.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://ga.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://vc.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://by.nszjky.cn

[U75] PHP：依赖注入
来源：http://ez.colortex.cn

composer require psr/container
来源：http://dx.shtwfgs.cn

[U76] PHP：简单路由
来源：http://ci.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uv.colortex.cn

[U77] PHP：模板渲染
来源：http://qc.panjiajie.cn

composer require twig/twig
来源：http://uq.shxzukj.cn

[U78] PHP：单元测试
来源：http://cc.colortex.cn

composer require --dev phpunit/phpunit
来源：http://rf.9csxet.cn

[U79] PHP：静态分析
来源：http://xm.yuntaijiaju.cn

composer require --dev phpstan/phpstan
来源：http://xc.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://bl.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nv.colortex.cn

[U81] JS：初始化项目
来源：http://un.bjjhwx.cn

npm init -y;  npm i express
来源：http://le.colortex.cn

[U82] JS：package.json 脚本
来源：http://fa.hahajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://in.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://gh.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ws.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://iy.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uu.chemitech.net.cn

[U85] JS：可选链
来源：http://vv.nicolike.cn

a?.b?.c
来源：http://xt.shxzskj.cn

[U86] JS：空值合并
来源：http://bp.newstarts.cn

a ?? b
来源：http://nv.shxzukj.cn

[U87] JS：解构默认值
来源：http://ib.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://xc.huanxung.cn

[U88] JS：对象展开合并
来源：http://gy.bookmarksfly.cn

{ ...a, ...b }
来源：http://tu.shxzskj.cn

[U89] JS：数组去重
来源：http://sb.bookmarksfly.cn

[...new Set(arr)]
来源：http://ox.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://cq.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://li.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wi.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ac.yuexingan06.cn

[U92] JS：深拷贝
来源：http://tu.hnjuh.cn

structuredClone(obj)
来源：http://ku.huanxung.cn

[U93] JS：模板字符串
来源：http://ia.gzmigu.cn

`共 ${n} 条`
来源：http://bh.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://wi.bjjhwx.cn

const double = x => x * 2;
来源：http://yk.huanxung.cn

[U95] JS：Promise 包装
来源：http://qm.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://tm.nszjky.cn

[U96] JS：async/await 与异常
来源：http://cr.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ag.asd995.cn

[U97] JS：并发请求
来源：http://ay.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://dg.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cu.jctech888.com.cn

[U99] JS：事件监听
来源：http://cr.newstarts.cn

el.addEventListener("click", e => {})
来源：http://se.newstarts.cn

[U100] JS：DOM 查询
来源：http://yb.colortex.cn

document.querySelector(".item")
来源：http://tc.chemitech.net.cn

[U101] JS：classList 操作
来源：http://qt.hnjuh.cn

el.classList.toggle("active")
来源：http://wt.521024.cn

[U102] JS：本地存储
来源：http://kl.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://es.asd995.cn

[U103] JS：定时器
来源：http://ec.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://be.asd995.cn

[U104] JS：防抖
来源：http://sw.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cn.nicolike.cn

[U105] JS：节流
来源：http://sd.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://as.nszjky.cn

[U106] JS：日期格式化
来源：http://ng.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pk.haigaiapp.cn

[U107] JS：数字千分位
来源：http://pz.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cr.colortex.cn

[U108] JS：随机整数
来源：http://gn.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hm.lnxyls.cn

[U109] JS：数组分组
来源：http://dj.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://gu.bookmarksfly.cn

[U110] JS：数组分块
来源：http://hu.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ae.huanxung.cn

[U111] JS：对象转 Map
来源：http://fs.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://hr.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://sf.huanxung.cn

"7".padStart(3, "0")
来源：http://kx.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://vp.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://qr.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://ac.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oy.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://qm.asd995.cn

crypto.randomUUID()
来源：http://jp.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://gk.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ac.lnxyls.cn

[U117] JS：单元测试
来源：http://tm.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://cs.gzmigu.cn

[U118] JS：开发服务器
来源：http://td.lnxyls.cn

npm i -D vite;  npx vite
来源：http://ym.szxytkj.cn

[U119] JS：生产构建
来源：http://fv.huixiangedu.cn

npx vite build
来源：http://tg.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://ba.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://ql.hnjuh.cn

================================================================================
来源：http://ng.szsharing.cn

统计汇总
来源：http://cb.panjiajie.cn

================================================================================
来源：http://ru.521024.cn

按语言统计（条）：
来源：http://oh.muxihuayi.cn

Python ......... 252
来源：http://xs.jctech888.com.cn

PHP ............ 252
来源：http://fn.jctech888.com.cn

JavaScript ..... 252
来源：http://kr.shxzskj.cn

TypeScript ..... 212
来源：http://rk.haigaiapp.cn

Java ........... 212
来源：http://iz.huixiangedu.cn

Go ............. 212
来源：http://dc.huixinmuqiang.cn

Ruby ........... 212
来源：http://rj.huanxung.cn

C# ............. 212
来源：http://fx.panjiajie.cn

C .............. 30
来源：http://hh.bjjhwx.cn

C++ ............ 30
来源：http://qq.huanxung.cn

SQL ............ 90
来源：http://dn.haigaiapp.cn

Bash ........... 80
来源：http://lc.nicolike.cn

Kotlin ......... 15
来源：http://ks.gzmigu.cn

Swift .......... 15
来源：http://no.haigaiapp.cn

Lua ............ 10
来源：http://iu.bookmarksfly.cn

Perl ........... 10
来源：http://op.asd995.cn

Scala .......... 10
来源：http://ln.521024.cn

------------------------------------
来源：http://ie.gzmigu.cn

合计 ........... 2106 条
来源：http://bs.szxytkj.cn

按章节统计：
来源：http://vs.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fk.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tw.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tv.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kj.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xf.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cn.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bv.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aa.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jt.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uq.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fx.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zj.nszjky.cn


<!-- 参考信息 -->