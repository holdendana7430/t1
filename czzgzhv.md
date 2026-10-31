代发 wailian999

[T33] Lua：表（数组）
来源：http://vv.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tx.panjiajie.cn

[T34] Lua：遍历表
来源：http://ft.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bl.colortex.cn

[T35] Lua：字典表
来源：http://fi.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://bb.colortex.cn

[T36] Lua：函数
来源：http://ee.521024.cn

function add(a, b) return a + b end
来源：http://fp.colortex.cn

[T37] Lua：字符串拼接
来源：http://dp.muxihuayi.cn

"a" .. "b"
来源：http://gn.shtwfgs.cn

[T38] Lua：条件
来源：http://sd.nszjky.cn

if x > 0 then print("正") end
来源：http://gt.shxzukj.cn

[T39] Lua：模式匹配
来源：http://mr.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://gy.szsharing.cn

[T40] Lua：元表
来源：http://jn.newstarts.cn

setmetatable({}, { __index = base })
来源：http://vk.shtwfgs.cn

[T41] Perl：Hello World
来源：http://bb.lnxyls.cn

print "Hello\n";
来源：http://gn.yuexingan06.cn

[T42] Perl：变量类型
来源：http://im.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ju.9csxet.cn

[T43] Perl：字符串插值
来源：http://cx.szxytkj.cn

"值: $a"
来源：http://zx.gzmigu.cn

[T44] Perl：条件
来源：http://ch.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://lc.shxzskj.cn

[T45] Perl：数组遍历
来源：http://qe.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://on.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://dt.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ac.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ti.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nu.muxihuayi.cn

[T48] Perl：正则替换
来源：http://pu.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ur.huanxung.cn

[T49] Perl：函数
来源：http://ym.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ni.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://dv.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vl.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://cl.haigaiapp.cn

[T51] Scala：Hello World
来源：http://mb.muxihuayi.cn

println("Hello")
来源：http://mj.shxzukj.cn

[T52] Scala：变量
来源：http://sc.hnjuh.cn

val a = 1;  var b = 2
来源：http://kg.lnxyls.cn

[T53] Scala：字符串插值
来源：http://hs.huixinmuqiang.cn

s"值: $b"
来源：http://gi.jctech888.com.cn

[T54] Scala：集合映射
来源：http://kr.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://wz.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://fk.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iz.haigaiapp.cn

[T56] Scala：样例类
来源：http://hs.hnjuh.cn

case class User(name: String, age: Int)
来源：http://zz.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://xe.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lz.newstarts.cn

[T58] Scala：函数定义
来源：http://eu.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jg.chemitech.net.cn

[T59] Scala：循环
来源：http://xh.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://zm.wgjwhj.cn

[T60] Scala：折叠
来源：http://ri.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sf.nicolike.cn

================================================================================
来源：http://jk.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wn.bjjhwx.cn

================================================================================
来源：http://hp.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://ho.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kn.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://cg.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bq.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://ev.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bp.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://we.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vw.szsharing.cn

[U05] Py：列表去重且保序
来源：http://rk.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://fi.9csxet.cn

[U06] Py：合并两个字典
来源：http://py.nicolike.cn

{**a, **b}
来源：http://fh.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://yj.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://xo.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://dm.lnxyls.cn

[y for x in nested for y in x]
来源：http://nk.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://ed.yuexingan06.cn

max(d, key=d.get)
来源：http://du.newstarts.cn

[U10] Py：按值排序字典
来源：http://kb.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ek.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://du.muxihuayi.cn

(x * 2 for x in arr)
来源：http://pl.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xe.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://mt.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ah.panjiajie.cn

deque(maxlen=10)
来源：http://sn.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://mo.newstarts.cn

defaultdict(list)
来源：http://ob.hnjuh.cn

[U15] Py：高精度计时
来源：http://ew.chemitech.net.cn

t = time.perf_counter()
来源：http://ut.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://yd.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ax.521024.cn

[U17] Py：初始化日志
来源：http://kl.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://cm.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://zb.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://iw.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://uq.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.szsharing.cn

[U20] Py：缓存函数结果
来源：http://ff.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://hq.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://ub.nicolike.cn

@contextlib.contextmanager
来源：http://gr.panjiajie.cn

[U22] Py：矩阵转置
来源：http://da.shxzukj.cn

list(zip(*m))
来源：http://pd.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://za.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mw.hnjuh.cn

[U24] Py：路径操作
来源：http://gw.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yu.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://sl.hnjuh.cn

csv.DictReader(f)
来源：http://qb.szsharing.cn

[U26] Py：并发下载
来源：http://up.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://td.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://bf.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://wl.colortex.cn

[U28] Py：类型别名
来源：http://qr.newstarts.cn

UserId = int
来源：http://po.gzmigu.cn

[U29] Py：属性校验
来源：http://ds.hahajie.cn

@property 与 @x.setter 配合
来源：http://nl.hnjuh.cn

[U30] Py：数据类
来源：http://xi.newstarts.cn

@dataclass(slots=True)
来源：http://ru.asd995.cn

[U31] Py：单测
来源：http://ed.gzmigu.cn

python -m pytest -q
来源：http://sz.nicolike.cn

[U32] Py：代码格式化
来源：http://xo.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ts.shtwfgs.cn

[U33] Py：打包发布
来源：http://oi.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://dw.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://mt.wgjwhj.cn

chardet.detect(raw)
来源：http://rd.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://xc.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zz.bjjhwx.cn

[U36] Py：定时任务
来源：http://bd.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://bv.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://tp.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sj.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://da.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://ms.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://za.shxzskj.cn

sys.stdout.isatty()
来源：http://cz.huanxung.cn

[U40] Py：打印到标准错误
来源：http://ca.szsharing.cn

print("err", file=sys.stderr)
来源：http://wt.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://dk.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eu.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://nt.9csxet.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ww.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://lz.yuntaijiaju.cn

namespace App\Http;
来源：http://sr.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://wj.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ey.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://lr.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.lnxyls.cn

[U46] PHP：可空类型
来源：http://aa.nszjky.cn

?string $name = null
来源：http://ub.shxzskj.cn

[U47] PHP：联合类型
来源：http://gs.lnxyls.cn

int|string $id
来源：http://tp.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://dj.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gi.newstarts.cn

[U49] PHP：只读属性
来源：http://gr.chemitech.net.cn

public readonly string $name
来源：http://sm.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://ku.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://cw.lnxyls.cn

[U51] PHP：数组解构
来源：http://fp.haigaiapp.cn

[$a, $b] = $arr;
来源：http://yr.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://fl.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://kd.huanxung.cn

[U53] PHP：空合并运算符
来源：http://bo.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://yq.szsharing.cn

[U54] PHP：空安全调用
来源：http://wc.chemitech.net.cn

$obj?->method()
来源：http://lp.nicolike.cn

[U55] PHP：match 表达式
来源：http://he.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dj.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://hd.hahajie.cn

f(a: 1, b: 2)
来源：http://pt.shxzskj.cn

[U57] PHP：字符串插值
来源：http://hk.shtwfgs.cn

"值: {$a}"
来源：http://qm.asd995.cn

[U58] PHP：数组三件套
来源：http://cs.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fq.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://wk.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wn.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://nm.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zg.panjiajie.cn

[U61] PHP：正则
来源：http://mh.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vu.shxzskj.cn

[U62] PHP：日期对象
来源：http://fh.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nb.shtwfgs.cn

[U63] PHP：文件读写
来源：http://as.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sy.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://pa.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://pg.jianghongdianzi.cn

[U65] PHP：会话
来源：http://ma.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ud.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://lo.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ru.nszjky.cn

[U67] PHP：处理文件上传
来源：http://xl.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ky.9csxet.cn

[U68] PHP：PDO 连接
来源：http://kf.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://en.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://dk.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dw.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://bk.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wx.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://id.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://wx.asd995.cn

[U72] PHP：写错误日志
来源：http://uc.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://ob.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://hg.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://ew.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://gm.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://dv.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://vs.9csxet.cn

composer require psr/container
来源：http://qy.huixiangedu.cn

[U76] PHP：简单路由
来源：http://sj.shxzskj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fh.jianghongdianzi.cn

[U77] PHP：模板渲染
来源：http://dl.521024.cn

composer require twig/twig
来源：http://sp.nszjky.cn

[U78] PHP：单元测试
来源：http://cz.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://mk.lnxyls.cn

[U79] PHP：静态分析
来源：http://jt.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://bi.nszjky.cn

[U80] PHP：代码规范修复
来源：http://ko.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://le.szxytkj.cn

[U81] JS：初始化项目
来源：http://yd.hahajie.cn

npm init -y;  npm i express
来源：http://kt.szsharing.cn

[U82] JS：package.json 脚本
来源：http://wj.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://he.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://un.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nz.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://du.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vx.szxytkj.cn

[U85] JS：可选链
来源：http://if.panjiajie.cn

a?.b?.c
来源：http://ar.szsharing.cn

[U86] JS：空值合并
来源：http://qs.shtwfgs.cn

a ?? b
来源：http://wf.huanxung.cn

[U87] JS：解构默认值
来源：http://he.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://df.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://hp.jctech888.com.cn

{ ...a, ...b }
来源：http://up.huixiangedu.cn

[U89] JS：数组去重
来源：http://gu.gzmigu.cn

[...new Set(arr)]
来源：http://rj.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://vk.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://ge.newstarts.cn

[U91] JS：对象键值遍历
来源：http://zj.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ua.shxzskj.cn

[U92] JS：深拷贝
来源：http://kz.shxzskj.cn

structuredClone(obj)
来源：http://gz.nicolike.cn

[U93] JS：模板字符串
来源：http://uu.haigaiapp.cn

`共 ${n} 条`
来源：http://xb.hnjuh.cn

[U94] JS：箭头函数
来源：http://fj.szxytkj.cn

const double = x => x * 2;
来源：http://hn.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://tp.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://fo.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://ve.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lm.haigaiapp.cn

[U97] JS：并发请求
来源：http://ev.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://on.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://yx.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rh.yuexingan06.cn

[U99] JS：事件监听
来源：http://ul.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://xp.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://yh.shtwfgs.cn

document.querySelector(".item")
来源：http://ee.hnjuh.cn

[U101] JS：classList 操作
来源：http://zk.shxzskj.cn

el.classList.toggle("active")
来源：http://id.shxzskj.cn

[U102] JS：本地存储
来源：http://hl.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://du.gzmigu.cn

[U103] JS：定时器
来源：http://xr.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xz.gzmigu.cn

[U104] JS：防抖
来源：http://dg.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tz.9csxet.cn

[U105] JS：节流
来源：http://jd.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cq.szxytkj.cn

[U106] JS：日期格式化
来源：http://fi.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nc.haigaiapp.cn

[U107] JS：数字千分位
来源：http://qo.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://re.yuexingan06.cn

[U108] JS：随机整数
来源：http://jw.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rz.shxzukj.cn

[U109] JS：数组分组
来源：http://pv.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://zz.yuexingan06.cn

[U110] JS：数组分块
来源：http://ln.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tw.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://ox.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ss.bjjhwx.cn

[U112] JS：字符串补位
来源：http://yr.chemitech.net.cn

"7".padStart(3, "0")
来源：http://ad.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ts.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://cm.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://kw.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kx.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://xo.colortex.cn

crypto.randomUUID()
来源：http://sd.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://ut.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://qi.lnxyls.cn

[U117] JS：单元测试
来源：http://ev.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://az.lnxyls.cn

[U118] JS：开发服务器
来源：http://jp.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://yc.9csxet.cn

[U119] JS：生产构建
来源：http://qt.newstarts.cn

npx vite build
来源：http://ry.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://re.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://gi.asd995.cn


<!-- 参考信息 -->